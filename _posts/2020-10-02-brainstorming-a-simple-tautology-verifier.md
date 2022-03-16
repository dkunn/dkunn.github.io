---
layout: post
title: "Brainstorming a Simple Tautology Verifier"
date: "2020-10-02"
---

Lately, I’ve been thinking of making something simple and straightforward so I thought I’d make a tautology checker/verifier! To be quite honest, I’m not sure if the program should have a GUI or just use the command line but no matter the choice, it should be a pretty fun small project.

## Tautology Verifier
Firstly, consider what the program is actually for first. What will it do?

The primary thing that the program has to do is to verify a tautology. It’s probably the simplest part. How will it do this? There are a few options, but as this is a simple program, the method will be by constructing a truth table. I don’t really feel like making one with a natural deduction approach because for one, there are already lots of things to accomplish those, like proof assistants. Another thing is it probably won’t be very simple, and I’m not comfortable with my knowledge on formal reasoning about programs yet.

The program also has to be able to take in inputs (could be through buttons and/or manually typing with a keyboard) and build an expression that can be parsed.

Finally, the program must output a final truth table with all the values—how to display this doesn’t matter. It can be an ASCII table printed on a console, a graphical table, an excel file, a csv file, etc. All are of varying difficulties, but as always, it’s best to go for the most challenging one (in this case, likely a graphical table).

Any other additional features, maybe changing the notation used, saving an output file, assigning meaningful statements to propositions and building (mostly) coherent sentences to reason, and so on, can be implemented freely.

## Language
When thinking of what to use for this project, I initially thought Haskell or some other functional language. Why is this? Well, firstly, it’d be quite nice to get some more experience with functional programming. Secondly, the first thing that came to mind were expression trees which can be implemented with something like this:

```
data LogicExpr = Prop Bool
                | Not LogicExpr
                | And LogicExpr LogicExpr
                | Or LogicExpr LogicExpr
                | Implies LogicExpr LogicExpr
                | Iff LogicExpr LogicExpr

eval :: LogicExpr -> Bool
eval (Prop p)      = p
eval (And p q)     = eval p && eval q
eval (Or p q)      = eval p || eval q
eval (Not p)       = (not . eval) p 
eval (Implies p q) = eval p `impl` eval q
eval (Iff p q)     = eval p `iff` eval q

impl :: Bool -> Bool -> Bool
impl True False = False
impl _ _        = True

iff :: Bool -> Bool -> Bool
iff True True   = True
iff False False = True
iff _ _         = False
```

There would be a binary tree of propositions that already have their assigned truth values. An expression can easily be evaluated to a final truth value. Starting with the representation of a truth table of initial values (which can be as simple as a list of list of Bools), the whole expression is evaluated recursively, with the end result being stored in a list of Bools (where the index corresponds to the row). It would then be a simple case of applying Haskell’s all function to a condition and the list of truth values.

The only downside to using Haskell is that I’ll probably be limited to using the command line since anything involving I/O can be somewhat difficult and I’m not sure I have the time right now to invest relearning some concepts and learning new frameworks/libraries.

My other possible language of choice is Java. Revisiting OO concepts, design patterns and possibly some of the more uncommonly used features of Java will be pretty helpful. Like Haskell, I’ve not used Java that much so while it won’t be as difficult as using Haskell, it’d still be somewhat challenging and it’d definitely be useful. If I wanted, I could also dabble in making a mobile app which would be a nice experience for a change.

Another option would be to make a web application using a JavaScript framework. I have used JS in the past so I am familiar with it, but not enough to be comfortable with it.

I’m not entirely sure which to choose yet, but I’m leaning towards Java purely because I do quite like the language and would like to get more comfortable with it and OO principles. That’s not to say that this isn’t possible with something like JS, but for obvious reasons they don’t compare to Java. Incidentally, it’s possible to completely emulate a functional paradigm in Java but again, I do want to take a “right tool for the right job” approach here.

## Challenges
The aspect that stands out somewhat will be the parsing part. An approach could be to simply modify the shunting-yard algorithm and convert expressions to postfix notation then evaluate it.

Another thing to consider would be keeping track of the value of each expression and, in relation to parsing, properly handling precedence and brackets/parentheses.

Preventing unknown symbols/characters from being entered would be another problem to consider, but it’d likely not apply to approaches using buttons (like a calculator).

The last thing to consider is the structure of the whole program.

## Structure
In my mind, I imagine the program to be something like a calculator. It’s easy to think of it in an object-oriented way so for now I’m gonna assume it will be done in an OOP fashion.

![Objects]({{ "/assets/img/brainstorm_tautverify.png" | relative_url }})

This doesn’t depict every entity, but it did help with some visualisation of a potential final result. For instance, **Table** can contain **Rows** which subsequently contain **Cell**s. In practice, this’ll probably be much different but the idea of breaking things down is there.

There are also other possible GUIs, like simply having the user type in an expression, generate the table then allow them to edit the table by adding columns and so on.
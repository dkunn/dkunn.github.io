---
layout: post
title: "Informal Reasoning and Propositional Logic Basics"
date: "2020-09-30"
---


<h2>Informal Reasoning</h2>


<p>Logic is a fundamental tool for any field of knowledge out there. Behind every problem that arises, the solution can be reached by utilising logic and reasoning. Whether it's used formally or informally, it is such an important thing that even an informal or elementary knowledge of it helps in comprehension, articulation and reasoning.</p>

<p>In a similar manner, reasoning is also important and is fundamental to any task. Informally, reasoning can be thought of as being categorised into two types: deductive and inductive.</p>

<p>The first type, deductive reasoning, uses <em>a priori</em> knowledge to present a conclusion. A priori knowledge refers to that which is acquired through pure reason---that is, it does not rely on empirical evidence or sense experience. Below is a classic example of deductive reasoning:</p>

$$P_1 \text{ Socrates is a man.}$$<br>
$$P_2 \text{ All men are mortal.}$$<br>
$$C \text{ Socrates is mortal.}$$

<p>Given that the premises $P_1$ and $P_2$ are both true, then the conclusion $C$ necessarily follows.</p>

<p>This is another example which also makes use of definitions:</p>

$$P_1\text{ A bachelor is an unmarried man.}$$<br>
$$P_2\text{ John Doe is a bachelor.}$$<br>
$$C \text{ John Doe is an unmarried man.}$$

<p>The latter is, in a sense, "more" direct and analytic, making use of the definition of a bachelor; in this case, "bachelor" and "unmarried man" are synonymous and can be substituted; if a man is a bachelor, then by virtue of definition, he is necessarily an unmarried man. Both of these example utilise a form of deduction called <em>syllogism</em>. Incidentally, the second example can be slightly changed to make the structure exactly the same as the first one:</p>

$$P_2\text{ John Doe is a bachelor.}$$<br>
$$P_1\text{ All bachelors are unmarried men.}$$<br>
$$C \text{ John Doe is an unmarried man.}$$

<p>As the way of reasoning discussed here is strictly informal, it's satisfactory, for now, to simply know the format of syllogism.</p>

<p>The other basic type of reasoning is inductive reasoning (not to be confused with mathematical induction) which is based on <em>a posteriori</em> knowledge. Empirical evidence or sense experience is used in the premises to formulate a (probable) conclusion through observation of patterns in reality.</p>

$$P_1\text{ It rained on Sunday for two weeks.}$$<br>
$$P_2\text{ It is Sunday tomorrow.}$$<br>
$$C\text{ It will rain tomorrow.}$$

<p>Given that the premises $P_1$ and $P_2$ are both true, then the conclusion $C$ has a decent chance of being true based on the premises alone.</p>

<p>Of course, we know that this is obviously false. Whether it will rain on a given day is not determined by what day it is, but the use of sense experience <em>can</em> be a reasonable way to make conclusions. For instance:</p>

$$P_1\text{ Whenever I kick a round ball, it rolls.}$$<br>
$$P_2\text{ There is a basketball in front of me.}$$<br>
$$P_3\text{ A basketball is a round ball.}$$<br>
$$C \text{If I kick the basketball, it will roll.}$$

<p>This one is more reasonable. It's technically possible to argue that this isn't true, supposing that, say, the ball is glued to the ground with a strong adhesive (or some other additional qualifier of the sort), but with common assumptions, it'd be generally accepted to be a true statement.</p>

<p>Obviously, due to the use of natural language, these types of reasoning are ill-suited for most cases, such as formal proofs, unless the problem is simple enough (or you qualify statements precisely enough such that you have an infinite amount of qualifiers which "realistically" requires an infinite amount of time). Informally, these may be quite useful in formulating arguments (particularly in many fields of philosophy) that are logically reasonable with ease. These may also help in composing your thoughts on certain matters by following a slightly more rigorous line of reasoning. However, this of course isn't a substitute for the level of rigor and preciseness of formal logic.</p>


<h2>Propositional Logic</h2>


<p>A proposition may be thought of as a statement that is either true or false. This is the principle in classical logic called the law of excluded middle. It is, at first glance, reasonable, considering that it's what is experienced in reality---you are either in your room or you are not---you can't be in your room and outside your room at the same time. Or can you? There are logic systems that reject this principle, or doesn't assume it (such as intuitionistic logic), but for now I won't delve into those.</p>

<p>A statement can be represented as a proposition using propositional variables. By convention, the letters $P$, $Q$ and $R$ are commonly used to denote a proposition. Each proposition has an assigned truth value (true or false).</p>

<p>Multiple propositions can also be combined or strung together into a singular proposition using <em>logical connectives</em>.</p>

<p>The notation for logic is fairly simple. There are many other alternative notations, but here are some basic ones:</p>

<table>
<tr>
    <th>$\text{Logical Connective}$</th>
    <th>$\text{Symbol}$</th>
</tr>
<tr>
    <th>$\text{Negation}$</th>
    <th>$\neg \sim \overline{P}$</th>
</tr>
<tr>
    <th>$\text{Conjunction (And)}$</th>
    <th>$\land \cdot$</th>
</tr>
<tr>
    <th>$\text{Disjunction (Or)}$</th>
    <th>$\lor +$</th>
</tr>
<tr>
    <th>$\text{Implication}$</th>
    <th>$\implies \to$</th>
</tr>
<tr>
    <th>$\text{Equivalence}$</th>
    <th>$\iff \equiv$</th>
</tr>
</table>

<p>All of these are straightforward and self explanatory, really. Generally, $+$, $\overline{P}$ and $\cdot$ are used in Boolean Algebra, particularly when dealing with matters such as logic gates. In most cases with mathematics (and typically philosophy), $\land , \lor$ and $\neg$ are used. For the truth values, there may also be different conventions, such as using $0$ and $1$ or $\top$ and $\bot$.</p>

<p>There are special cases where the symbols may not be synonymous, or they may have subtle differences. For instance, in many situations, $\implies$ and $\to$ can be used interchangeably. However, there are some situations where they're used in different ways depending on which context the implication is utilised. The difference is quite subtle so in most cases it's not really necessary to make this distinction.</p>

<p>For logical conjunction, $P \land Q$ if $P$ and $Q$ (that is, $P \equiv \top$ as well as $Q \equiv \top$).</p>

<p>The truth value of a disjunction $P \lor Q$ depends on whether at least one is true. If $P$, then $P \lor Q \equiv \top$. An important note here is that this "or" is what is called "inclusive-or"; in this case, the only requirement for the statement's value to be true is for one of the two propositional variables to be true. As such, the question asks "Is it the case that $P$ is true and/or $Q$ is true?" instead of "Is it the case that either $P$ is true or $Q$ is true but not both?" so even if both $P$ and $Q$ were true, the statement still holds true.</p>

<p>A negated proposition $\neg{P}$ is true if and only if $P \equiv \bot$. Another way to put this is $\neg{P} \iff (P \equiv \bot)$. Like the name suggests, it "flips" or negates the value (thinking about the concept of double negatives helps in understanding what it does).</p>

<p>The most difficult one of the five is implication as it is sometimes confused with equivalence. Let's consider both this time. Suppose that we have two propositions:</p>

$$\text{Let:}\\P \equiv \text{It is sunny.} \\ Q \equiv \text{I hang my clothes outside.}$$

<p>$P \implies Q$ can be read as: "If it is sunny, then I hang my clothes outside." This can also be interpreted as: "Whenever it is sunny, I hang my clothes outside." So if it's sunny, then I hang my clothes outside. Suppose that it is sunny. Then according to $P \implies Q$, I will hang my clothes outside. If it's not sunny, then I won't. Simple. However, if I hang my clothes outside, it is not the case that it is sunny. If the proposition is instead $Q \implies P$, then this will be, but it is not.</p>

<p>Now consider equivalence which is the easiest. I have already used it using both the notations $\iff $ and $\equiv$. It is typically also referred to in text as $\text{if and only if}$.</p>

<p>Consider $P \iff Q$, or: "It is sunny if and only if I hang my clothes outside." Strange, right? Unlike the implication example, in this one, $Q$ necessarily comes with $P$ and vice versa. That is, if $P$, then $Q$ and if $Q$, then $P$. In notation form: $P \implies Q \land Q \implies P \equiv P \iff Q$. In other words, equivalence can be viewed as implication both ways.</p>

<p>There's one trap to avoid here, and it can be solved by thinking about equivalence (if and only if) as an implication both ways or even simply considering the term used for its name. In order to prove that $P \iff Q$, it's necessary to prove that $(P \implies Q) \land (Q \implies P)$.</p>

<p>Incidentally, it's also possible to represent $P \implies Q$ using $\impliedby$ like so: $Q \impliedby P$.</p>

<p>Propositional logic can be used to reason more accurately by not solely relying on natural language like the examples of informal reasoning above. Recall that the very first example follows a format called syllogism. This deductive reasoning can be represented in a similar, but different manner (there is an implicit assumption, however) using <em>modus ponens</em>:</p>

$$\text{Let:}\\P \equiv \text{Socrates is a man.}\\Q \equiv \text{Socrates is mortal.}$$

<p>Then we simply use the format for a modus ponens argument:</p>

$(P \land P \implies Q) \implies Q$

<p>In other words:</p>

$$\text{Socrates is a man and if Socrates is a man, then Socrates is mortal.}\\ \text{Socrates is a man, therefore, Socrates is mortal.}$$

<p>The proposition is also called a <em>tautology</em>---a proposition that is always true regardless of the permutation of truth values of each proposition that makes up the proposition. Notice how the statement about all men being mortal disappeared. That was what was being referred to as an implicit assumption because there is no explicit information that all men are mortal. There is simply the proposition that if you are a man, then you are mortal. This is a limitation of propositional logic and it is one where another type of logic, called predicate logic, is better equipped to handle.</p>

<p>Another example of tautology is the law of excluded middle, which can be represented as $P \lor \neg{P}$. It's not difficult to see how this is a tautology---whether $P$ is the case or not, it will always be a true statement.</p>

<p>There are a number of ways to verify whether a given proposition is a tautology. The simplest and most straightforward algorithmic way to verify a tautology is by constructing a truth table. Other ways include using natural deduction and proof assistants such as Agda, Coq and Lean. While constructing truth table is the easiest, it is somewhat of a brute-force solution so for propositions involving a large number of propositional variables, there will be significantly more rows required since all possible truth value permutations are represented. The number of rows grows exponentially ($2^n$).</p>

<h3>Side Thoughts</h3>

<p>This is my first time trying out LaTex without actively using a compiler. It was more difficult than I expected trying to get things to work as they should and it would have been much easier to type out a LaTex document and compile it manually. Fortunately, I managed to come up with some (not-so-great) band aid fixes so for now I shall use these. There seems to be some issues with rendering symbols but hopefully they're recognisable enough.</p>
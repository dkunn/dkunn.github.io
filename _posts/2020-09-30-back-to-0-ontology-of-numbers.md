---
layout: post
title: "Back to 0: Ontology of Numbers"
date: "2020-09-30"
---

## Retrospection

In the past years, I often found myself doubting what I’ve learned in school, particularly with subjects such as Mathematics. It happens in all subjects which is completely natural I suppose—as you gain more knowledge, perhaps more gaps are uncovered in what you thought you previously knew. I find that for me, this is the case especially with Mathematics. I have very vague early memories of sitting in a classroom, writing the pronunciation of numbers such as 58647, being told about roman numerals and the terms for place values: ones, tens, hundreds—tenths, hundredths, thousandths—and so on. But what were they for? I know I’ve learned them at quite a young age. I’ve been taught arithmetic at a young age. In fact, I also have memories of really struggling with subtracting two (and perhaps it could’ve even been one) or more digits using the column method (or whatever it is called) the first time I encountered such questions. This was to the point that I think I answered none of the questions correctly. In the past years, I’d been thinking: how was I able to know how to do arithmetic, and consequently, everything that follows? I don’t remember experiencing that “click” where everything suddenly makes sense, as I once had when successfully understanding how programming works after trying to do so for many times before.

The simple reason was that I wasn’t able to “connect the dots”, so to speak, back then.

I suppose this is natural, considering that I was very young. And there is, of course, another simple reason: there are many things that I didn’t understand; I thought I did, but I didn’t.

I’m grateful for having taken Religious Studies in my A levels. It’s perhaps the one thing that really pushed these thoughts to the front of my mind. Actually, I wanted to take Philosophy, but it wasn’t available so I took Religious Studies instead (though informally, it was called Philosophy and Ethics, which I thought was somewhat deceiving). The course was divided into three: Philosophy of Religion, Ethics and Developments in Religious Thought which I classified as Theology in my mind. I’m sure this is quite an accurate alternate name for it, actually. Thanks to this subject, I became acquainted with the idea of rigorous logical methods and ways of thinking about things and as such, I gained a lot of interest in everything about philosophy. I started asking with questions in my head, including concepts such as language and describing things, why certain things are as they are, and more importantly, why 1 + 1 = 2. The latter can be said as the basis of this series that I’m starting. Simply put, I’d like to reorganise my thoughts and understanding about numbers from the beginning—hence, the name “Back to 0”. This first post will probably be on the more philosophical side and the underlying ideas will probably be quite jumbled but hopefully it is coherent enough to be of some help.

In simple terms, this series of posts will be mainly about attempting to explain, using my own words as possible, how I can think of my understanding of numbers and arithmetic. I wish I could do something akin to the “proof” that 1 + 1 = 2 in the Principia Mathematica but alas, that is extremely far beyond my capacity. Another aspect of this series is to examine my understanding and look for misconceptions, illogical jumps and mistakes—making errors is part of the journey, after all.

## Separation of Language and Existence of a Thing

The idea behind this series didn’t start with a singular thought, of course. There were also other things that I’d encountered that contributed to this, such as models of computations like the lambda calculus, philosophy of language, philosophy of mathematics and so on.

I wanted to know: what can be derived “from scratch”, so to speak? What if there was language to talk about everything else but maths? First, perhaps there’s a need to delve a bit into language and describing things. There are many concepts that may be relevant here, but to discuss all of them would be impossible.

The first thing of interest to discuss is what a thing actually is. Language is used to describe things, but exactly what is a thing?

A proposition might tell something about a thing. For instance, “This monitor is large.” encodes a few pieces of information. Firstly, that the monitor is indeed large. Disregard the subjectivity of the term “large” as this is simply an assertion about the monitor’s size (relative to the origin’s frame of reference).

Secondly, there is an implicit sign of where the monitor is—this depends on the origin of the proposition. Suppose that you were using a monitor right now and you make this proposition. The universe of discourse (or perhaps more simply, the context) then changes. The “monitor” now refers to your monitor instead of mine and the property of being large is now tested upon your monitor. The truth value of such a proposition is contingent upon your monitor, but again, disregarding this, there is a clear separation here between language and the actual thing. This is true of tangible things but what about those that aren’t?

“Do numbers exist?” is a question that can yield a variety of possible answers. With intangible—or, more appropriately, abstract—things, there don’t seem to be physical existence that they can be attributed to in the same way as, for instance, every day objects can have direct attributions. An example would be concepts such as “happiness” or “beauty”. In the same way, mathematical concepts such as “one”, “two”, “infinity” and “derivative” cannot be attributed to a physical object in the same way direct attribution such as “monitor” works. Predicates (properties in semantic form) such as “large” can be indirectly attributed to the monitor in a different way than “monitor”. Nevertheless, it is still an attribution.

Consider another example; how about “happy”? What is the difference between “happiness” and “happy”?

“Happy” can be indirectly attributed to a person exhibiting this emotion; “happiness” cannot. There are reasons behind these concerning linguistics, but what about in an ontological sense?

An easier way to think of all these may be to simply think of words as labels. “Monitor” is a label for the physical object. “Large” is a label for the property or attribute of “monitor”. “Happy” is a label for the property of the person. “Happiness” is a label for the abstract idea which relates to “happy”.

A bit of introspection here:

![Different levels of reference]({{ "/assets/img/ontology_of_numbers.png" | relative_url }})

Suppose that, for each property of a thing, the label (i.e. the word used to describe the property) is directly attributed to the property, but is indirectly attributed to the object which essentially is how it is used—to convey information. Then the existence of each thing may be made up of different layers: the thing itself (which can be physical entities or manifested abstract entities) and its properties (manifested abstract entities). Note that properties can also be the thing: for example, happy, happiness and sorrow.

The labels are not part of the things they are attributed to. In referring to a singular thing, these would essentially have two layers: those that can be directly attributed to the thing (i.e. the name or alias) or the labels of the properties—in other words, the predicates. This applies to properties as well, where the alias directly attributes to the property and the predicates indirectly attributes to the property.

### Side Thoughts
I’m reminded of something like a recursive definition where a property is either a singular property with no other properties attributed to it or a property with other properties. Actually, thinking about it some more, this would end up being circular if the link is traced back far enough… (see next section) Consequently, are there properties that are singular? It’s quite a difficult thing to imagine. Furthermore, it’s probably the case that there are infinite properties which complicates matters more. Nevertheless, I’d like to proceed further with the goal of providing some sort of general basic model for a thing’s existence.

## Numbers

Using this idea of words as labels, let’s try tackling the question “do numbers exist?” To get an idea of an approach to this, perhaps another question might require answers first: “what are numbers?”.

I have an intuition and seemingly innate idea of what numbers are but it seems very difficult to put it into words, so perhaps a quick Google search is in order:

an arithmetical value, expressed by a word, symbol, or figure, representing a particular quantity and used in counting and making calculations.

From Oxford Languages (which seems to be where Google pulls definitions out from)
As always, when searching for the definition of a word, there are sometimes terms used that might not be quite clear. There aren’t to me, at least. In particular, I think it’d be somewhat difficult to explain value and quantity in a concise way. Quick Google searches of the definitions of these use the same or related words in the same way—in other words, circular, which is to be expected since that come with the nature of being a dictionary (and, of course, tautology and synonyms and all that). It is impossible to learn what things are based on definitions from dictionaries alone. So, really, the only answer would be that labels can ultimately be defined (intuitively) through a posteriori knowledge or experience. For numbers, and by definition, the idea of quantity, it’s safe to say that understanding and knowing what they are is the same way. I’ll go into more detail in a future post about this idea because it’s quite fun to discuss.

Taking into account the idea of separation of language and existence, it seems useful to define “numbers” as labels existing in the same level of abstractness as language.

There is another issue with this concerning the meaning of “exist” but suppose in this case that to “exist” means to have real existence—that is, to somehow exist in space and/or time, or be a manifested abstract thing—then the answer would be no. An important clarification here is that “real” existence does not have any special meaning; it does not, for instance, assert that manifested abstract things have Platonic existence, or that there is such a thing (i.e. existence in the Realm of Forms).

Suppose, as an alternative, that it asserts whether numbers exist as concepts that could be utilised to represent relationships (involving the idea of “quantity”—more on this later) in the real world. The answer would then be yes.

Ultimately, this view can be put in simple terms: the symbols called “numbers” are simply symbols that do not have real existence—they are simply labels. There are a number interesting ideas and concepts that can be discussed here such as those that involve Platonic ideas but I won’t delve into those.

In the image above, the idea of a quantity 1 has a name serving as its label of “1” or “one”. It is obvious that this does not have the same existence as something like the monitor object. Likewise, properties such as happy exists in a different way. As mentioned earlier, predicates such as “(is an) emotion” can be attributed (or labelled) to the thing happy and transitively, it implicitly encodes that the person is experiencing an emotion (happiness in this case). Are numbers—that is, the symbols that represent quantity—the same thing? With the help of the above, yes would be a reasonable answer—quantities are properties and the symbols called “numbers” are labels.

### Side Thoughts
I tried to avoid discussing and suggesting concepts like logicism, intuitionism and so on because they’re really complicated ideas to tackle and I don’t know enough to comfortably do so anyway.

Furthermore, with regards to the real/non-real existence part, it was somewhat difficult to contextualise. For instance, what makes language objects different from abstract properties such as large? It’s possible to claim that a person’s act of speaking a sentence gives it real enough existence, and consequently, the language objects are also given manifested existence. Truth be told, currently, the only answer I can give is to limit the model to certain contexts only. Or define language to be non-real. In any case, hopefully the point that there are different ways to think of the term “numbers” gets across.

## Summary
- Language and actual existence of a thing is separate.
- Existence can be physical or abstract.
- The existence of a thing consists of the thing itself and properties.
- Properties can be things, but as above, their existence is of a different type—that is, they are manifested abstract entities. The existence of a property is dependent on the physical expressions (e.g. size of an object). Another example is happiness which is dependent on things such as chemicals like dopamine, serotonin, etc. as well as the mouth being curved (i.e. smiling).
- Language is used to label things and properties.
- Language has abstract existence, but it does not have real existence. Language constructs are neither physical entities nor manifested abstract entities.
- The meaning or definition of a thing is defined semantically in a circular manner (tautology) and is ultimately learned through experience.
- Labels and properties have implicit links with the thing or property they represent and these work transitively—that is, labels that serve as aliases are directly attributed to the thing but the labels that serve as predicates are indirectly attributed to the thing.
- The term “numbers” refers to all the labels for quantities (i.e. “1”, “56”, “12” and so on).
- Numbers and quantities are the same idea, but existing in different levels of abstractness. Quantities are manifested abstract things while numbers are simply abstract things of thought (language object).
- As a number is a language object, it has no real existence. However, quantity has real existence (in the sense that it is property that is manifested by physical objects).
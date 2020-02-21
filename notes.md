= Introduction

Some time after learning about Design Patterns through the "Gang of Four" book,
I bought some books by architect Christopher Alexander, upon whose ideas these
"patterns" were based.  From these -- _The Timeless Way of Building_ and _A
Pattern Lanugage_ -- I learned several things which put these patterns in a
larger and more useful context.  Recently I stumbled on a link to his essay
[_A City is Not a Tree_](https://www.patternlanguage.com/archive/cityisnotatree.html)
was inspired to look into more of his works to see whether they might also apply
to software.  Specifically, I bought _Notes on the Synthesis of Form_ and the
first two volumes of _The Nature of Order_, namely _The Phenomenon of Life_ and
_The Process of Creating Life_.

I expect I'm mostly going to focus on software as experienced by developers,
since I am one, rather than software as experienced by its users, although that
would be at least as valuable an area to investigate.

I expect the format and content of this to start off unstructured and grow
gradually as I find my way round these ideas.

= Overview

== My Reading of the Sources


From my previous reading, and the inroads I've made into my recent purchases, my
understanding is that Christopher Alexander -- writing around 1950-1980 --
believes that

* the built environment can be better or worse for people, depending on how the
constructed forms provide the necessary functions;

* the things which make it better are certain high-level properties relating
form and function;

* that the properties he tries to define are saying that better forms tend to be
more like "life" in some way;

* that these better forms in particular make an environment more enjoyable to
inhabit, and more likely to be maintained and extended to fit the inhabitants'
ongoing lives;

* that it's easy for most people to recognise this "better" but hard to
construct it from scratch (as opposed to making small improvements on existing
"good" forms);

* that explaining these patterns should make it easier for people, expert or
not, to construct new environments and improve existing ones towards better
embodying them -- that is, he wants to offer not only declarative or
denotational descriptions, but also operational ones.


= A Pattern Language

== My Reading of the Source

__TODO__


= The Timeless Way of Building

== My Reading of the Source

__TODO__


= A City is Not a Tree

== My Reading of the Source

This essay basically says that in "good" cities, the meaningful physical parts
overlap and, where they do, the two things which partly overlap form another
meaningful part when taken together (not just in the overlap).  A part may be
"meaningful" in terms of its function and/or aesthetics.  More formally, he says
that the functional/physical structure forms a semilattice, rather than a
strict hierarchy.  A semilattice is a collection of sets where the union of any
two overlapping sets is also a member of the collection.  (The intersection of
those sets may not be, nor any or all subsets of a set in the collection.)

It further says that, where the recursive structure of a city forms a strict
hierarchy, its functions and hence its inhabitants end up cut off from each
other in ways which are unpleasant for those inhabitants.

== Application to Software

Given that most approaches to anything other than tiny software systems involve
hierarchical decomposition, this essay leads me to several musings.

* Is strictly hierarchical decomposition a bad thing in some way?

* Is the decomposition achieved in practice actually strictly hierarchical, in
design and/or implementation, or does it in reality tend to have overlaps.

* If the parts of a software system overlap in some way, does that result in a
semilattice?

* Could we automatically find coherent parts and measures of overlap by
analysing software in the manner of software metrics?  I'm not sure how you
would detect a "meaningful" part, nor measure overlap.

* I expect that measures of conformance "being a semilattice" might vary in
"strength" at different parts of the system (just as in physical architecture).

* How is all this affected by the fact that the parts in the design of a
software system -- to the extent that it exists explicitly, in someone's head or
in documents -- may not match 1-to-N the parts of an implementation?

* How might this relate to Conway's Law, which says that the structure of your
software will match the structure of your oprganisation?  Should software teams
intentionally overlap (in a way which thereby forms an effective larger team) in
places where the software needs to integrate through meaningful overlap?

... and, most interestingly, ...

* To the extent that a system might conform to the semilattice defintion, does
that actually make it "better" in some way?

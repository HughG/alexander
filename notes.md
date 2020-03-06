= Introduction

Some time after learning about Design Patterns through the "Gang of Four" book,
I bought some books by architect Christopher Alexander, upon whose ideas these
"patterns" were based.  From these -- _The Timeless Way of Building_ and _A
Pattern Language_ -- I learned several things which put these patterns in a
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
understanding is that Christopher Alexander -- writing around 1960-1980 --
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
denotational descriptions, but also operational ones: processes people can use.

== Timelines    

I've written about Alexander's writings in more-or-less the order I read them.
He published them in a different order:

* 1964: _Notes on the Synthesis of Form_
* 1965: _A City is Not a Tree_
* 1977: _A Pattern Language_
* 1979: _The Timeless Way of Building_
* 1980: _The Phenomenon of Life_
* ???: _The Process of Creating Life_


= Dangling Thoughts ...

I'm hoping _The Process of Creating Life_ will point me towards something in
software which might be a "refactoring towards order", by analogy with
_Refactoring to Patterns_ by Joshua Kerievsky.



= Random Other References

== TRIZ

TRIZ is an innovation and problem-solving "toolkit" which for me relates to
Alexander's work in two ways.

* It is based on generalising from successful practice.

* Some of its main tools are about ways to resolve specific conflicts.

It does talk about analysing a specific system to find conflicts in the system
but doesn't present them as a _hierarchy_, DAG, or semilattice, as in _A
Pattern Language_.

It also talks about simplifying systems (trimming) by finding away to remove
some part or effect in a system by re-using other parts or effects in that
system or its environment.  This could be seen as a step-by-step or
"refactoring" way to get to a system in which centres have more meaningful
connections.  The aim in this approach is more about practicality and
efficiency than about beauty, but there's an overlap between beauty and
parsimony.


== Geometry from Entanglement

New Scientist, 2019-09-11: _What is space-time? The true origins of the fabric of reality_
https://www.newscientist.com/article/mg24332470-500-what-is-space-time-the-true-origins-of-the-fabric-of-reality/

This article discusses research (by Sean Carroll et al. at the California
Institute of Technology) shows that, at least in simple cases, the more
entangled things are at the quantum level, the closer they are.  That is, you
can derive the property of geometry for space-time purely from abstract notions
of degrees of freedom (reduced by entanglement).

"Entropy, a measure of disorder, is directly related to entanglement: the more
entangled a region is with the rest of the world, the more entropy it contains.
...  Gravity, it appears, can arise from entanglement, rather than directly
from mass and energy.  ... Gravity, in other words, can emerge directly from
the quantum essence of reality, without quantising any assumed classical
stuff."

This feels analogous to several ideas.

* The "meaningful overlapping sets" in _The City is Not a Tree_.

* The idea in _The Nature of Order_ that centres are richer the more
relationship they have to other centres.

* Ideas I think I recall in _Notes on the Synthesis of Form_, _A Pattern
Language_, and/or _The Timeless Way of Building_, that patterns and the systems
derived from them are more effective, the more conflicts are simultaneously
resolved by a particular part of the construction.  (Although, thinking about
software, I wonder if greater overlap of effect like that would make that part
more difficult to change -- i.e., without then leaving some requirements newly
unresolved again.)

== Degrees of Life

This was a very short article (a few paragraphs) in the front section of some
issue of New Scientist, but I can't find it now.  It was about some researcher
who was interested in mathematical correspondences which vary in degree across
various systems, of which those at one extreme would be regarded as alive.
Somewhere in the middle are things like vortices in flowing water, which
maintain some sort of structure despite incoming interfering energy, and even
"reproduce" in some sense.

I wish I could find the researcher's name so I could look for further links to
the ideas in _The Nature of Order_.


= A Pattern Language

== My Reading of the Source

__TODO__

== Application to Software

__TODO__


= The Timeless Way of Building

== My Reading of the Source

__TODO__

== Application to Software

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

* I expect that measures of conformance to "being a semilattice" might vary in
"strength" at different parts of the system (just as in physical architecture).

* How is all this affected by the fact that the parts in the design of a
software system -- to the extent that it exists explicitly, in someone's head or
in documents -- may not match 1-to-N the parts of an implementation?

* How might this relate to Conway's Law, which says that the structure of your
software will match the structure of your organisation?  Should software teams
intentionally overlap (in a way which thereby forms an effective larger team) in
places where the software needs to integrate through meaningful overlap?

... and, most interestingly, ...

* To the extent that a system might conform to the semilattice definition, does
that actually make it "better" in some way?


= Notes on the Synthesis of Form

References:

* https://en.wikipedia.org/wiki/Notes_on_the_Synthesis_of_Form

* https://nplusonemag.com/issue-35/reviews/on-design-thinking/ (linked from
Wikipedia)

In Maggie Gram's article, Alexander is quoted as repudiating his earlier work,
including this book, inasmuch as they try to define a single method for solving
any design problem -- as I understand so far, any task of resolving conflicting
requirements.  It leads into this by talking about Horst Rittel opposing
"design methods" on the basis that the problems really worth solving -- "from
poverty to the need for sanitary sewers" -- were very large with very complex
context, meaning it was impossible to find a comprehensive, precise definition
of the problem ... and, therefore, of solutions or even of one correct method
for finding solutions.  Instead, basically, designers should be "allowed" or
encouraged to take all sorts of approaches.


= The Nature of Order, Book One: The Phenomenon of Life

== Notes from the Source

=== Preface

2: The general mechanistic world-view in the 20th century contributed to an
awkwardness and ugliness in the practice and output of architecture.  Getting
beauty back may require changing our world-view.

3: Beyond world-view, we need a practical theory of order: one which allows us
to both understand and make it.  Also, "I want a conception of order subtle
enough to explain the way the yellow tower makes us feel."

4: Current understandings of order in terms of mechanism don't help us create
touching beauty, harmony, and wholeness.

5: The Cartesian world-view omits personal experience and values, but it was
only intended as a way to model phenomena, not our real lives.  Alexander
contends that some statements about value can be definitely true or false (not
just opinions); in particular, clear, geometric statements about what is or
makes harmony in a built thing.

6: Because values are not in the mechanistic view, architects have come to take
"what is good" as a matter of opinion, meaning anyone's is equally valid.  They
tend to pick some simplifying principle because otherwise it's too hard to know
what to do (with no world-view about values) but the results aren't
satisfactory.  The absence of "life" from these views "makes cooperative work
... _very difficult in principle_."

7: To make buildings with life and profound order we need a view of "things in
their wholeness", not just reductionist.  Alexander's view has ornament and
function as two sides of the same coin, sees "life" in inanimate objects, and
sees order as related to our personal, human experience.  It extends the
scientific view, rather than contradicting it.

* HUGR NOTE: I wonder whether science since 1980 might  be more in accord with
this in some ways.



== My Reading of the Source

(Still reading this ...)

__TODO__


== Application to Software

__TODO__


= Synthesis

== Coming in through Design Patterns

The original Gang of Four book gives quite low-level patterns, each with some
motivation in terms of forces, in the Alexandrian style: "suppose you want X
but Y".

=== Hierarchy of Patterns

However, _A Pattern Language_ says that you really want to discover (from 
successful practice) families of patterns, joined in a DAG, loosely related to
physical levels of structure (and, therefore, to levels of detail in
construction).  The arrows A -> B in such a DAG are saying that, in applying a
pattern A to resolve a conflict by making one kind of thing, you are likely to
find that you have to resolve a conflict at a lower level by using pattern B.
Also, the patterns in this book are more abstract than those in the GoF book,
although perhaps about the same level as, for example, Martin Fowler's
_Enterprise Integration Patterns_.  Another interesting point is that the
patterns are labelled with a one-to-three-star rating indicating a degree of
confidence, based on how many other people have used or seen these patterns
and view them as successful.

=== Recursive Construction

The DAG structure above is not only telling you about related physical
structures at the same and different levels of scale, but also about how to
construct your system:

* recursively down levels of scale, by solving the higher-level contradictions
first; and,

* iteratively over time during construction, because the details of the
high-level solutions will constrain you in unforeseen ways.

This is an argument for design up front, but not too detailed.  In several
examples Alexander sketches out a mental model of the construction of the whole
system in terms of which specific patterns to apply in roughly what order, but
with the understanding that new details will be discovered at each step.

=== Maintanance and Repair

__TODO__


=== Domain-Specificity

In that book the languages are created from experience and are specific to some
domain or sub-domain.  For example, the main pattern language is a general one
about building places for people to live, and spans levels from pattern 1,
"Independent Regions" (in which "a region has at least several million people
in it", or it will be irrelevant in national government) down to pattern 251,
"Different Chairs" (in which any seating area should have "a variety of
different chairs" because different people are different sizes and prefer to
sit differently).

In _A Timeless Way of Building_ among other things he gives several examples
of applying subsets of these patterns to particular projects, such as a cottage
(Chapter 21) and a psychiatric institution (Chapter 22).  The latter includes
extra, more domain-specific patterns which were derived over a series of
workshops, based on analysis of the prospective medical staff's knowledge of
other successful institutions.

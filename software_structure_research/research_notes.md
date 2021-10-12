# Software Structure Research Notes

Other people have surely already come up with some ideas relevant to my interest
in patterns and structure of software.  This folder contains downloaded papers
and my own notes on them.

This is by no means an academic literature survey, just an intuitive attempt to
avoid entirely re-inventing the wheel.  The problem is knowing what terms to
search for.

# Starting Ideas

Something (or several things) about structure must be important, given all the
15 Patterns are about structure in some sense.  But simple ideas like class
or entity-relationship diagrams seem too "small" as concepts, or maybe too
fine-grained.  However I'm not sure what sort of "thing" I want to be
thinking about that might have structure: physical architecture is clearly
about buildings which divide up space in relation to other spaces and
features, and make it useful and enjoyable for certain purposes.  For software,
beyond the usual UML things I start thinking about: data flows and conversions;
vague TRIZ-related ideas on how Substance-Field Theory might point to ideas of
structure -- Substance = Data, Field = Code, but Code = Data -- although ...
TRIZ is more concerned about function and effects than specific spaces.)

I have a vague intuition that topology may be interesting if it lets me "see"
or otherwise detect gradients, repetitions, "Boundaries", "Deep Interlock and
Ambiguity", etc.  But I think it needs some notion of scale or abstraction as
well, otherwise it would be hard to make any sense of a full-system view for
large systems.

I also wonder if "texture" is somehow relevant, thinking about "Alternating
Repetition", "Roughness", and "Deep Interlock and Ambiguity".  I'm not sure
what texture measures one could have, and whether it could be based on the
original program code, or data; or extracted topology; or features of the
deployed system and its data flows (e.g., inter-component latencies, points of
data conversion).

I also think gradients must be relevant somehow, given "Gradients" (and, at
extremes, "Contrast"), "Deep Interlock and Ambiguity", "Alternating
Repetition"

# Search Terms

I searched for terms like the following.

* software structure metrics
* software structure
* software visualisation
* software pattern visualisation
* software texture metrics
* software topology
* topology texture
* topology gradient
* software gradient

# Results

## Quality Metrics

### Code Structure Analysis & Quality Metrics

https://schahbazali.wordpress.com/2011/06/25/code-structure-analysis-quality-metrics/

NO: Useful in general but not what I'm looking for.

Overview of a number of common (as of 2011) sofware structure metrics.  However,
these are all scalar measures over some "piece" of code -- methods, classes, or
larger -- so they don't summarise or highlight structure, only give fine-grained
measures of "goodness" for the structure.

### Science Direct "Code Metrics" Article List

https://www.sciencedirect.com/topics/computer-science/code-metrics

NO: A list of articles mentioning "code metrics".  Again not what I'm looking
for.

More advanced research into code metrics, and coding & project guidelines based
on these, but nothing about seeing structure.

### Sealights Article on Code Quality

https://www.sealights.io/code-quality/code-quality-metrics-is-your-code-any-good/

NO: Didn't learn anything new.  An "article" to sell their software development
quality monitoring solution.

### Refactoring to Patterns

MAYBE for my research in that Alexander's "15 patterns" are described as not
only things you can recognise in a structure, but as steps you can take to
evolve a structure when you need to add something new to it.  That's maybe more
like "refactoring to new features" :-)

https://www.industriallogic.com/xp/refactoring/catalog.html
Website of the book; specifically, a diagrammatic catalogue of the refactorings.

The book: https://www.informit.com/store/refactoring-to-patterns-9780321213358


## Structure

### Structure101

https://structure101.com/products/studio/

NO: not what I'm looking for but interesting / useful.

Interesting tool to let you try out refactoring of structure (extracted from
code) using a GUI, to see the results without having to edit lots of code.

### Bauhaus / Axivion

https://www.iste.uni-stuttgart.de/ps/research/projects/#id-3333f339-0

https://www.axivion.com/en/products/axivion-suite/

NO: Moderately interesting but not what I'm looking for.

Research project into software structure analysis and improvement, with
commercial spin-off.  Details of commercial product are vague and over-hype-y.


## Topology

### Software Development with the Emphasis on Topology

https://link.springer.com/chapter/10.1007/978-3-642-12082-4_28

MAYBE relevant.

Formal systems stuff.  Abstract talks about "topological functioning model"
(TFM), the point of this paper being to carry that topology knowledge through
into derived UML class diagrams.

For Alexander-related research purposes, it may be interesting to know what
TFM models and how that topology "looks".

From a general software engineering point of view, I wonder if/how this could
be applied in iterative development; it sounds a bit Waterfall to me -- first
develop the model, then write the code -- but I may be wrong.

TODO: Get access to this at some point?

### Design decision topology model for pattern relationship analysis

https://dl.acm.org/doi/abs/10.1145/2371736.2371740

MAYBE relevant.

Abstract: model Design Patterns in terms of a graph of design decisions and
their consequences and ? ... do some automated relationship analysis to ? ...
provide a clearer model (than just "designer expertise") for understanding how
the many design patterns in the ever-expanding literature "out there" fit
together???

TODO: Get access to this at some point?

### Topology analysis of software dependencies

https://www.researchgate.net/publication/220403697_Topology_analysis_of_software_dependencies

Research prototype of a tool to rank "potentially interesting" code elements
for a developer trying to understand or modify code, where the rank is based on
the topology of structural dependencies.

TODO: Get access to this at some point?

Also mentioned in https://www.researchgate.net/publication/348832106_Predicting_code_context_models_for_software_development_tasks
as the "Suade" tool, an Eclipse plugin: https://core.ac.uk/download/pdf/20881461.pdf





## Visualisation

### Wikipedia Topics

https://en.wikipedia.org/wiki/Software_visualization

https://en.wikipedia.org/wiki/Software_archaeology

https://en.wikipedia.org/wiki/Software_maps

Sofware maps typically show module hierarchy as a 2D layout, with the 3rd
dimension and/or others like colour, texture, etc. used to convey metrics.

One paper (somewhere) talked about inferring structure / layers from
class-level connections, rather than "believing" the module structure.

I'm not quite sure how this approach is expected to deal with overly-coupled
systems which can't topologically be laid out in 2D.

### Survey of Visualisation of Static Aspects of Software

https://hal.inria.fr/inria-00546158/file/visualization_static_aspects_2011.pdf

Very interesting but again not what I'm looking for.

Lots of different ways of visualising static views of software, both at a given
moment in time and as the system evolves.  Mostly research tools rather than
things a developer could just buy, I think.

I particularly liked the new-to-me concept of Voronoi treemaps.  They might go
some way towards allowing you to visualise connections in 2D but I think are
more about making the division of 2D space less visually "artificial".

### HPI / Seerene Software Maps

https://hpi.de/doellner/projects/software-dna.html (see also
https://hpi.de/doellner/publications)

https://www.seerene.com/

Sounds pretty interesting but not what I'm looking for.

Using ML and visualisation to show useful(?) information extracted from outputs
of your development tools (e.g., commit histories), even to the extent of
"inferring the real process".  Website a bit over-hype-y.

### CodeCity: 3D visualization of large-scale software

https://dl.acm.org/doi/10.1145/1370175.1370188

Can't get access to this paper.

### A review of top software architecture visualization tools

https://searchapparchitecture.techtarget.com/tip/A-review-of-top-software-architecture-visualization-tools

TODO: Maybe sign up to get at this?

### Texture-based Visualization of Metrics on Software Architectures

https://pure.rug.nl/ws/portalfiles/portal/2739853/2008ProcSoftVisByelas.pdf

Mildly interesting, but not what I'm looking for.

Use of distinct, simple 2D textures as a feature to mark some category in a
diagram; e.g., which kinds technology a module primarily involves (GUI,
logging, etc.)

### Visual Realism for the Visualization of Software Metrics

https://www.researchgate.net/publication/221193038_Visual_Realism_for_the_Visualization_of_Software_Metrics

Use of visual textures (e.g., "bumpiness" / "roughness") as a feature to
show some continuous scalar property in a diagram, e.g., degree of fan-in.


## Pattern Visualisation

### Design Pattern Reverse Engineering

https://www.ijert.org/design-pattern-detection-and-visualization-using-reverse-engineering

Aha!  Something for my research :-)

A research tool trying out ways to infer the use of design patterns by looking
pattern-matching class relationships against known patterns.

This approach might extend to inferring more abstract patterns like the ones I
half-have in mind, but it assumes you already know what patterns you're looking
for.  Hmm ... maybe there would be some way to look for "clusters" of "kinds of
relationships between classes"?

### Pattern Visualization for Software Comprehension

https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.156.6040&rep=rep1&type=pdf

Also something for my research :-)

Similar to the "Design Pattern Reverse Engineering" paper but with a GUI tool.
(I note the Uni of Montreal came up again in my searches, I think.)

Notes that automatic detection based on structure is not enough, because some
of "the" design patterns have basically the same structure.  They suggest
human review and selection, but I wonder whether you could use other clues such
as neighbouring patterns or domain-specific names in the text (since
Alexander's Pattern Languages form a domain-specific DAG).

### Interactive visualization of design patterns can help in framework understanding

https://dl.acm.org/doi/10.1145/217838.217874

Can't access this paper.  Abstract sounds interesting but _probably_ not for my
research: inferring and visualising the design patterns in a framework, in case
they're not documented well.

Other papers by same researcher (which I also can't access):
https://www.researchgate.net/scientific-contributions/Yuichi-Nakamura-70065689


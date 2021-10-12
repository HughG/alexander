# Overview

## References

See also [someone else's atetmpt to apply the 15 principles to HCI and Organisations](http://www.truthtable.com/Fifteen_Princples.html).

## Interpretations

I'm wondering whether some principles are more/only useful as post hoc guidelines (i.e., "If it doesn't look like this, you've done something wrong"), and others can be used as positive instructions (i.e., "take steps like these").

## Open Questions

Where do "tests" sit in all this?  Would they emerge from specific principles, e.g., "Positive space"?  Or are they just "things which regularly use the system, thereby revealing where it needs to be maintained or improved"?  No doubt they would be as affected (or not) by these principles, just as the production system.


# 1. Levels of Scale

## Summary

Different centres should be at the same scale, or differ in scale by at least an order of magnitude, otherwise they'll interfere with each other.  This doesn't have to be decimal orders of magnitude: I think it's anything from about "base 2" to "base 10"; maybe even "x 2/3"?

## Translation

This seems to have obvious analogues in terms of source code, such as program, function, data, and module structures.  The principle might translate to ideas like these.

* Functions should have 2-10 statements.
* Data types should have 2-10 fields.
* Modules should have 2-10 sub-modules.

Or maybe it's more like ...

* Individual function statements should be doing things "2-10 times smaller than" the overall aim of the function.

... except that's a bit wooly unless we have some more precise measure of "smaller than" beyond "conceptually".

At one point I added these, but they don't say anything about scale, so I think they're not relevant (at least, for this pattern -- they might be relevant constraints in some "software geometry" at a given Level of Scale).

* Functions should call 2-10 other functions.
* Modules should use 2-10 other modules.


# 2. Strong Centres


# 3. Boundaries


# 4. Alternating Repetition

## Random thoughts

Hmm ...

* by construction
  * as material is moved (like sand dunes)
  * as material is added (like tipi poles, supporting pillars)
* periodicity
* frequency decomposition; interference

# 5. Positive Space


# 6. Good Shape

## Interpretation

Either this is a weak principle, or I understand it weakly.  Seems like it's just "apply all the other ones".


# 7. Local Symmetries

## Interpretation

This feels fundamental, although it might be some rotational/reflectional extension of Alternating Repetition


# 8. Deep Interlock and Ambiguity

## Interpretation

This feels like an extension of Boundaries and Alternating Repetition.  Is it much of a separate principle in itself?


# 9. Contrast

## Interpretation

This feels like an extension of Gradients: the opposite ends of your gradient must be "far enough apart" and, if the extent of the gradient is smaller, the contrast is stronger.


# 10. Gradients

## Interpretation

This feels fundamental: it doesn't come from any of the others, and it explains/supports a couple of others (Contrast, and from that also Boundaries).


# 11. Roughness

## Interpretation

This feels fundamental, and linked to Alternating Repetition: when some structure has to repeat across space (alternating or not), it will have to adjust slightly to fit irregular boundaries.

I think this one is both an instruction, and probably a strong "you got it wrong" signal.


# 12. Echoes

## Interpretation

This feels like both an instruction and a "you got it wrong" signal, but not strong guidance.  I think it's saying that you should apply the same set of domain-specific patterns across "space" and Levels of Scale; and you can tell whether you've managed that or not by how strongly you can see Echoes.


# 13. The Void


# 14. Simplicity and Inner Calm

## Summary

From Alexander's description in PoCL, p. 79, this feels to me a bit like a combination of "Echoes" and "The Void": removing unneeded detail at various Levels of Scale, all across the space; with the caveat that it doesn't necessarily mean making a void where detail is removed -- maybe just simpler detail, or less detail at smaller Levels of Scale, only at larger ones?

## Interpretation

I think this is a "positive instruction": it's saying 


# 15. Not-separateness


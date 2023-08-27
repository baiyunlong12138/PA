# A Reaction Transform Language
The key part of the reaction is the atom- and bond-change list, which is also the basic idea of generic reation.

## Description
Any set of reactions which undergo the same set of atom and bond changes, regardless of the underlying molecule substrates, can be considered an example of a given generic reaction.

Which means: any reaction undergoes the same set of atom and bond changes would be considered part of the same generic reaction. This is also the fundamental parts of generic molecular generator.

## Representation
The language SMIRKS is defined for generic reactions. It is hybrid of SMILES and SMARTS in order to meet the two fundamental of generic reaction: expression of a reaction graph and expression of indirect effects.

In SMIRKS, the meaning of SMARTS [H] is changed from "any Atom with one attached hydrogen" to "A hydrogen Atom".

More details see https://www.ics.uci.edu/~dock/manuals/DaylightTheoryManual/theory.smirks.html

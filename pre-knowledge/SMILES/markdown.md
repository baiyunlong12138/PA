# SMILES: A Simplified Chemical Language
SMILES, is the abbreviation from "Simplified Molecular-Input Line-Entry System". It is a line notation for describing the strucuture of chemical species using short ASCII strings, which can be converted back into 2D or #d models.


## Specification Rules
Each element of molecular need to be considered: Atom, Bond, Branch, Cyclic structure and disconnected structure.

Atoms are represented by their atomic symbols. 
Each non-hydrogen atom is specified independently by its atomic symbol enclosed in square brackets, *[]*.
Elements in the "organic subset" B, C, N, O, P, S, F, Cl, Br, and I may be written without brackets if the number of attached hydrogens conforms to the lowest normal valence consistent with explicit bonds.

Single, double, triple, and aromatic bonds are represented by the symbols -, =, #, and : .


```{figure} ./picture/smiles.png
:height: 250px
:name: Syntax

Some syntaxs of SMIELS
```

## Canonicalization
One import thing about SMILES is the canonicalization, because each molecular has multiple valid SMILES notations. Most of the tools only accepted the canonicalized SMILES, also known as "unique SMILES".

## Isomeric SMILES
Isotopes can also be presented using SMILES. There are also special syntax for chiral specification.


See more details under this [link](https://www.ics.uci.edu/~dock/manuals/DaylightTheoryManual/theory.smiles.html#RTFToC26).


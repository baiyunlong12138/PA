# SMARTS: A Language for Describing Molecular Patterns
<span style="font-size:18px;">
SMARTS is a language that are used to specify substructures, it is an extension of SMILES, which means they share the same syntax.
One can use SMARTS to search a specific substructure in a database. In fact, almost all SMARTS are valid SMARTS targets.
All SMILES expressions are also valid SMARTS expressions.
</span>

```{important}
SMARTS is used to define the reaction pattern.
```


## Logical Operators
<span style="font-size:18px;">
One of the biggest feature for SMARTS is the logical operators, which allow user to search more complex combination.
</span>

```{list-table}
:header-rows: 1
:name: SMARTS Logical Operators

* - Symbol
  - Expression
  - Meaning
* - Exclamation
  - !e1
  - not e1
* - Ampersand
  - e1&e2
  - e1 and e2 (high precedence)
* - Comma
  - e1,e2
  - e1 or e2
* - Semicolon
  - e1;e2
  - e1 and e2 (low precedence)
```

High precedence operator means they are evaluated first.

# Example
Here is a detailed example of interpretation of Logical operators:

```{figure} ./picture/logicOp.png
:height: 350px
:name: LogicalOp

Example of Logical Operator and its Meanning
```

**More details** see under [link](https://www.ics.uci.edu/~dock/manuals/DaylightTheoryManual/theory.smarts.html).
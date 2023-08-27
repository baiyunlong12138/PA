# Manual of the generator
In this chapter, a comprehensive user guide will be introduced, and all necessary packages and libraries are listed below. 

## Installation

Each project can easily be installed using poetry or pip. Here pip is recommeneded.

**Required Packages**: 
* RDkit
* pandas
* jinja2

Install all of them using:
```
pip install RDkit
pip install pandas
pip install jinja2
```

```{note} This code is running by jupyter-notebook, also make sure you have all needed packages installed
```

## Run the code

The software will need two files: 
* input reactant file
* input pattern file

which 
* input reactant file contains a list of SMILES of reactant
* input pattern file contains a list of SMARTS of reaction patterns

Just replace the content of these two files to your desired `reactants` and `reaction patterns`. The code will automatically give you a table that contains the corresponding production.
How to use Chemical coding language, see $SMARTS$.
### Important function 

Inside the code, several RDkit functions are used. They have different syntaxs and input parameters for different situations. It is important to understand how the function works, in order to deal with more complicated reaction.
**Later** we will maybe integrated them inside the code.

Here is the list of them:
 
* Chem.MolFromSmiles
* Chem.MolFromSmarts
* Chem.MolToSmarts
* Chem.MolToSmiles
* Chem.Draw.MolToImage
* AllChem.ReactionFromSmarts
* Chem.SDWriter
* AllChem.Compute2DCoords


### Important knowledge of class in code

#### The class molecule
molecule is a class defined by RDkit.
**Remember**: Chemical coding languages are just strings, they are not been manipulate directly. But first been converted into `molecule` class. 

Then the object of `molecule` class can be converted to image, can be put under certain reaction patterns, also can be converted to coordinate display files. 

#### The class reaction
In RDkit, the reaction is a specific class, which can be generated from $SMARTS$.

Then the object can execute reation for reactants.

See more [Details](https://github.com/rdkit/rdkit/tree/master)



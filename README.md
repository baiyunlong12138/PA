# PA
Projekt Arbeit RWTH 2023 MODES

by Yunlong Bai, Shiyao Ju.
08.2023
Aachen

# Installation

First, install all the required packages for this documentation.
Open terminal, run
```
pip install -r requirements.txt
```

The `requirements.txt` can be found directly under the root.

## Compiling the documentation
After installing all the packages and open terminal under this file, build the documentation via
```
jupyter-book build PA
```
And open it without (substitute `firefox` with your favorite browser)
```
firefox /_build/html/index.html
```
You can clean the build directory with
```
jupyter-book clean docs
```



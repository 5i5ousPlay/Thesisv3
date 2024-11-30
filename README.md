Thesis v3 package so our code isnt the messiest thing ever

# Installation

Go to the directory you want to work in and clone the repository
using the following command from within your project directory:

```commandline
git clone https://github.com/5i5ousPlay/thesisv3.git
```
Your project directory should look like this.

```directory
Project Directory Structure

project_directory
|-thesisv3
    |-analysis
    |-building
    |-preprocessing
    |-tests
    |-utils
    |-validation
    |-__init__.py
|-requirements.txt
|-setup.py
```

Create a virtual environment in this project directory using the following
command.

```commandline
python -m venv venv
```

Start the virtual environment with:

```commandline
venv\Scripts\activate
```

Your project directory should now look like this.

```directory
Project Directory Structure

project_directory
|-thesisv3
    |-analysis
    |-building
    |-preprocessing
    |-tests
    |-utils
    |-validation
    |-__init__.py
|-requirements.txt
|-setup.py
|-venv
```

To install the package in editable mode (you can edit the code while testing it in
a notebook or something), run the following command:

```commandline
pip install -e .
```

This will install the thesis package and all the necessary dependencies it has.

## External Dependencies

### Grakel
Just install some python stuff from the Windows Virtual Studio SDK:
https://learn.microsoft.com/en-us/visualstudio/python/working-with-c-cpp-python-in-visual-studio?view=vs-2019#prerequisites

### Music21 & Musescore
TODO: Al can put the installation things that need to be done to get musescore / music21
running properly


# Importing the Library

Make sure that wherever you're coding it's on the same level as the 
package directory.

```directory
Project Directory Structure

project_directory
|-thesisv3
    |-analysis
    |-building
    |-preprocessing
    |-tests
    |-utils
    |-validation
    |-__init__.py
|-notebook.ipynb <-------- your notebook or script or whatever
|-requirements.txt
|-setup.py
|-venv
```

You can import stuff from the library like so:

```python
from thesisv3.validation.tuners import KNNGraphTuner
```

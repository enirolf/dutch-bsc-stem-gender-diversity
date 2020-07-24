# Gender diversity in Dutch academic STEM programs

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/enirolf/dutch-bsc-stem-gender-diversity/master?filepath=stem-gender-diversity.ipynb)

This repository is meant to give insight into the (lack) of gender diversity in STEM programs at Dutch universities. We used DUO's open data ([here](https://duo.nl/open_onderwijsdata/databestanden/ho/ingeschreven/wo-ingeschr/)) for this purpose.

## Viewing the notebook

Check [nbviewer](https://nbviewer.jupyter.org/github/enirolf/dutch-bsc-stem-gender-diversity/blob/master/stem-gender-diversity.ipynb) to for the notebook as a static HTML page. If you want to play around, add stuff, etc., check it out on [binder](https://mybinder.org/v2/gh/enirolf/dutch-bsc-stem-gender-diversity/master?filepath=stem-gender-diversity.ipynb).

## Running it locally

If you want to contribute to this repo or run the notebook locally, follow the steps below.

The preferred method of running the notebooks is by using a *virtual environment* ([venv](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)). Install it using the following commands (make sure you have Python 3 installed. We use Python 3.8 but earlier versions should also be supported):

For Linux/macOS:

```bash
$ python3 -m pip install --user virtualenv
```

or, if you don't want to use `pip` (Ubuntu only):

```bash
$ sudo apt install python3-virtualenv
```

For Windows:

```bash
$ py -m pip install --user virtualenv
```

### Creating and activating the virtual environment

Creating a new virtual environment can be done by running the following commands:

```bash
$ virtualenv .venv/ -p /usr/bin/python3
$ source .venv/bin/activate
$ pip install -r requirements.txt
$ ipython kernel install --user --name=.venv
```

- The first line creates a new environment. You only have to run this command once.
- The second line activates the environment. You need to run this command each time you revisit the project.
- The third line installs all project dependencies in the virtual environment. It is good practice to run this command after each `pull`, since new packages may have been added.
- The fourth line installs a Jupyter kernel inside our virtual environment so we can run the notebook.

To exit the environment, simply type

```
$ deactivate
```

Remember to reactivate the environment when you return to the project.

It is possible to run the project without a virtual environment, though not recommended, since it might interfere with the Python dependencies currently installed on your machine. 

# ProcessMiningClass
Implementation of examples from D.R. Ferreira, A Primer on Process Mining: Practical Skills with Python and Graphviz, Springer, 2017

## Jupyter lab installation
We are going to install Jupyter lab under Python 3.6 locally.

First, go to the link [Python 3.6 install](https://www.python.org/downloads/release/python-360/) and download the corresponding version of Python 3.6 of your operative system and install it. Frequently, some version of Python is pre-installed in your system, but another version of Python.

You can find the just installed Python 3.6 with the command in the local Terminal
  which python3
Let us suppose, Python 3.6 is installed in /usr/bin/python3

# create a virtual environment with python 3.6
virtualenv --python=/usr/bin/python3 env_py3.6

# activate the virtual environment named 'env_py3.6'
source env_py3.6/bin/activate

# install jupyter lab in (env_py3.6)
pip install jupyterlab

# optionally, you can install more packages, for instance
pip install matplotlib
pip install graphviz

# optionally, generate output suitable for requirements file
pip freeze

# optionally, generate a requirements file and then install it in another environment
pip freeze > requirements.txt
pip install -r requirements.txt

# run jupyter lab in (env_py3.6)
jupyter lab

# the local web page of jupyter lab will appear automatically (after some seconds) on your web browser, for example:
http://localhost:8889/lab

# logout from the environment 'env_py3.6'
deactivate

## Workflow mining

## Organizational mining

## Performance mining


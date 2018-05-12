# ProcessMiningClass
Implementation of examples from D.R. Ferreira, A Primer on Process Mining: Practical Skills with Python and Graphviz, Springer, 2017

## Jupyter lab installation
We are going to install Jupyter lab under Python 3.6 locally.

First, go to the link [Python 3.6 install](https://www.python.org/downloads/release/python-360/) and download the corresponding version of Python 3.6 of your operative system and install it. Frequently, some version of Python is pre-installed in your system, but a different version of Python 3.6.

You can find the just installed Python 3.6 with the command in the local Terminal

    which python3
  
Let us suppose, Python 3.6 is installed in /usr/bin/python3. Now, we will create a *virtual environment*, where a set of packages will be installed and executed independently of packages installed in the local system. `virtualenv` is an excellent way to ensure a set of packages for running Jupyter lab and our particular applications.

Now, we will create a virtual environment with Python 3.6. This instruction will create a fold with the name `env_py3.6` and will install some basic Pyhton packages. Let us note that `/usr/bin/python3` is the location of Python 3.6 obtained from the instruction `which python`.

    virtualenv --python=/usr/bin/python3 env_py3.6

Then, we will activate the virtual environment named `env_py3.6`. This will activate a prompt `(env_py3.6)`.

    source env_py3.6/bin/activate

Now, we will install Jupyter lab in the environment (env_py3.6):

    pip install jupyterlab

It's done! Optionally, you can install more packages, for instance

    pip install matplotlib
    pip install graphviz

If you want, you can generate output suitable for requirements file with all installed packages

    pip freeze

Optionally, generate a requirements file and then install it in another environment

    pip freeze > requirements.txt
    pip install -r requirements.txt

Finally, run jupyter lab in (env_py3.6)

    jupyter lab

Then, the local web page of jupyter lab will appear automatically (after some seconds) on your web browser, for example: http://localhost:8889/lab

For log out from the Jupyter lab running, press `Ctrl-C`, the log out from the environment `env_py3.6`

    deactivate

## Workflow mining

## Organizational mining

## Performance mining


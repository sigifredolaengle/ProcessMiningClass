# Process Mining Class
Implementation of examples from D.R. Ferreira, *A Primer on Process Mining: Practical Skills with Python and Graphviz*, Springer, 2017

## Jupyter lab installation
We are going to install Jupyter lab under Python 3.6 locally.

First, go to the link [Python 3.6 install](https://www.python.org/downloads/release/python-360/) and download the corresponding version of Python 3.6 of your operating system (MacOs, Linux, or Windows) and install it. Frequently, some version of Python is pre-installed in your system, but a different one version of Python 3.6.

You can find the just installed Python 3.6 with the following command in the local Terminal

    $ which python3
  
Let us suppose, Python 3.6 is installed in `/usr/bin/python3`. Now, we will create a *virtual environment*, where a set of packages will be installed and executed independently of packages installed in the local system. `virtualenv` is an excellent way to ensure running Jupyter lab and your particular applications correctly.

Now, we will create a virtual environment with Python 3.6. The following instruction will create a fold with the name `env_py3.6`, where `virtualenv` will install some basic Python packages. If you do not have installed `virtualenv`, then install it by following instructions in [virvtualenv installation](https://virtualenv.pypa.io/en/stable/installation/). Let us note that `/usr/bin/python3` is the location of Python 3.6 obtained from the instruction `$ which python`. In addition, let us note that the folder `env_py3.6` is not necessarily the folder of your data! It is just a folder with right packages for execution of Jupyter lab. Creating the virtual environment:

    $ virtualenv --python=/usr/bin/python3 env_py3.6

Then, we will activate the virtual environment named `env_py3.6`. This will activate a prompt `(env_py3.6)`.

    (env_py3.6) $ source env_py3.6/bin/activate

### Stet-by-step installation

Now, we will install Jupyter lab in the environment `(env_py3.6)`:

    (env_py3.6) $ pip install jupyterlab

It's done! Optionally, you can install more packages, for instance

    (env_py3.6) $ pip install matplotlib
    (env_py3.6) $ pip install graphviz
    (env_py3.6) $ pip install networkx
    (env_py3.6) $ pip install scipy

If you want, you can generate output suitable for requirements file with all installed packages

    (env_py3.6) $ pip freeze

Optionally, generate a requirements file and then install it in another environment:

    (env_py3.6) $ pip freeze > requirements.txt

### Installation with `requirements.txt`

The second form for installing is simpler and it uses `requirements.txt`, which you can download from this GitHub:

	(env_py3.6) $ pip install -r requirements.txt

### Running Jupyter lab

Finally, run jupyter lab in the environment `(env_py3.6)`:

	(env_py3.6) $ jupyter lab

Then, the local web page of jupyter lab will appear automatically (after some seconds) on your web browser, for example: http://localhost:8889/lab

For log out from the Jupyter lab running, press `Ctrl-C` in the Terminal, then log out from the environment `env_py3.6` with the following instruction:

    (env_py3.6) $ deactivate

For erasing the environment:

	$ rm -rf env_py3.6
	
### Re-running

Simply, in your Terminal write:

	$ source /Users/laengle-uchile/env_py3.6/bin/activate

Where `/Users/laengle-uchile/env_py3.6/` is the global location of the virtual environment `env_py3.6`. Then write:

	(env_py3.6) $ jupyter lab
	
### Summarizing

The [video](https://www.dropbox.com/s/pbzwvwldiyveq8p/install_jupyterlab.mov?dl=0) contains an animated summary of the installation procedure of Jupyter lab.
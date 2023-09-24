

### References

[python environment setup](https://gist.github.com/stormasm/7bd667d6b8629e54f85328215e49520e)

### How To

[How to set up an environment with venv](https://arelle.readthedocs.io/en/latest/contributing.html#setting-up-your-environment)

* Fork the Arelle repo
* Clone your fork: git clone git@github.com:<your-github-username>/Arelle.git
* Install pyenv
* Install a supported version of Python. For example, pyenv install 3.11.5
* Create a virtual env using the Python version you just installed. For example, PYENV_VERSION=3.11.5 pyenv exec python -m venv venv
* Activate your environment: source venv/bin/activate
* Install dependencies: pip install -r requirements-dev.txt

Verify you can run the app
* GUI: python arelleGUI.pyw
* CLI: python arelleCmdLine.py

### venv versus virtualenv

[Difference between venv and virtualenv](https://pythonhow.com/what/what-is-the-difference-between-venv-pyvenv-pyenv-virtualenv-virtualenvwrapper-pipenv/)

What is the difference between venv, pyvenv, pyenv, virtualenv, virtualenvwrapper, pipenv, etc?
All of these tools are used to create isolated Python environments, but they differ in terms of their purpose, functionality, and the level of complexity they provide. Here there's a wider explanation:

1. venv: This is a built-in module in Python 3.3 and later versions that allows you to create virtual environments in Python. It creates a new Python environment with its own site directories, which can be used to install and manage packages for specific projects. It's simple, lightweight, and easy to use.

2. pyvenv: This is a deprecated tool in Python 3.6 and later versions that is similar to venv. It's no longer recommended to use this tool as it has been replaced by the venv module.

3. pyenv: This is a tool that allows you to manage multiple versions of Python on your machine. It's not specifically designed for creating virtual environments, but it allows you to switch between different versions of Python on the fly.

4. virtualenv: This is a popular third-party tool that allows you to create isolated Python environments. It works with both Python 2 and 3 and allows you to create virtual environments with different Python versions, which can be useful for testing your code across different Python versions.

5. virtualenvwrapper: This is a set of extensions to virtualenv that makes it easier to manage virtual environments. It provides commands to create, activate, and delete virtual environments, and allows you to organize your environments in a more structured way.

6. pipenv: This is a tool that combines virtual environments with package management. It creates a new virtual environment for each project and automatically installs the required packages from a Pipfile. It's designed to simplify the process of managing dependencies for your projects and provides a simpler interface than virtualenv.

In summary, venv and virtualenv are similar in functionality but differ in implementation, where venv is a built-in module in Python 3 while virtualenv is a third-party tool. pyvenv is a deprecated tool that has been replaced by venv. pyenv is a tool that allows you to manage multiple Python versions on your machine. virtualenvwrapper is an extension to virtualenv that provides additional functionality for managing virtual environments. pipenv combines virtual environments with package management.

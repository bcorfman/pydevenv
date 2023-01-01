# pydevenv
Sets up a Python project in a Mac OS X- or Linux-based environment with VSCode, git, and Poetry support. Once the project is configured, the script then creates a Git repo and pushing the resulting project files up to GitHub with an initial commit. It's basic project-level Infrastructure-as-Code (IaC) for how I do things with Python. Maybe you'll find it useful too.

## Prerequisites
* Python 3.7 or higher
* Install [Poetry](https://python-poetry.org). 
* Install [GitHub CLI](https://cli.github.com). 

## Setup
* Clone the `pydevenv` repo. 
* Create a $PYDEVENV environment variable with a path to your local copy of the `pydevenv` repo.
* Create a `pat.txt` file in the pydevenv folder. The `pat.txt` should contain your GitHub Personal Access Token. This PAT must have ability to create a repo, commit files and push them to GitHub. (To create the PAT initially, go to your GitHub profile and select "Settings": "Developer Settings": "Personal Access Tokens": "Tokens (classic)" along the left-hand menu.)
* Finally, add the `pydevenv` folder to your PATH.

## Run 
* From a command prompt inside your development folder, type `pydevenv [project_name]`, e.g., `pydevenv helloworld`.
  - NOTE: `pydevenv` will use the Python executable that it finds first on your PATH when setting up the virtual environment for your project. I use [`pyenv`](https://github.com/pyenv/pyenv) to choose the specific Python version I want before calling `pydevenv`. 
* Once the script finishes, you will have a Python project named project_name under Git source control, and a copy of your new project on GitHub as well.

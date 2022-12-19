# pydevenv
Sets up a Python project on Mac OS X with VSCode, git, and Poetry support before creating and pushing the project files up to GitHub with an initial commit. In other words, it's some basic project-level Infrastructure-as-Code (IaC) for my idea of a "best" development environment. I'll continue to evolve this idea of "best" over time as I discover improved ways to do things.

## Prerequisites
* Python 3.7 or higher
* Install [Poetry](https://python-poetry.org). (I would much rather use PDM as my dependency manager, but I can't script my choices or defaults like I can with Poetry.) 
* Install [GitHub CLI](https://cli.github.com). 
* Once you've cloned the pydevenv repo, include a `pat.txt` file in the folder that contains your GitHub Personal Access Token. This PAT must have ability to create a repo, commit files and push them to GitHub. (If you're having trouble locating this feature, go to your GitHub profile, and select "Settings": "Developer Settings": "Personal Access Tokens": "Tokens (classic)" along the left-hand menu.)
* Add the `pydevenv` folder to your PATH.

## Run 
* From a command prompt inside your development folder, type `pydevenv [project_name]`, e.g., `pydevenv helloworld`.
  - NOTE: `pydevenv` will use the Python executable that it finds first on your PATH when setting up the virtual environment for your project. I use [`pyenv`](https://github.com/pyenv/pyenv) to choose the specific Python version I want before calling `pydevenv`. 
* Once the script finishes, you will have a Python project named project_name under Git source control, and a copy of your new project on GitHub as well.

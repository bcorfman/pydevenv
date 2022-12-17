# pydevenv
Sets up a Python project on Mac OS X with VSCode, git, and Poetry support before creating and pushing the project files up to GitHub with an initial commit. In other words, it's some basic project-level Infrastructure-as-Code (IaC) for setting up my development environment the way I want. The setup will continue to evolve over time as I hopefully discover better ways to do things.

## Prerequisites
* Python 3.7 or higher
* Install [Poetry](https://python-poetry.org). (I would rather use PDM as my dependency manager, but I can't script my choices or defaults like I can with Poetry.) 
* Install [GitHub CLI](https://cli.github.com). 
* Once you've cloned the pydevenv repo, include a `pat.txt` file in the folder that contains your GitHub Personal Access Token. This PAT must have ability to create a repo, commit files and push them to GitHub. (If you're having trouble locating this feature, go to your GitHub profile, and select "Settings": "Developer Settings": "Personal Access Tokens": "Tokens (classic)" along the left-hand menu.)
* Add the `pydevenv` folder to your PATH.

## Run 
* From a command prompt inside your development folder, type `pydevenv [project_name]`, e.g., `pydevenv helloworld`.
* Once the script finishes, you will have a basic Python project under Git source control, with a copy of your new project on GitHub as well.

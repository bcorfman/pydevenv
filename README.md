# pydevenv
Sets up a Python project on Mac OS X with VSCode, git, and Poetry support before creating and pushing the project files up to GitHub with an initial commit.

## Prerequisites
* Python 3.7 or higher
* Install [Poetry](https://python-poetry.org).
* Install [GitHub CLI](https://cli.github.com).
* Once you've cloned the pydevenv repo, include a `pat.txt` file in the folder that contains your GitHub Personal Access Token. This PAT must have ability to create, commit and push to GitHub. (If you're having trouble locating this, go to your GitHub profile, and select "Settings": "Developer Settings": "Personal Access Tokens": "Tokens (classic)" along the left-hand menu.)
* Add the `pydevenv` folder to your PATH.

## Run 
* From a command prompt inside your development folder, type `pydevenv [project_name]`, e.g., `pydevenv helloworld`.
* Once the script finishes, you will have a basic Python project under Git source control, with a copy of your new project on GitHub as well.

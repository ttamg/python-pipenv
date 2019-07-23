# python-pipenv
python starter project using pipenv

The purpose of this is to give a good starting point for a new python project using a virtual environment and using the **pipenv** utility.


## Prerequisites

You need to have the following installed on your machine:
*   Python 3.6 - google how to install python 3.6 if you do not have this
*   Pipenv - try `pip install pipenv` or see here for instructions https://docs.pipenv.org/en/latest/
*   VS Code, or an alternative IDE of your choice - https://code.visualstudio.com/download


## Quickstart

To pull down this starter image and get going:

1.  Download this starter project into a brand new directory on your machine.
2.  Change the name of the directory for your new project name now if you like
3.  CD into the project directory 
4.  Create the virtualenvironment using the command `pipenv shell` on the commandline - this will create a new virtual environment which can be activated at any time by typing `pipenv shell` when in this directory.
5.  Install the dependencies in the **Pipfile** by using `pipenv install --dev --pre` to install just the development and production packages.  Note that to install just the production packages you use `pipenv install`
6.  Type `code .` to load VS Code in this project
7.  From the menu select **Python: Select Interpreter** and select the new virtual environment that we just created with the new project name
8.  Get coding!

If you wish to commit your project to a new git project, from the command line run `git init` to set up a new git repository.


## Why use Pipenv?

**pipenv** controls the dependencies and sets up a separate virtual environment.  This means that you do not need to manually create a new virtual environment with a new project which can be a bit of work if you are not doing it regularly.  **Pipenv** makes it easier

Within the `Pipfile` the dependencies are stored.  There are separate dependencies for production (under `[packages]`) and for development (under `[development]`).  This can be edited manually, but better is to install and uninstall using **pipenv** on the command line instead.  See below for instructions.

The `Pipfile.lock` can be used to pin the packages to particular version numbers.  

Some useful **pipenv** commands:

*   Instead of doing any `pip install` always use `pipenv install` instead
*   `pipenv --rm` removes the full virtual environment and can then be reinitialised from scratch
*   `pipenv clean` removes any packages which are installed but are not specified in the Pipfile
*   `pipenv install [package name]` installs a new package and adds to the Pipfile
*   `pipenv install [package name] --dev` installs a new package but only for development (e.g. test packages)
*   `pipenv uninstall [package name]` removes a package from the virtual environment and from the Pipfile
*   Type `pipenv` to see help on this.

This is a useful guide to Pipenv - https://realpython.com/pipenv-guide/


## Using GIT

For committing and sharing projects, use **git**.

Initialise a new git repository using `git init` on the command line from within the project root directory.

Some useful **git** resources:

*   https://realpython.com/python-git-github-intro/
*   https://git-scm.com/book/en/v1/Getting-Started-Git-Basics


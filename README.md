# Notebook starter

[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

A lightweight template to help teams collaborate with Jupyter Notebooks in VS Code. 

## Getting started

1. Use the template to create a new repository.
2. Open in VS Code (at this time it must be VS Code Insiders).
3. Install the recommended exentsions when prompted.
4. Open a terminal and run: `pip install -r requirements.txt`.
5. Run: `pre-commit install`.
6. Create `.py` files as needed, then right click a file and select `Open as a Jupyter Notebook` to open in a notebook format.

## Continuous integration

The template is ready for continuous integration out of the box. All that is needed is to sign-in, using GitHub, here: https://pre-commit.ci/.

## FAQ

- Why use this template?
  - This template helps when you want to use notebooks with version control (Git). `.ipynb` files store and update metadata that makes version control hard. This template solves this problem using extenstions that let you work with `.py` scripts through a notebook interface. It also use `pre-commit` to enforce consistent styling of these scripts.
- Why can't I open my `.py` file as a notebook (more than once)?
  - This template is affected by the following issue: https://github.com/notebookPowerTools/vscode-jupytext/issues/9. The issue means that the same `.py` file cannot be opened as a notebook twice in succession. The issue can be worked around by alternating between two `.py` files.
- Why do I get an error message when trying to make a commit?
  - If black makes a change to a file, an error message will be displayed. This is intentional - see the answer from the author here: https://stackoverflow.com/questions/58398995/black-as-pre-commit-hook-always-fails-my-commits. Review the applied changes and commit again if you are happy.

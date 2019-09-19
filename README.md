# Pre-commit hooks

This repo contains hooks that can be used by projects through the [pre-commit framework](https://pre-commit.com/).

## Usage

* [Install pre-commit](https://pre-commit.com/#install) - note that our Python projects already have pre-commit as a dependency
* Create the `.pre-commit-config.yaml` file in your project and [add hooks](https://pre-commit.com/#plugins) to run
* Run `pre-commit install` to enable the hooks (or `pipenv run pre-commit install` for our Python repos)

## Adding hooks

Hook definitions are in the `.pre-commit-hooks.yaml` file. This file lists all the available hooks that can be used.

To create a new hook, you can create simple `system` hooks directly in the config file. If you want to create a more complex hook, a variety of languages are available. Create a file in a `pre_commit_hooks` directory in this repo, add it to the `.pre-commit-hooks.yaml` file, and it can be used in any project.

Details on configuration and testing hooks locally can be found in the [Creating new hooks](https://pre-commit.com/#new-hooks) documentation.
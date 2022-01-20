# {{ cookiecutter.project_name }}


{{ cookiecutter.project_short_description }}

* [MKDocs Documentation](https://squidfunk.github.io/mkdocs-material/getting-started/)


## Create environment

For convince sake a [`Taskfile`](https://github.com/adriancooney/Taskfile) has been generated that contains the tasks to build your documentation project. 

I would recommend to create an alias, like so 

```bash
# Run your tasks like: run <task>
alias run=./Taskfile
```

Then create a virtual environment.

```bash
run create-venv
```

By default the virtual env will be named after your `project_slug`. So to activate it:


```bash
source .virtualenv/<project_slug>/bin/activate
```

To install dependencies:

```bash
run pip-install
```

Serve the docs on localhost

```bash
run docs-serve
```

To build the static site for the docs

```bash
run docs-build
```

Credits
-------

This package was created with Cookiecutter_ and the [larsagny/cookiecutter-mkdocs-material](https://github.com/larsagny/cookiecutter-mkdocs-material) project template.

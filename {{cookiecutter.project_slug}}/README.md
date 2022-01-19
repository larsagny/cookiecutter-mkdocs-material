# {{ cookiecutter.project_name }}


{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Free software: {{ cookiecutter.open_source_license }}
{% endif %}
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

By default the virtual env will named after your `project_slug`. So to activate it:


```bash
. .virtualenv/<project_slug>/bin/activate
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

This package was created with Cookiecutter_ and the `larsclaussen/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage

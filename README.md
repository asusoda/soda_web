# `soda_web`

## Introduction

Welcome to the `soda_web` repository, the Django backend project
managed with Poetry for ASU's [Software Developers
Association](https://thesoda.io). This README provides essential
instructions on setting up and running our Django-based web
application.

## Prerequisites

Before you start, ensure Python is installed on your system. Download
it from [python.org](https://www.python.org/downloads/).

## Installing Poetry

Poetry is our tool for managing dependencies. To install Poetry:

1. Visit the [Poetry installation
   guide](https://python-poetry.org/docs/#installation).
2. Follow the instructions for your operating system.
3. Check the installation by executing `poetry --version` in your
   command line.

## Setting Up "soda_web"

Clone the "soda_web" repository and navigate to its directory:

```bash
git clone https://github.com/asusoda/soda_web.git
cd soda_web
```

Inside the directory, use Poetry to install dependencies:

```bash
poetry install
```

This command reads `pyproject.toml` and installs all the necessary
dependencies for "soda_web".

## Activating the Virtual Environment

Poetry creates a virtual environment for the project. Activate it
with:

```bash
poetry shell
```

This step ensures all Python operations are executed within the
project's environment.

## Running the Django Server

To run the Django server in "soda_web":

1. Make sure you're in the root directory of the project.
2. Execute these commands:

```bash
# Apply database migrations
python manage.py migrate

# Start the Django server
python manage.py runserver
```

The server will start at `http://localhost:8000/`.

## Additional Django Commands

- Creating migrations after model changes:

  ```bash
  python manage.py makemigrations
  ```

- Creating a superuser for the Django admin:

  ```bash
  python manage.py createsuperuser
  ```

  Complete the prompts to set up the superuser.

## Conclusion

You are now set to use the "soda_web" project with Poetry and Django.
For detailed Django documentation, visit [Django's official
site](https://docs.djangoproject.com/en/stable/). For advanced Poetry
usage, see [Poetry's documentation](https://python-poetry.org/docs/).

---

Should you encounter any issues or have queries, please refer to this
project's issue tracker.

Happy coding! 🚀🐍🌐


# flask-tutorial
# reference
https://flask.palletsprojects.com/en/3.0.x/tutorial/

# Project Layout
Create a project directory and enter it:
```shell
$ mkdir flask-tutorial
$ cd flask-tutorial
```

By the end, your project layout will look like this:
```text
/home/user/Projects/flask-tutorial
├── flaskr/
│   ├── __init__.py
│   ├── db.py
│   ├── schema.sql
│   ├── auth.py
│   ├── blog.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── auth/
│   │   │   ├── login.html
│   │   │   └── register.html
│   │   └── blog/
│   │       ├── create.html
│   │       ├── index.html
│   │       └── update.html
│   └── static/
│       └── style.css
├── tests/
│   ├── conftest.py
│   ├── data.sql
│   ├── test_factory.py
│   ├── test_db.py
│   ├── test_auth.py
│   └── test_blog.py
├── .venv/
├── pyproject.toml
└── MANIFEST.in
```

# Installation

## Python Version
We recommend using the latest version of Python. Flask supports Python 3.8 and newer.

## Virtual environments

### Create an environment
Create a project folder and a .venv folder within:
```bash
# macOS/Linux
$ python3 -m venv .venv

# Windows
> py -3 -m venv .venv
```

### Activate the environment
Before you work on your project, activate the corresponding environment:
```shell
# macOS/Linux
$ . .venv/vin/activate

# Windows
> .venv\Scripts\activate
```

### Install Flask
Within the activated environment, use the following command to install Flask:
```shell
$ pip install Flask
```

# Run The Application
```shell
$ flask --app flaskr run --debug
```
pylint mirror
=============

Mirror of pylint package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For pylint: see https://github.com/pycqa/pylint


### Using pylint with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: https://github.com/pre-commit/mirrors-pylint
        rev: ''  # Use the sha / tag you want to point at
        hooks:
        -   id: pylint


Note: this way pylint runs in an isolated Python virtualenv.
If you need pylint to do dynamic analysis of the code
in the app's own Python virtualenv, use it as a
[Repository local hook](https://pre-commit.com/#repository-local-hooks).

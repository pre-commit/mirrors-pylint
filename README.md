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

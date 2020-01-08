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

`pre-commit` runs `pylint` from an isolated virtualenv.  Many
of `pylint`'s checks perform dynamic analysis which will fail there.
You may find configuring `pylint` as a [`local` hook] more useful.

[`local` hook]: https://pre-commit.com/#repository-local-hooks

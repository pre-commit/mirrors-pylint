pylint mirror
=============

Mirror of pylint package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For fixmyjs: see https://bitbucket.org/logilab/pylint/


### Using pylint with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: git://github.com/pre-commit/mirrors-pylint
        sha: ''  # Use the sha / tag you want to point at
        hooks:
        -   id: pylint

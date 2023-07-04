# playground

[![Release](https://img.shields.io/github/v/release/laysa/playground)](https://img.shields.io/github/v/release/laysa/playground)
[![Build status](https://img.shields.io/github/actions/workflow/status/laysa/playground/main.yml?branch=main)](https://github.com/laysa/playground/actions/workflows/main.yml?query=branch%3Amain)
[![codecov](https://codecov.io/gh/laysa/playground/branch/main/graph/badge.svg)](https://codecov.io/gh/laysa/playground)
[![Commit activity](https://img.shields.io/github/commit-activity/m/laysa/playground)](https://img.shields.io/github/commit-activity/m/laysa/playground)
[![License](https://img.shields.io/github/license/laysa/playground)](https://img.shields.io/github/license/laysa/playground)

This is a template repository for Python projects that use Poetry for their dependency management.

- **Github repository**: <https://github.com/laysa/playground/>
- **Documentation** <https://laysa.github.io/playground/>

## Getting started with your project

First, create a repository on GitHub with the same name as this project, and then run the following commands:

``` bash
git init -b main
git add .
git commit -m "init commit"
git remote add origin git@github.com:laysa/playground.git
git push -u origin main
```

Finally, install the environment and the pre-commit hooks with 

```bash
make install
```

You are now ready to start development on your project! The CI/CD
pipeline will be triggered when you open a pull request, merge to main,
or when you create a new release.

To finalize the set-up for publishing to PyPi or Artifactory, see
[here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).
For activating the automatic documentation with MkDocs, see
[here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).

## Releasing a new version

- Add the `ARTIFACTORY_URL`, `ARTIFACTORY_USERNAME`, and `ARTIFACTORY_PASSWORD` to your projects secrets by visiting [this page](https://github.com/laysa/playground/settings/secrets/actions/new).
- Create a [new release](https://github.com/laysa/playground/releases/new) on Github. Create a new tag in the form ``*.*.*``.

For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).

---

Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
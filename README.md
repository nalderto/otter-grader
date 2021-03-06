# Otter-Grader

[![PyPI](https://img.shields.io/pypi/v/otter-grader.svg)](https://pypi.org/project/otter-grader/)
[![Build Status](https://travis-ci.org/ucbds-infra/otter-grader.svg?branch=master)](https://travis-ci.org/ucbds-infra/otter-grader)
[![codecov](https://codecov.io/gh/ucbds-infra/otter-grader/branch/master/graph/badge.svg)](https://codecov.io/gh/ucbds-infra/otter-grader)
[![Documentation Status](https://readthedocs.org/projects/otter-grader/badge/?version=latest)](https://otter-grader.readthedocs.io/en/latest/?badge=latest)
[![Slack](https://img.shields.io/endpoint?logo=slack&url=https%3A%2F%2Fraw.githubusercontent.com%2Fucbds-infra%2Fotter-grader%2Fmaster%2Fslack-shields.json)](https://join.slack.com/t/otter-grader/shared_invite/enQtOTM5MTQ0MzkwMTk0LTBiNWIzZTYxNDA2NDZmM2JkMzcwZjA4YWViNDM4ZTgyNDVhNDgwOTQ0NjNlZjcwNmY5YzJiZjZhZGNhNzc5MjA)

Otter Grader is a light-weight, modular open-source autograder developed by the Data Science Education Program at UC Berkeley. It is designed to work with classes at any scale by abstracting away the autograding internals in a way that is compatible with any instructor's assignment distribution and collection pipeline. Otter supports local grading through parallel Docker containers, grading using the autograder platforms of 3rd party learning management systems (LMSs), the deployment of an Otter-managed grading virtual machine, and a client package that allows students to run public checks on their own machines. Otter is designed to grade Python scripts and Jupyter Notebooks, and is compatible with a few different LMSs, including Canvas and Gradescope.

## Documentation

The documentation for Otter can be found [here](https://otter-grader.rtfd.io).

## Contributing

PRs are welcome! Please submit a PR to the master branch with any updates. Make sure to update the changelog in the docs with any information about the contribution.

To set up the testing environment, install the requirements in `requirements.txt` and run the `test` directory as a module to execute the tests:

```
python3 -m test
```

To run the tests for a specific tool, add the command-line path for that tool to the command. For example, to run the tests for `otter generate autograder`, run

```
python3 -m test generate autograder
```

or to run all tests for commands under `otter generate`, run

```
python3 -m test generate
```

## Changelog

The changelog can be found in the [documentation](https://otter-grader.rtfd.io).

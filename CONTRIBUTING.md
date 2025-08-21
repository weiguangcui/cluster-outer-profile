# Contributing to Cluster Outer Profile Analysis

Welcome! We're excited you want to contribute to this project. This document outlines how you can help.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/cluster-outer-profile.git`
3. Create a new branch: `git checkout -b feature/your-feature-name`
4. Set up the development environment (see README.md)
5. Make your changes
6. Run tests: `pytest`
7. Commit your changes: `git commit -m "Add your message here"`
8. Push to your fork: `git push origin feature/your-feature-name`
9. Open a pull request

## Code Style

- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for Python code
- Use docstrings following the [numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html)
- Keep lines under 88 characters (Black's default)
- Use type hints for function signatures

## Pull Request Process

1. Ensure any install or build dependencies are removed before the end of the layer when doing a build.
2. Update the README.md with details of changes to the interface, this includes new environment variables, exposed ports, useful file locations, and container parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this Pull Request would represent.
4. You may merge the Pull Request once you have the sign-off of two other developers, or if you do not have permission to do that, you may request the second reviewer to merge it for you.

## Data Management

- Large data files should not be committed to the repository
- Use the `data/raw` directory for raw data
- Processed data should be stored in `data/processed`
- Document all data processing steps in the relevant notebook or script

## Code of Conduct

This project adheres to the Contributor Covenant [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

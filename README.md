# Poetry POC

A proof-of-concept Python project using Poetry for dependency management and Apache Spark (`pyspark`) for distributed computing utilities. This project demonstrates a clean setup with pre-commit hooks for code quality and is structured for easy deployment (e.g., to Databricks).

## Features
- **Dependency Management**: Managed with Poetry for reproducible builds.
- **Spark Integration**: Uses `pyspark` for Spark-based functionality.
- **Code Quality**: Enforced with pre-commit hooks (`black`, `flake8`, etc.).
- **Modular Structure**: Source code in `src/` for clean packaging.

## Prerequisites
- **Python**: 3.12+
- **Poetry**: 2.0.0+ (latest version recommended)
- **Git**: For version control
- **Optional**: Databricks cluster (if deploying)

## Installation

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd poetry_poc

## Setup

1. **Clone the Repo**:
   ```bash
   git clone <repository-url>
   cd poetry_poc

2. **Install Poetry**:
   ```bash
   pip install poetry

3. **Install Dependencies**:
    ```bash
    poetry install

4. **Activate Virtualenv**:
    ```bash
    source "$(poetry env activate)"

## Usage:
### Running Locally:
- Execute the main script:

    ```bash
    poetry run python src/main.py

### Building the Package
- Generate distributable files (.tar.gz and .whl):

    ```bash
    poetry build


## Code Quality
Pre-commit hooks run automatically on `git commit`  to:

- Format code with black.
- Lint with flake8.
- Validate pyproject.toml with poetry check.

### Install hooks:
    poetry run pre-commit install

### Run manually on all files:
    poetry run pre-commit run --all-files

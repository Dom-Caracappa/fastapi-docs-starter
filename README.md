# FastAPI Docs Starter

This project is a practice environment to learn API documentation with FastAPI and Sphinx.

![Python](https://img.shields.io/badge/python-3.13-blue)
![License](https://img.shields.io/github/license/Dom-Caracappa/fastapi-docs-starter)
[![Documentation Status](https://img.shields.io/badge/docs-latest-brightgreen)](https://dom-caracappa.github.io/fastapi-docs-starter/)

## About

- **Framework**: FastAPI
- **Documentation**: Sphinx + reStructuredText (with Alabaster and Furo themes)
- **Features**:
  - REST API endpoints: `/`, `/info`, `/health`, `/echo`, `/fact`, `/math-fact`
  - Dynamic API docs built with Sphinx
  - Hosted on GitHub Pages

## Getting Started

1. Clone the repo:
    ```bash
    git clone https://github.com/Dom-Caracappa/fastapi-docs-starter.git
    cd fastapi-docs-starter
    ```

2. Create a virtual environment:
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # or `.venv\Scripts\activate` on Windows
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the FastAPI app:
    ```bash
    uvicorn app.main:app --reload
    ```

5. Build the docs:
    ```bash
    cd docs
    make clean && make html
    cd ..
    ghp-import -n -p -f docs/build/html
    ```

## Live Docs

[View the API Documentation](https://dom-caracappa.github.io/fastapi-docs-starter/)



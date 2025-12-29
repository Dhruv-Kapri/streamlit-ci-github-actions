# streamlit-ci-github-actions

A minimal Streamlit project with **CI using GitHub Actions**, focused on
testing, reproducibility, and clean automation.

<!-- --- -->

## Project Structure

  ```
  .
  ├── app.py                # Streamlit application
  ├── _test.py              # Pytest test cases
  ├── requirements.txt      # Python dependencies
  ├── README.md
  ├── LICENSE
  └── CI-Notes.pdf          # Notes (optional / local reference)
  ```

<!-- --- -->

## Getting Started

1. Create virtual environment
  ```bash
  python3 -m venv .venv
  source .venv/bin/activate
  ```

2. Install dependencies
  ```bash
  pip install -r requirements.txt
  ```

3. Run Streamlit app
  ```bash
  streamlit run app.py
  ```

> Running Tests
Tests are written using pytest.
  ```bash
  pytest _test.py
  ```

<!-- --- -->

## CI with GitHub Actions

This project uses GitHub Actions to automatically:
- Install dependencies
- Run pytest on every push and pull request to main

Workflow file: `.github/workflows/ci.yml`

<!-- --- -->

## Purpose of This Project
- Learn CI/CD basics
- Understand GitHub Actions
- Validate Streamlit apps with automated testing
- Keep workflows simple and production-aligned

<!-- --- -->
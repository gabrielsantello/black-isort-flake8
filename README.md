# Python Code Formatting and Style Guide

## Introduction
This README provides guidelines for maintaining clean and consistent Python code. Following these best practices ensures readability, maintainability, and adherence to the PEP 8 style guide. We'll cover the following tools:

1. **PEP 8**: The official Python Enhancement Proposal that defines the coding conventions for the Python standard library.
2. **Black**: An uncompromising code formatter that automatically formats your Python code to follow PEP 8 guidelines.
3. **isort**: A tool for sorting Python imports in a consistent and organized manner.
4. **flake8**: A code linting tool that checks your code against PEP 8 and identifies potential issues.

## Table of Contents
1. [PEP 8 Best Practices](#pep-8-best-practices)
2. [Using Black](#using-black)
3. [Sorting Imports with isort](#sorting-imports-with-isort)
4. [Code Linting with flake8](#code-linting-with-flake8)
5. [Setting Up Pre-commit Hooks](#setting-up-pre-commit-hooks)

---

## 1. PEP 8 Best Practices
PEP 8 provides guidelines for writing clean and readable Python code. Some key practices include:

- Limit lines to 88 characters (instead of the older 79-character limit).
- Use double quotes for strings.
- Use consistent indentation (usually 4 spaces).
- Follow naming conventions for variables, functions, and classes.

## 2. Using Black
Black is an opinionated code formatter that automatically reformats your Python code to adhere to PEP 8. To use Black:

1. Install Black:
   ```
   pip install black
   ```

2. Format your code:
   ```
   black my_file.py
   ```

## 3. Sorting Imports with isort
isort organizes your import statements according to PEP 8 guidelines. To use isort:

1. Install isort:
   ```
   pip install isort
   ```

2. Sort your imports:
   ```
   isort my_file.py
   ```

## 4. Code Linting with flake8
flake8 checks your code for style violations, errors, and potential bugs. To use flake8:

1. Install flake8:
   ```
   pip install flake8
   ```

2. Run flake8 on your code:
   ```
   flake8 my_file.py
   ```

## 5. Setting Up Pre-commit Hooks (pre-commit.com/hooks.html) - use "bandit", "flake8", "black", "isort"
Pre-commit hooks allow you to run checks automatically before each commit. Here's how to set up a pre-commit hook for your project:

1. Install the `pre-commit` package:
   ```
   pip install pre-commit
   ```

2. Create a `.pre-commit-config.yaml` file in your project directory with the following content:

   ```yaml
   - repo: https://github.com/pre-commit/mirrors-black
     rev: v21.12b0
     hooks:
       - id: black

   - repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.3
     hooks:
       - id: isort

   - repo: https://github.com/pre-commit/mirrors-flake8
     rev: v4.1.1
     hooks:
       - id: flake8
   ```

3. Run the following command to install the pre-commit hooks:
   ```
   pre-commit install
   ```

4. Now, every time you commit changes, the pre-commit hooks will automatically format your code, sort imports, and check for style violations.
---

Happy coding! 🚀🐍

Source:
(1) How to use black, flake8, and isort to format Python codes - Amir .... http://www.sefidian.com/2021/08/03/how-to-use-black-flake8-and-isort-to-format-python-codes/.
(2) Keeping python code clean with pre-commit hooks: black, flake8 and isort. https://medium.com/staqu-dev-logs/keeping-python-code-clean-with-pre-commit-hooks-black-flake8-and-isort-cac8b01e0ea1.
(3) Ensuring PEP 8 Compliance: Tools for Automating Adherence to ... - Medium. https://medium.com/@kartheekgottipati/ensuring-pep-8-compliance-tools-for-automating-adherence-to-coding-standards-5a6cc2f48519.
(4) How to Make your Code Shine with GitLab CI Pipelines | Semantix - Medium. https://medium.com/semantixbr/how-to-make-your-code-shine-with-gitlab-ci-pipelines-48ade99192d1.
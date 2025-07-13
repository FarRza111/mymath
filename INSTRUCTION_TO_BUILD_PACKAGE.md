# mymath

A simple Python package that provides a basic `add(a, b)` function.

---

## Overview

This document explains the full process of how the `mymath` package was created, published to GitHub, and how your team can easily install and use it.

---

## Step 1: Create the Package Locally

``` python
### Project Structure
mymath/
├── mymath/
│ └── init.py
├── pyproject.toml
├── README.md
└── .gitignore
```


### Write the Function

In mymath/__init__.py:
```python
def add(a, b):
    return a + b
```


### pyproject.toml
```python
[project]
name = "mymath"
version = "0.1.0"
description = "A simple math utility package"
authors = [{ name = "Your Name", email = "you@example.com" }]
readme = "README.md"
license = { text = "MIT" }
requires-python = ">=3.7"

[build-system]
requires = ["setuptools>=61.0"]
build-backend = "setuptools.build_meta"

[tool.setuptools.packages.find]
where = ["."]
```


### gitignore
    __pycache__/
    *.pyc
    dist/
    .venv/


### Step 3: Install the Package
    
    team can install the package directly from GitHub using SSH:
    SSH
    
    pip install git+ssh://git@github.com/FarRza111/mymath.git
    
    OR 
    
    HTTPS
    
    pip install git+https://github.com/FarRza111/mymath.git

### Optionally, tag new versions:
    
    git tag v0.2.0
    git push origin v0.2.0

### install specific version
``` python
pip install git+https://github.com/FarRza111/mymath.git@v0.2.0
```



# Jupyter Notebook Skeleton Template

## Summary
---

This project was created to simplify my setup process for data projects using Python, Pipx, and Poetry. Setting up a consistent environment for data analysis and experimentation can be time-consuming. This template aims to streamline my process by providing a standardized project structure and instructions to quickly get started with Jupyter Notebooks and essential libraries.

## Prerequisites
---

### Python

Python is an interpreted, object-oriented, high-level programming language with dynamic semantics. Its high-level built in data structures, combined with dynamic typing and dynamic binding, make it very attractive for Rapid Application Development, as well as for use as a scripting or glue language to connect existing components together.

You can download it from [python.org](https://www.python.org/)

### Pipx

Pipx is a tool to install and run any of these thousands of application-containing packages in a safe, convenient, and reliable way. In a way, it turns Python Package Index (PyPI) into a big app store for Python applications. Not all Python packages have entry points, but many do.

You can learn more about it [here](https://pypa.github.io/pipx/)

### Poetry

Poetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you. Poetry offers a lockfile to ensure repeatable installs, and can build your project for distribution.

You can read more about it [here](https://python-poetry.org/)

## Getting Started
---

To get started with this Skeleton Template, follow these steps:

0. Install Jupyter Notebook using Pipx

`pipx install jupyter==7.0.0b2 --include-deps`

1. Create new Python project with Poetry

```shell
mkdir jupyter-project-skeleton && cd jupyter-project-skeleton
mkdir jupyter_project_skeleton
mkdir notebooks
mkdir data
`poetry init -n`
```

2. Install and register a new ipykernel

```shell
poetry add ipykernel
poetry run python -m ipykernel install --user --name jupyter_project_skeleton
jupyter kernelspec list
```

3. To install the defined dependencies

```shell
poetry add pandas matplotlib scikit-learn
poetry add black -G dev
```
4. Launch a Jupyter Notebook

`jupyter notebook`


### Usage
---

Keep the project structure organized to maintain clarity and consistency across your data projects.

- Use the `notebooks` directory to create notebooks for your data analysis tasks. You can organize your notebooks by creating subdirectories if needed.
- Store your datasets and data files in the `data` directory. This keeps your data organized and accessible from your notebooks.


### Version
---

v0.0.1

### Coming Soon

- [ ] Add a sample project with a in the jupyter_project_skeleton folder.
- [ ] Create a sample Jupyter Notebook in `notebooks` folder, that consumes dummy data in csv format located in `data` folder.

# SQA-Assignment

**Table of Content**:
1. [Introduction](https://github.com/Harmos274/SQA-Assignment#introduction)
2. [Task Estimation in Scrum](https://github.com/Harmos274/SQA-Assignment#task-estimation-in-scrum)
3. [Coding Standards](https://github.com/Harmos274/SQA-Assignment#coding-standards)
4. [Code Reviews](https://github.com/Harmos274/SQA-Assignment#code-reviews)

## Introduction

## Task Estimation in Scrum

## Coding Standards

### General Knowledge

#### Solid Principles

In this company we believe in SOLID principles, because our softwares needs to be reliable on the long term, we need to make them easily maintainable.

SOLID stands for:
- **S**ingle Responsability
- **O**pen/Closed Principle
- **L**iskov Substitution
- **I**nterface Segregation Principle
- **D**ependency Injection

This is a set of rules created to build better scalable softwares.
Concisely, you need to ensure that every atomic element of your code serves only one purpose. The best thing to do is asking to yourself what is the purpose of what your coding, if it's "this ***and*** that" then you need to split your component in two. You also need to change the least possible the code already done, and work by extending it instead of rewriting it.

Keep in mind that all the principles are purely **good practices** and sometimes you'll need to transgress them because the situation needs it.

Read [that article](https://stackify.com/solid-design-principles/) to learn more about SOLID principles.

#### Testing practices

### Python 3

#### Project Structure

To prevent a certain lack of consistency between projects every Python 3 projects needs to follow a specific file structure.

For example if you're developing on a project named `sample` you'll see that kind of file structure:

```
Makefile
README.md
LICENSE
setup.py
requirements.txt
sample/__init__.py
sample/core.py
sample/helpers.py
docs/conf.py
docs/index.rst
tests/test_basic.py
tests/test_advanced.py
```

As you can see the `sample/` folder is where the actual business code of the project is. There's also a `test/` folder where you can put your tests.
The `requirements.txt` file is a `pip` requirement file where all the packages needed to run the program are specified using the [pip format](https://pip.pypa.io/en/stable/reference/requirements-file-format/#example).

To know more on this structure you can read [this article](https://docs.python-guide.org/writing/structure/), it also includes some architecture advice.

#### PEP8 

#### Unit Testing

## Code Reviews


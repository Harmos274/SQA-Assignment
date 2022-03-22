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

#### Testing practices

### Python 3

#### Project Structure

#### PEP8 

#### Unit Testing with Pytest

In order to apply a quality assurance policy, the company has chosen Pytest to run unit tests.
Pytest is an external testing module for python. It is more intuitive and easier to use than the built in Python 3 testing module.
You can organize your tests in classes, this allow you to respect the separation of concern practice.
This module gives the developers a simple way to test their code when unexpected things happen.

>Testing that your program responds as expected in negative situations is very important.

Pytest is pretty easy to use, because it provides developers an API to test functions:

    def inc(x):
        return x + 1


    def test_answer():
        assert inc(3) == 5

Pytest would answer:

    ______________________________test_answer_______________________________

        def test_answer():
    >       assert inc(3) == 5
    E       assert 4 == 5
    E        +  where 4 = inc(3)

    test_sample.py:6: AssertionError
    ========================short test summary info=========================
    FAILED test_sample.py::test_answer - assert 4 == 5
    ===========================1 failed in 0.12s============================


Pytest allows developers to use mocks, in order to imitate modules that we do not want to test, because we consider them external to our code. For example, you can mock HTTP responses to test your program in a lot of different situations.

You can get a full guide of Pytest by reading this [article](https://medium.com/worldsensing-techblog/tips-and-tricks-for-unit-tests-b35af5ba79b1).

## Code Reviews


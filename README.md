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

#### PEP8 

On Python 3 we choose to follow the [PEP8](https://realpython.com/python-pep8/) set of rules, which are the most classics rules in Python that almost everybody follows. Here are some basic keypoints:

- Function names are in `snake_case` and are named with verb
- Variable names are in `snake_case` and are named with word or a single letter
- Classes are in `PascalCase` and their methods in `snake_case`
- Constants are in `SCREAMING_SNAKE_CASE` and are named with full words
- Module names are in `snake_case`
- Package names are named in `lowercase` with no space or separation between words
- Use 4 consecutive spaces for each level of indentation

Note that **we don't use the 80 characters limit per line**, you need to be concise but no needs to break your line at weird places to stay in your character limit.

If you want to practice a bit how to write good python code you can follow [this courses](https://openclassrooms.com/en/courses/6900866-write-maintainable-python-code) on OpenClassrooms which will introduce you to PEP8 and also teach you some useful design patterns.

#### Unit Testing

## Code Reviews


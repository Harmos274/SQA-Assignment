# SQA-Assignment

**Table of Content**:
1. [Introduction](https://github.com/Harmos274/SQA-Assignment#introduction)
2. [Task Estimation in Scrum](https://github.com/Harmos274/SQA-Assignment#task-estimation-in-scrum)
3. [Coding Standards](https://github.com/Harmos274/SQA-Assignment#coding-standards)
4. [Code Reviews](https://github.com/Harmos274/SQA-Assignment#code-reviews)

## Introduction

This document is a handbook describing all the best practices you need to know when you are developing four our company.
In it you'll find how to estimate your task when you're using SCRUM, what are our code standards and advices and finally how to do efficient code reviews.

Every section begins with a selection of keypoints that summarizes its content if you need a quick remembering.

## Task Estimation in Scrum

### Introduction

The task estimation is a very important part of the SCRUM process for different reasons:

> Estimates allow us to predict when a Sprint Goal will be met, and therefore when a substantial increment of value will be delivered

>Our estimates help our stakeholders plan ahead. They are part of the value we provide

>Estimates help us to de-risk scope of uncertain size and complexity

>Estimated work can be traded in and out of scope for other work of similar size. Without estimates you can't trade

>The very process of estimation adds value. When we estimate we discuss requirements in more detail, and gain a better understanding of what is needed

You can find a complete discussion of the **pros and cons** we should estimate tasks in SCRUM [here](https://dzone.com/articles/agile-estimation-practice). Notice that in this article are presented several methods of estimation, but in the section below, you will be explained the **fibonacci** method of task estimation.

### How to estimate tasks ?

To estimate task according to SCRUM framework, you should focus on the **amount of effort** that will be required to achiev the task. Furthermore, as it is universally accepted that the more complex a task is, the hardest it become to estimate it.  
Though we will always **estimate** the **size** of a task, by opposition to its expected **duration**.  

While there are many methods to achieve this purpose, we use **Fibonacci scale** using the **First Story as benchmark.**   

If you are interested in understanding deeply the pros and the cons of this method, as well as some few other methods, we invite you to take a close look to [this article](https://medium.com/serious-scrum/best-way-to-estimate-effort-using-story-point-in-sprint-planning-f43ad2d6fa91) since we will only cover outlines just below.

Fibonacci scale is based on **Fibonacci sequence**. It consists of numbers that each number is the sum of the two preceding ones, starting from 0 and 1. The beginning of the sequence start as below :

> 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...

...and goes to the infinite.

In Fibonacci scale, each member estimate the complexity of the task only numbers from fibonacci sequence and present it to the rest of the group. It will leads to a **discussion** until all the team come to a consensus.

And that's it ! Pretty simple, isn't it ?

However we expect **every team members** to pay attention **carrefuly** the two rules elements below.

#### The importance of discussion  

Task estimation is achieved with the **whole team**. As mentionned on the aboved mentionned article:
> _"it is not surprising to see different even contradictory views on how effort should be estimated"_  
> 
Thus you should always remember that the research of a consensus through **discussion is an integral part of the job, if not the essence of it**. You will find in the next section some common errors to avoid to find a consensus efficiently, and peacefully.

_N.B. : The voice of a newcomer worth as much as the other voice. Hence a proper enboarding is very important_  
  
#### Forget the _duration_ and focus on  the _size_ of a task
By estimating a task in SCRUM, we try to capture its complexity through the amount of effort we expect that will be needed.  
Thus, despite it can be a great temptation to make a parallel with the amount of time you expect to work on a task. By estimating, you also want to **estimate the risk** the task consume a lot of time.
This subject has been discussed many time on the internet, so that I invite you to browse by yourself on the internet. Stackoverflow threads such as [this one](https://softwareengineering.stackexchange.com/questions/216796/how-to-estimate-tasks-in-scrum) will help you to understand the purpose of this statement more accurately.

#### Most Common Errors

Here you can find two articles treating the easy mistakes you can make while estimating tasks in SCRUM: [12 Common Errors Made When Using Story Points]() and [Do & Don’t - Sprint Backlog Estimation](). Those posts are really interesting and explain the major issues in using story points, during the estimation but also during the rest of the sprint.

However, some mistakes seem **occur frequently**:

#### Don’t Compare Story Points With Hours

The effort estimation is **relative** between each developer, story points allow developers who work at different speeds to **estimate effort together**. By translating it into hours, you lose the main reason to use story points.

#### Averaging Story Points

During the estimation process, if half of the team says 2, and the second half says 5, it is a **mistake** to average story point at 3. Task estimation trend to **lower the risk** of unknown size or complexity of product backlog items. If a huge difference in estimation happens, it frequently attests of **hidden complexity** or **misunderstanding** of the task. You also will lose an opportunity for an interesting discussion.

![Discuss](./assets/task_estimation_discuss.png)

To avoid the averaging of story points, it is recommended to **discuss and estimate again** to use the process explained by the image above.

#### Conforming to the Expert in the Room

While estimating the tasks, it is highly likely that every member of the team would **conform with the expert** of the group. To avoid it, it is recommended to let the expert **explain his view of the task**, and then proceed to the estimation **without the expert**.

As story points do not take part in the **SCRUM guide**, a lot of teams have different opinions about them. Knowing things not to do will help you to exploit **the power of story points**.

## Coding Standards

- Follow as much as possible the SOLID Principles
- Test your code with Pytest
- You tests need to be fast, simple and readable
- Follow the requested project structure
- Follow the PEP8 directives as much as possible, **except the 80 columns restriction**

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

Unit tests allow the developer to be sure that an extract of code works. It consists of small tests making sure small parts of code operate well.

>Unit tests help you find and fix bugs earlier.

>Your suite of unit tests becomes a safety net for developers.

>Unit tests can contribute to higher code quality.

>Unit tests might contribute to better application architecture.

>Unit tests can act as documentation.

>Detect code smells in your codebase.

Unit Tests Role In A QA Strategy, and it is one of the best ways to get constant feedback on your code. It is additional with other types of code, being part of the practical test pyramid, but is the testing section performed by developers.

![Tests Pyramide](./assets/coding_standards-pyramide.png)

Tests should be fast, simple and readable, but should not repeat logical implementation of code.
If you want a complete discussion on unit testing, and a list of useful good practices, please read [this](https://www.testim.io/blog/unit-testing-best-practices/).

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

#### Unit Testing with Pytest

In order to apply a quality assurance policy, the company has chosen Pytest to run unit tests.
Pytest is an external testing module for python. It is more intuitive and easier to use than the built in Python 3 testing module.
You can organize your tests in classes, this allow you to respect the separation of concern practice.
This module gives the developers a simple way to test their code when unexpected things happen.

>Testing that your program responds as expected in negative situations is very important.

Pytest is pretty easy to use, because it provides developers an API to test functions:

```python
def inc(x):
    return x + 1


def test_answer():
    assert inc(3) == 5
```

Pytest would answer:

```
______________________________test_answer_______________________________

    def test_answer():
>       assert inc(3) == 5
E       assert 4 == 5
E        +  where 4 = inc(3)

test_sample.py:6: AssertionError
========================short test summary info=========================
FAILED test_sample.py::test_answer - assert 4 == 5
===========================1 failed in 0.12s============================
```


Pytest allows developers to use mocks, in order to imitate modules that we do not want to test, because we consider them external to our code. For example, you can mock HTTP responses to test your program in a lot of different situations.

You can get a full guide of Pytest by reading this [article](https://medium.com/worldsensing-techblog/tips-and-tricks-for-unit-tests-b35af5ba79b1).

## Code Reviews

- Be humble  
- Be concise  
- Be available  
- Be proactive  

### Introduction

In this section we will address the **code reviews** process in the company. Indeed, as a developper you will be submiting some new code or modifications to the code base.  

> How to ensure that your contribution participate in improving the codebase ?  

> How to reduce the number of issues added (often unintentionally) to the code base ?  

> How to ensure that the code added to the code base do what it is intended for ?

These are only few questions among the many ones that a team wants to be answered **before** some code to be added to the code base. At the same time, it allows developpers to **exchange** about their respective experience.

That is the reason why you will be having peer code reviews, as reviewed coder as well as reviewer.  

To make sure these reviews will be valuable for you, people you will be reviewing and the team, in this section, we will give you some **advices** on "how to make a good code reviews ?" and present you the **most common mistakes**.

### How to make a code review ?

They are two situations in a code review. The first one, you are the author of the code. When your submitting something to review you need to follow those quick instructions:

- Run the tests and linters **before** submitting your Pull Request, it may seems basic but a lot of people only rely on the CI to do it for them
- Be **available**, the reviewer may need more explanation from you on some parts of the code, don't forget that the review in bidirectional, it's more like a conversation than an evaluation
- Be **humble**, nobody is against you, again it's a process of cooperation. It's totally normal if your so called *perfect code* needs some rewrite on some part, **never takes it personally**
- Try to find a good name and description for your Pull Request, avoid unprecize titles and not requests without description, sometimes you won't be sure about your solution to a problem don't hesitate to say it in the PR's description, because it will guide your reviewers during their work

Finally the second one, you are the reviewer (or a part of the reviewers assigned on the Pull Request), you need to follow those instructions:

- Don't limit your review to what you see in the GitHub diffs and pull the branch locally to see the modifications
- Respect people's time and don't review the PR too long after the submission, how long will depends on how much the project is actively maintained
- Try to be as precise and constructive as possible and **don't hesitate to ask the author** about things you're not sure you're understanding
- Follow a checklist (you can see more about a good Python 3 code review's checklist [here](https://deepsource.io/blog/python-code-review-checklist/))
- Take your time, **the more you work on it, the less you'll see the flaws**. Avoid passing more than 1 hour at a time and try to not review more than 400 lines of code per session
- Be **humble** too, sometimes your change request may not be a good solutions to the problem, remember that nobody is flawless and it's ok. You need to see the code review as a team work and not an evaluation
- Always try to see how the submitted code will **evolve in the future**, remember why a short-term solution is called like that

Read more about the code review process in those 3 articles:
- [Best Practices for Reviewing Pull Requests in GitHub](https://www.backhub.co/blog/best-practices-reviewing-pull-requests-github)
- [How to do a code review](https://google.github.io/eng-practices/review/reviewer/)
- [Best Practices for Code Review](https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/)

### Most common errors

We will address **4 common errors** that we already encountered during code reviews. Those could have been avoided by following some good practices. You will find [here](https://www.backhub.co/blog/best-practices-reviewing-pull-requests-github) and [here](https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/) two articles which you can use as guides when you're reviewing code.

#### Do NOT let the code cool down

If one of your colleague asks you to review their work. He will be certainly waiting for your review for the next few minutes and then will switch to something else. Thus, when you will do the review, maybe few hours later, he will have to switch back to his previous work which could have an **extra switching cost** for him. Moreover, he could have forgotten some aspect of his code and he'll need to remind them before treating your feedbacks.

#### Provide a constructive feedback

What is worse than receiving negative and inaccurate feedback such as :

 > WTF did you do ? Why don't you use only X instead?!

We engage you to use as much as possible affirmative form, using sentences begining with :

> "I would suggest you to..."

or

> "I am suprised by... I would rather use..."

At the same time, do not hesitate to share any kind of positive feeling you could have when you're reviewing the code. Congratulation are always welcome !

#### Keep your ego out

This is probably one of the most common mistake. If you find yourself in a position where you are reviewing someone who is senior to you, **NEVER** assume that you have nothing to learn from him. To the contrary, always assume that this person can teach you something that you don't know yet. Especially if your are facing a very young developer (such as an intern), they are more enclined than to find unexpected solutions.
They succeed in crossing the crocodile river swimming since no one told them that it was impossible.

#### Never assume that the code will run

A very common mistake is to review a code, assuming that the code you are reviewing is working as intended. **ALWAYS** run the code on your own to check that everything works as expected. The last thing you want is to face an emergency while production is broken due to a piece of code you reviewed.

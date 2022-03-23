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

## Coding Standards

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

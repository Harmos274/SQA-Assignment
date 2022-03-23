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

### Introduction

In this section we will address the **code reviews** process in the company. Indeed, as a developper you will be submiting some new code or modifications to the code base.  

> How to ensure that your contribution participate in improving the codebase ?  

> How to reduce the number of issues added (often unintentionally) to the code base ?  

> How to ensure that the code added to the code base do what it is intended for ?

These are only few questions among the many ones that a team wants to be answered **before** some code to be added to the code base. At the same time, it allows developpers to **exchange** about their respective experience.

That is the reason why you will be having peer code reviews, as reviewed coder as well as reviewer.  

To make sure these reviews will be valuable for you , people you will be reviewing and the team, in this section, we will give you some **advices** on "how to make a good code reviews ?" and present you the **most common mistakes**.

### How to make a code review ?

### Most common errors

We will address **4 common errors** that are already encountered while doing a code review. These can be avoid by following good practices. You will find [here](https://www.backhub.co/blog/best-practices-reviewing-pull-requests-github) and [here](https://smartbear.com/learn/code-review/best-practices-for-peer-code-review/) an article which you could use as a guide for your code reviews.

#### Do NOT let the code cool down

If one of your colleague ask you to review its work. He will be certainly waiting for your review in the next minutes and then will switch to something else. Thus when you will do the review, maybe few hours later he will have to switch back to his previous work which will have an **extra switching cost** for him. Moreover, he could have forget some aspect of his code he will have to remind in order to fix its code.

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

A very common mistake is to review a code, assuming that the code you are reviewing is working as intended. **ALWAYS** run the code on your own to check everything works as expected. The last thing you want is to face an emergency while production is broken due to a piece of code you reviewed.

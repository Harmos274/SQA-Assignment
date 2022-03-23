# SQA-Assignment

**Table of Content**:
1. [Introduction](https://github.com/Harmos274/SQA-Assignment#introduction)
2. [Task Estimation in Scrum](https://github.com/Harmos274/SQA-Assignment#task-estimation-in-scrum)
3. [Coding Standards](https://github.com/Harmos274/SQA-Assignment#coding-standards)
4. [Code Reviews](https://github.com/Harmos274/SQA-Assignment#code-reviews)

## Introduction

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

## Code Reviews


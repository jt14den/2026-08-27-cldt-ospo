---
title: UC OSPO Licensing CLDT - Day 1 Notes
tags: CollabLesson, Notes, UC-OSPO-Network, Licensing, Day1
description: Day 1 (Thursday) collaborative notes content, scoped to match slide deck 1.
---

## Day 1 - Live Content (Thu 8/27)

### Introduction

#### Overview
##### Objectives
After completing this episode, participants should be able to...
- Explain how trainers and participants will interact throughout the workshop.
- Summarise the main skills that will be taught in this workshop.

##### Questions
- What is covered in this training?
- Who are the trainers?
- Who is participating?

#### Code of Conduct
[The Carpentries Code of Conduct](https://docs.carpentries.org/policies/coc/)


#### CodiMD
- Edit/Split/View Modes
- Write in Markdown - click the '?' button in the top bar for a quick Markdown reference sheet.

::: success
#### Our First Exercise (10 minutes)
Think of an example of a great lesson that you have followed (were taught in a class, read through online, read in a book).
What did you find was so good about it? 
Why did it make such an impression on you?
Try to differentiate between **what was good about the performance** of the teacher/trainer and **what was good about the content** of the lesson itself.
Take a few minutes to write down some notes about your answer, then introduce yourself to the other participants and tell them about it.
:::

We will focus on three main areas:

* Designing a lesson
* Building a lesson website
* Collaborating effectively

#### Instructor Training
[The Carpentries Instructor Training](https://carpentries.github.io/instructor-training/)

#### Key Points
- This training aims to teach you a process for designing a lesson and the skills to develop it as an open source website, in collaboration with others.


---

### Lesson Design

#### Overview
##### Objectives
After completing this episode, participants should be able to...
- Explain the lesson design process we will be adopting for this course.
- Summarise the lessons that participants will be working on.

##### Questions
- What are the recommended steps to take when developing a new lesson?
- What lesson do you want to develop during and after this workshop?


#### The Lesson Design Process We Will Use
![An overview of the iterative process of lesson design and development 
, adapted from Nicholl's five phases,
that will be presented in this training.
](https://carpentries.github.io/lesson-development-training/fig/cldt-design-process.svg)

1. Define desired learning outcomes.
2. Design assessments to determine progress towards desired outcomes.
3. Write content to lead learners from one of these assessments to the next.
4. Assess learner progress towards outcomes during teaching.
5. Evaluate how closely the outcomes meet the objectives.

::: success
#### Discussion (10 minutes)
Share your answers to the following questions in the shared notes, then discuss them with the Trainers, your collaborators, and the other participants.

1. What is the topic of the lesson that you plan to develop based on this training?
2. Have you created training material on this topic before?
3. What is motivating you to create this lesson?
:::


#### Iterative Development
![Diagram of the life cycle of a lesson in The Carpentries ecosystem. 
A lesson is proposed at the beginning of the pre-alpha stage. 
It enters alpha when it is taught for the first time. 
In beta, it is taught by other instructors. 
A full release of the lesson is made when it is stable.
Pilot workshops take place during the alpha and beta phases.](https://carpentries.github.io/lesson-development-training/fig/life_cycle.png)

- `pre-alpha`: first draft of lesson is being created
- `alpha`: lesson is being taught by authors
- `beta`: lesson is ready to be taught by other instructors
- `stable`: lesson has been tested by other instructors and improved based on feedback. Major changes and updates are relatively infrequent.

#### Lesson Developer Handbook
[More information about the lesson life cycle](https://docs.carpentries.org/resources/curriculum/lesson-life-cycle.html) is available in the community handbook. That site also contains the [Lesson Developer Handbook](https://docs.carpentries.org/handbooks/lesson_developers.html), which collects a lot of resources and guidance for Carpentries community members interested in curriculum development.

#### Key Points
- We will learn to develop lessons based on the (slightly adapted) Nicholl's backward lesson design  process.
- There can be many reasons to create a new lesson.
- This training will give you a process to follow to ensure your lesson is effective.


---

### Identifying Your Target Audience

#### Overview
##### Objectives
After completing this episode, participants should be able to...
- Describe the importance of aligning lesson design with the intended audience.
- Compose a list of prior knowledge required to follow a lesson.

##### Questions
- Why is it so important to think about the target audience early in the process?
- How can you ensure that your lesson reaches the right audience?


#### Two Important Characteristics of a Target Audience

* Expertise
* Motivation

::: info
#### Lesson Design Notes
We will now create documents to capture your decisions, drafted content etc as you begin designing your new lesson. Use the template below to create this document.

Make a copy of [the Lesson Design Notes template](https://codimd.carpentries.org/HPwUE3FnTeSQJ9-_5EfU7Q?view#).

The content you draft there will be transferred into a new lesson website later in this first part of the training.
:::


::: success
#### Exercise: thinking about target audience (15 minutes total for both parts)

##### Part 1 (all, 5 minutes)
Think about a member of the target audience for your lesson, and answer the following questions in the context of your lesson topic:
1. What is their background?
2. What do they already know how to do?
3. What do they want to do with the skills they will learn from your lesson?
4. What problem will your lesson help them solve?

##### Part 2a (for groups collaborating on the same lesson, 10 minutes)
Share your answers with your collaborators. 
How do they compare?
If you have identified different audiences, are they compatible?
Or would your time be better spent focussing on one particular audience for this lesson?

Take notes on your discussion in your Lesson Design Notes document. 
It can be particularly helpful to note down any decisions made e.g. potential target audiences that were explicitly discounted, and your reasons for doing so.

##### Part 2b (for participants developing their lessons alone, 10 minutes)
Take notes about your choice of target audience in your Lesson Design Notes document. It can be particularly helpful to note down any decisions made e.g. potential target audiences that were explicitly discounted, and your reasons for doing so.

Then write 1-2 diagnostic questions, for use before the lesson is taught,
to help you assess whether a respondent falls within the intended audience for your lesson.
:::

::: success
#### Exercise: Defining Prerequisite Knowledge (5 minutes)
Write a list of the skills/knowledge your learners will be required to have before they can follow your lesson. Add this list to the 'Target Audience' section of your Lesson Design Notes document.

If you are struggling with this exercise because your lesson audience is novices, think about skills like touch typing, using a web browser, or interacting with a command line or graphical interface. These are skills commonly overlooked by experts and competent practitioners.
:::


#### Key Points
- We recommend an iterative lesson design process that begins with identifying the target audience, before defining learning outcomes, then creating assessments, writing explanatory content, and evaluating the lesson in a workshop.
- Thinking about the target audience early in the design process helps to ensure that your lesson is built around the needs and motivations of real people.
- Use the description of your target audience to help attract people with the appropriate interests and prior knowledge to your lesson.


---

### Defining Lesson Objectives/Outcomes

#### Objectives
After completing this episode, participants should be able to...
- Explain the importance of defining specific, measurable, attainable, relevant and time-bound objectives for a lesson.
- Evaluate a written lesson objective according to these criteria.

#### Questions
- How can describing the things you intend to teach aid the process of writing a lesson?
- How can you be specific and realistic about what you will teach in your lesson?
- What are some of the risks associated with unrealistic or undefined expectations of a lesson?

![We have reached step 1 in our iterative development cycle: define desired learning outcomes.](https://carpentries.github.io/lesson-development-training/fig/cldt-step-1.svg)

#### Bloom's Taxonomy
A popular aid for defining learning objectives, providing a bank of action verbs to use when drafting them.

![Bloom's taxonomy - a framework for categorising educational goals, image from Wikimedia Commons reused under CC BY 4.0 license](https://upload.wikimedia.org/wikipedia/commons/6/6a/Bloom%27s_revised_taxonomy.svg)

A version of Bloom's containing verbs more closely related to computing skills: https://ccecc.acm.org/assessment/blooms-for-computing

#### What does an objective look like?
![An example learning objective, "import data into an indexed DataFrame with read_csv", with emphasis placed on the action verb ("import") and the specificity ("indexed") of the objective.](https://carpentries.github.io/lesson-development-training/fig/objective.svg)

That example is code-specific. For a conceptual lesson like ours, the same pattern (action verb + specificity) looks like:

> **explain** why a GPL-3.0-licensed dependency cannot be bundled into closed-source software

Same shape, no code: a precise verb ("explain," not "understand") plus a specific, observable scenario.

#### SMART Objectives Should Be...
* **Specific**: they should clearly describe a particular skill or ability the learner should have.
* **Measurable**: it should be possible to observe and ascertain when the learner has learned the skill/abilities described in the objectives.
* **Attainable**: the learner should realistically be able to acquire the skills or abilities in the time available in a workshop/by following the text of the lesson.
* **Relevant**: they should be relevant to the overall topic or domain of the lesson as a whole.
* **Time-bound**: they should include some timeframe within which the goal will be reached. For learning objectives, this is built into the approach described above.

::: success
#### Exercise: evaluating learning objectives (15 minutes)
Look at the example learning objectives below. 
Fill in the table for each objective, checking off the cells if you think an objective meets the criteria or leaving it unchecked if not. 
You should assume each objective is for a lesson to be taught in a two-day workshop. 
Note down any observations you make as you move through the list. 

If you have time, try to imagine the titles of lessons that would have these objectives.
This part of the exercise should take 10 minutes.

_At the end of this lesson, learners will be able to:_

1. create formatted page content with Markdown.
2. program with Rust.
3. fully understand GitHub Actions.

| Objective | Action verb? | Specific | Measurable | Attainable |
|-----------|--------------|----------|------------|------------|
| 1         |              |          |            |            |
| 2         |              |          |            |            |
| 3         |              |          |            |            |

Use :heavy_check_mark: :negative_squared_cross_mark: and :question: or type "yes", "no", and "maybe"/"not sure" in your copy of the table to indicate your responses.

In the last five minutes of the exercise, we will discuss as a group how each objective might be improved.
:::

::: success
#### Exercise: defining objectives for your lesson (20 minutes)
Write learning objectives for your lesson - what do you want learners to be able to do at the end of the workshop? 
When writing these lesson-level objectives, try to follow the SMART framework: make them specific, measurable, attainable, relevant, and time-bound.

Take notes about the your discussion in your Lesson Design Notes document. A record of the decisions you made and your reasons for choosing these objectives can be very helpful for you and others to understand the design and scope of the lesson later.

If you find yourself writing very specific *episode* level objectives, keep them in your notes and try to think of a slightly broader objective that may contain several very specific objectives.
We will come back and work more on episode objectives later in the training.
:::

::: success
#### Exercise: reviewing lesson objectives (15 minutes)
Swap objectives written in the previous exercise with a partner (you can also explain or show them what you wrote about your target audience, but this not essential) and review them with the following questions in mind:
- Are the objectives clear?
- Do they use "action" verbs?
- Could you directly observe whether a learner had reached this objective?

Now run the objectives through [this Lesson Objective Advisor tool from the University of Manchester's Faculty of Science and Engineering](https://web.cs.manchester.ac.uk/iloadvisor/). Do the results match your assessment?
- Where do the skills described in these objectives sit on the scale?
- (optional) Are these objectives realistic, given the target audience of the lesson?


If you're comfortable with genAI tools, a chatbot pointed at [this episode](https://carpentries.github.io/lesson-development-training/objectives.html) can also give feedback on drafted objectives, just instruct it not to rewrite them for you, only to critique.

:::

#### Key Points
- Defining objectives for a lesson can help to focus your content on the most important outcomes, and outline the scope of the project.
- Following the SMART framework can help make your learning objectives as useful as possible.
- Leaving objectives unrealistic or undefined increases the risk of a lesson losing focus or spending time on activities that do not help learners gain the most important skills.


---

### Example Data and Narrative

#### Overview
##### Objectives
After completing this episode, participants should be able to...
- Find candidate datasets to use in a lesson.
- Evaluate the suitability of a dataset to be used in a lesson.
- Choose examples that will prepare learners for formative assessments in the lesson.
- Develop a story

##### Questions
- Why should a lesson tell a story?
- What considerations are there when choosing an example dataset for a lesson?
- Where can I find openly-licensed, published data to use in a lesson?

::: success

#### Exercise: Choosing a Dataset or Narrative (30 minutes)

Referring to [the advice you reviewed before this training](https://docs.carpentries.org/resources/curriculum/narrative-example-data.html), find an appropriate dataset or a narrative for your lesson.
Identify one or more potential candidates and note down the advantages and disadvantages of each one.

As a summary, here are some aspects we suggest that you consider:

* For datasets:
    * size
    * complexity
    * "messiness"/noise
    * relevance to target audience
    * availability
    * license
    * ethics
* For narratives:
    * authenticity
    * relevance to target audience
    * complexity
    * possibility to teach useful things first/early

Take notes in your Lesson Design Notes document about your discussion and the decisions made. It may be particularly helpful to record:

* Which datasets and narratives did you consider?
* How and why did you choose between them?
* What implications do you think your choice of dataset and/or narrative will have for the design and further implementation of your lesson?
:::

Dr. Mine Çetinkaya-Rundel's keynote talk from CarpentryConnect 2019, [Let Them Eat Cake (First)!](https://www.youtube.com/watch?v=fQ4t7p6ZXDg)

#### Key Points
- Using a narrative throughout a lesson helps reduce learner cognitive load
- Choosing a lesson includes considering data license and ethical considerations.
- Openly-licensed datasets can be found in subject area repositories or general data repositories.

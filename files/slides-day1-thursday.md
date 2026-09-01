---
title: Slides - UC OSPO Network CLDT (Software Licensing Cohort) - Day 1
tags: CollabLesson, Slide, UC-OSPO-Network, Licensing
description: View the slide with "Slide Mode".
slideOptions:
  theme: simple
  #parallaxBackgroundImage: 'https://s3.amazonaws.com/hakim-static/reveal-js/reveal-parallax-1.jpg'
---

##### Collaborative Lesson Development!

![](https://carpentries.github.io/lesson-development-training/fig/CLDT-hex-sticker.png)

<!-- Put the link to this slide here so people can follow -->
slides: https://codimd.carpentries.org/OGjyBF5ISNSgX-hyMBxprg

---

![](https://ucospo.net/education/uc-ospo-network-logo.svg)

---

#### Welcome!

Congratulations on your lesson proposal being scoped for the UC OSPO Network's **Software Licensing** curriculum track.

Note:

* Cohort: Karla Padilla (UCSD, lead), Reid Otsuji (UCSD), Laura Langdon (UC OSPO), Jose Niño Muriel (UCSB)
* Lesson concept: [UC-OSPO-Network/education#83](https://github.com/UC-OSPO-Network/education/issues/83)

---

#### Who am I?

- Tim Dennis, UCLA Library Data Science Center / UC OSPO Network, organizing and teaching this training directly

Note:

* Solo-instructed this round (no co-instructor team), flag that up front so the group knows who to go to for everything
* Post-training support comes from the standing Tuesday meeting (Reid/Karla/Laura already have it; Jose joins by invite), not a separate infrastructure-developer team

---

#### Carpentries Lesson Development Lifecycle

![](https://carpentries.github.io/curriculum-development/figures/release_timeline.svg)

Source: <https://cdh.carpentries.org/the-lesson-life-cycle.html>

Note:

* This is the 30,000-foot view: lessons move from idea → drafted → piloted → stable, with community review at each stage. We'll walk this same cycle in miniature over the next two days.

---

#### Goal for your lesson

Note:

* We don't expect a "finished" lesson by the end of this training
* We want a **teachable** lesson
* Built in the Carpentries template (Workbench), that's Friday afternoon's focus
* Living in a place that can be collaborated on and further developed: your `licensing-and-copyright` repo in the UC-OSPO-Network GitHub org

---

#### Roadmap

| <!--- --> | <!-- --> |
| -------- | -------- |
| **1.** This training (Thu 8/27 PM + Fri 8/28) | **4.** Continued drafting, supported by your standing Tuesday check-in |
| **2.** Repo created live Friday, added to `licensing-and-copyright` team | **5.** Pilot to a real audience (required for checkout) |
| **3.** Build out episodes in the Carpentries Workbench | **6.** Carpentries Incubator once there's a teachable draft |

Note:

* GitHub access is already staged: `licensing-and-copyright` child team under `ospo-lesson-authors`, everyone added or invited
* Repo creation happens live in Friday's Workbench episode, not pre-staged, so you get the actual hands-on exercise as taught
* No fixed dates past this week yet, pace is set by your group and the standing Tuesday slot

---

#### UC OSPO Network support

I can help with:

* Carpentries Workbench (setup, fixing configuration)
* GitHub/Git (setup and config, PRs)
* Mapping your content into the template
* Content review and feedback as you draft

Note:

* Follow-up channel: last 15-30 minutes of Reid/Karla/Laura's standing Tuesday meeting, repurposed post-training as our working session
* Jose isn't part of that standing meeting, loop him in separately as needed
* This mirrors what worked for the IMLS Open Science cohorts: ongoing coaching beats a one-time training

---

### Questions - before we move on to the workshop

Note:

* Pause here for logistics/schedule questions only, save content questions for as they come up. If nothing, just say "let's get into it" and move on.

---

### Collaborative Development Workshop

Note:

* This is just a section divider, nothing to present, go straight to the next slide.

---

**Exercise: our first exercise (10 minutes)**

Think of an example of a great lesson that you've followed (in a class, online, in a book). What made it good? Try to separate **what was good about the performance** of the teacher from **what was good about the content** of the lesson itself. Jot a few notes, then introduce yourself to the group and share.

---

### Workshop goals

* This workshop teaches **good practices** in lesson design and development, and open source collaboration skills.
* The training is best suited to groups of trainees who want to collaborate on a lesson project, which is exactly this cohort.

---

**This training covers topics such as**:

* Identifying and characterizing the target audience for a lesson
* Defining SMART learning objectives
* Explaining the pedagogical value of authentic tasks
* Creating exercises for formative assessment
* Explaining how considerations of cognitive load can influence the pacing, length, and organisation of a lesson

Note:

SMART - Specific, Measurable, Attainable, Realistic & Timely

---

**The technical training**:

* Uses [The Carpentries Workbench](https://carpentries.github.io/workbench/), an open source lesson infrastructure that helps instructors create and publish lessons.
* Is hands-on, so you will have the opportunity to apply the principles you learn by building your lesson as we work through the content.

Source:
* [carpentries.github.io/lesson-development-training](https://carpentries.github.io/lesson-development-training)

---

### Today: Day 1 (Thu 8/27, 1:00-5:00pm PT)

Lesson Design *(~25min)* → Target Audience *(~50min)* → *break* → Learning Objectives *(~80min)* → Example Data & Narrative *(~35min, started, not finished)*

Note:

* Rough pacing checkpoints, so you can tell if you're on track without checking a separate schedule: aim to hit the break around 2:15-2:30pm, and start Narrative by ~4:15-4:25pm at the latest so it doesn't get squeezed
* Full curriculum is normally taught over several weeks; we're compressing it into two half/full days for this cohort, expect a faster pace than the source curriculum's default timing
* Friday continues at 9:00am PT sharp with Episodes, Exercise Design, Writing, the Workbench, and drafting

---

#### A Lesson Design Process

First up: how we'll approach designing your lesson, before we ever touch a website. We'll use a modified version of **backward design** (Nicholls' five-phase paradigm): start by defining what you want learners to do *after* the lesson, then design backward from there.

With your target audience already in view, our process is:

1. Define desired learning outcomes
2. Design assessments to determine progress toward them
3. Write content to lead learners from one assessment to the next
4. Assess learner progress during teaching
5. *(after the break, i.e., after you pilot)* evaluate how closely the outcomes met the objectives

---

![An overview of the iterative process of lesson design and development used in this training.](https://carpentries.github.io/lesson-development-training/fig/cldt-design-process.svg)

Note:

* This is the only process diagram the current curriculum uses: it replaces the separate "Nicholls' five phases" diagram from earlier versions of this deck
* By the end of checkout/certification you'll have completed one full loop of this cycle

---

#### Iterative Development

Lessons are never really "finished." They move through a life cycle:

![Diagram of the life cycle of a lesson in The Carpentries ecosystem. A lesson is proposed at the beginning of the pre-alpha stage. It enters alpha when it is taught for the first time. In beta, it is taught by other instructors. A full release of the lesson is made when it is stable. Pilot workshops take place during the alpha and beta phases.](https://carpentries.github.io/lesson-development-training/fig/life_cycle.png)

* **pre-alpha**: first draft is being created: this is where your lesson will sit through the end of this training
* **alpha**: taught by the original authors, not yet fully tested
* **beta**: ready to be taught by instructors not significantly involved in development
* **stable**: tested by others and improved based on feedback; changes are relatively infrequent

Note:

* Model vulnerability here: a 2-minute story about a time you piloted something and realized mid-teaching that a concept was missing: it sets the tone that "alpha" content is expected, not a failure

---

### Identifying Your Target Audience

**Two things to nail down: expertise and motivation.**

#### :female-astronaut: :book: :person_with_ball: :bulb:

---

#### Lesson Design Notes

Before the next exercise: make a copy of the shared **Lesson Design Notes** template and fill in your lesson title. You'll populate it with notes throughout the rest of the training.

https://codimd.carpentries.org/xtFJewnNRQWvF5vBlV0-gQ?view

Note:

* This is a new artifact in the current curriculum, every exercise from here on asks trainees to record their answers in this doc, not just the shared CodiMD notes
* Distinct from the CodiMD notetaking doc: CodiMD is the group's running chat/notes; Lesson Design Notes is each team's own working document
* Give everyone ~2 minutes to actually make the copy and paste their URL into the CodiMD before moving on, don't just say the instruction and keep talking

---

![](https://carpentries.github.io/instructor-training/fig/skill-level.svg)

Note:

* Novice vs. competent practitioner vs. expert: which one is Licensing's audience? Worth naming explicitly since it drives every downstream design choice today

---

**Exercise: thinking about target audience (15 minutes)**

Part 1 (5 min, individually): for a member of your lesson's target audience,

1. What is their background?
2. What do they already know how to do?
3. What do they want to do with the skills they'll learn?
4. What problem will your lesson help them solve?

---

**Part 2 (10 min, as a team):** compare answers. If you've identified different audiences, are they compatible, or is it worth narrowing to one?

Record your answers in your Lesson Design Notes doc.

---

**Exercise: defining prerequisite knowledge (5 minutes)**

Write a list of the skills/knowledge your learners will need *before* they can follow your lesson.

Note:

* If your lesson audience is novices in licensing specifically, think about baseline skills too: reading a repo's file structure, opening a text file, using GitHub's web UI. These get overlooked often.

---

### *Break*

---

### Defining Learning Objectives

#### Focus on Skills

* Ensure your audience stays motivated and your lesson feels relevant by focusing on teaching skills rather than tools.
* Lessons should be centered around what you're empowering learners to *do*, not a list of functions or commands.
* Emphasizing skills over tools helps you prioritize key concepts and consider how your lesson can impact learners' work.

---

**Cognitive Skills Come in Levels**

* Clear learning objectives should focus on teaching new, cognitive skills, things learners can do with their minds.
* Learning cognitive skills requires the ability to remember and distinguish new concepts before being able to apply and create new things.
* Remembering and distinguishing are typically easier to learn than applying and creating.
* Defining lesson objectives up front keeps you focused on necessary content and avoids distractions or missing important points.

---

### What Does an Objective Look Like?

![Lesson Objective structure](https://carpentries.github.io/lesson-development-training/fig/objective.svg)

That example is code-specific. For a conceptual lesson like ours, the same pattern (action verb + specificity) looks like:

> **explain** why a GPL-3.0-licensed dependency cannot be bundled into closed-source software

Same shape, no code: a precise verb ("explain," not "understand") plus a specific, observable scenario, not just "understand copyleft licensing."

Note:

* Objectives can be defined for a lesson as a whole, and for individual sections within it

---

**Objectives for the current section of this training:**
>1. Explain the importance of defining specific, measurable, attainable, relevant and time-bound objectives for a lesson.
>2. Evaluate a written lesson objective according to these criteria.

---

![Bloom's Taxonomy - a framework for categorising educational goals](https://upload.wikimedia.org/wikipedia/commons/6/6a/Bloom%27s_revised_taxonomy.svg)

A [computing-specific version of Bloom's](https://ccecc.acm.org/assessment/blooms-for-computing) has action verbs closer to what we're doing today.

Note:

* Updated to the canonical Wikimedia Commons image the current curriculum cites directly (the old deck used a third-party blog's version of this chart)

---

**Writing Good Objectives**

* **Learning objectives** can be defined for a lesson as a whole or for individual sections within it.
* Each objective should start with a **verb and describe one (and only one) skill** the learner will obtain.
* The skills described by the objectives should be **measurable**.
* **Action verbs** such as "explain," "choose," or "predict" are more helpful than passive verbs such as "know," "understand," or "appreciate."
* **[Bloom's Taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/)** is a useful aid for defining learning objectives.
* Learning objectives should be written in a way that is **motivating to the learner**.

---

### S · M · A · R · T

**Specific · Measurable · Attainable · Relevant · Time-bound**

---

**SMART objectives should be:**
* **Specific**: they should clearly describe a particular skill or ability the learner should have.
* **Measurable**: it should be possible to observe and ascertain when the learner has learned the skill/abilities described in the objectives.
* **Attainable**: the learner should realistically be able to acquire the skills or abilities in the time available in a workshop/by following the text of the lesson.

---

**SMART objectives should be (cont.):**
* **Relevant**: they should be relevant to the overall topic or domain of the lesson as a whole.
* **Time-bound**: they should include some timeframe within which the goal will be reached. For learning objectives, this is built into the approach described above.

---

### Exercise: evaluating learning objectives (15 minutes)

*At the end of this lesson, learners will be able to:*
1. create formatted page content with Markdown.
2. program with Rust.
3. fully understand GitHub Actions.

Rate each: action verb? specific? measurable? attainable? Then discuss as a group how each might be improved.

Table + full instructions: https://codimd.carpentries.org/SbA0GfwhQLeYYVRVDbERqA?both#exercise-evaluating-learning-objectives-15-minutes

Note:

* Spoiler for you, not the group: #2 and #3 are both bad ("program with Rust" isn't specific/attainable in a workshop; "fully understand" isn't measurable/observable). #1 is closest but could still be tighter.

---

**Lesson Scope**

* Refers to the amount of content that should be included in a lesson.
* Avoid trying to fit too much content into a lesson, that's counterproductive.
* Consider the **order in which new skills must be acquired**: higher-level cognitive skills take longer, so it's unrealistic to expect learners completing creative tasks before the end of the lesson.
* Lessons can be broadly considered as blocks of content associated with a **particular learning objective**.

---

**Exercise: defining objectives for your lesson (20 minutes)**

Write learning objectives for your lesson into your Lesson Design Notes doc, SMART, for your lesson as a whole.

**Exercise: reviewing lesson objectives (15 minutes)**

Swap with a partner, review against the SMART criteria, then run them through the [Lesson Objective Advisor tool](https://web.cs.manchester.ac.uk/iloadvisor/).

Note:

* **Instructor pacing note:** if we're running behind, this second exercise (reviewing) is the one built to skip. Point trainees to the Lesson Objective Advisor tool as homework instead of running it live. The evaluating-objectives and defining-your-own-objectives exercises above are not the ones to cut.

---

### Where We Are

#### Review

- You are clear about your audience
- You are clear about what skills you want your audience to learn
- You defined specific and realistic overall lesson objectives and outcomes

**One more thing before we build anything: your narrative.** Building the actual website is Friday's focus, right now, let's find the story that will carry your lesson.

Note:

* Don't let this slide read as "let's build the site now", that's not until tomorrow. This is a checkpoint before the last content block of today (Narrative), not a hand-off to Workbench.

---

### Example Data and Narrative

*Started today, finished tomorrow. This is intentionally left open overnight.*

---

**Why does a lesson need a narrative?**

* Writing your lesson as a story helps learners stay motivated and engaged, and connects the skills they're learning to their own work.
* For a licensing lesson specifically, the **narrative/use-case thread matters more than an example dataset**: there's no code or data being manipulated here, so what carries the lesson is a realistic licensing scenario your learners will recognize.

Further watching: Dr. Mine Çetinkaya-Rundel's CarpentryConnect 2019 keynote, [*Let Them Eat Cake (First)!*](https://www.youtube.com/watch?v=fQ4t7p6ZXDg)

Note:

* This slide deliberately de-emphasizes dataset selection relative to the standard curriculum: the source episode spends real time on dataset criteria (size, complexity, noise, license, ethics) that don't apply to a licensing lesson the same way

---

**Exercise: Choosing a Narrative (started now, continue overnight)**

Identify one or more candidate narratives/use-cases for your licensing lesson. Note the advantages and disadvantages of each.

Consider:
* authenticity
* relevance to your target audience
* complexity
* whether it lets you teach useful things early

**Overnight:** sit with this question as a team. Come back tomorrow with a candidate thread to react to, not a finished answer.

Record your discussion and decisions in your Lesson Design Notes doc.

---

### Key points, Day 1

- We use a (slightly adapted) backward design process: audience → outcomes → assessments → content → assess → evaluate.
- SMART objectives keep a lesson focused and realistic in scope.
- A strong narrative does for a licensing lesson what a good dataset does for a coding lesson, it's the thing that makes the content stick.

---

**Tomorrow: Fri 8/28, 9:00am PT sharp, hard stop at 5:00pm**

Share narrative threads → Episodes → Designing Exercises → *break* → Writing → Workbench → drafting → *lunch* → How We Operate → Preparing to Teach → Wrap-up

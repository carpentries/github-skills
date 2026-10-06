---
title: "Managing Issues"
teaching: 30
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- How can labelling help me manage issues on a repository?
- How do I add labels to issues?
- What are the recommended labels, and when should I use them?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After following this section, participants will be able to:

- Explain the value of labelling issues.
- Apply labels to issues.
- Explore the set of labels recommended by The Carpentries.
- Create milestones to help plan and track progress on their project.

::::::::::::::::::::::::::::::::::::::::::::::::

## Issue Triage
Maintainers typically do not have time to respond immediately to every new issue and comment that is added to their repository.
In a more common scenario, a Maintainer visits their repository and finds several new issues and pull requests, plus some new comments and changes to those that were open at the end of their previous visit.

A good first step to take in these circumstances is _issue triage_: time spent processing the open issues and figuring out what should be prioritised, what can be closed, what needs to be brought to the attention of others in the community (co-Maintainers, Curriculum Advisors, would-be contributors, Core Team, etc), and so on.

::: callout

## The Value of Teamwork
This triage process is usually made much easier, more efficient, and more fun when co-Maintainers of a lesson can meet synchronously to work through issues and pull requests together.

Community members have reported positive experience with short, regularly scheduled (e.g. monthly) coworking sessions with their Maintainer team, using screen-sharing and focussed discussion to distribute tasks and collaboratively determine how to process and respond to contributions.

It can also be a good opportunity for Maintainers to get to know each other better, and to share their skills and experience with using Git, GitHub, and the lesson infrastructure.

:::

## Labelling Issues
The triage process can be improved with effective use of _labels_ applied to issues.
Labels are tags that can be applied to issues (and pull requests), annotating them according to their status, type, complexity, etc.
When labels are applied to an issue, they appear next to it in the issue listing for the repository.
Clicking on a label will show you a list of all issues with that label.

When returning to a lesson repository after some time away, labels applied to old issues can help to remind you of their context, and labels can be added or updated as you triage the issue list.

### Carpentries Issue Labels
The Carpentries maintains [an expanded set of issue labels](https://docs.carpentries.org/resources/curriculum/issue-labels.html), which is larger than the default set provided by GitHub and intended to provide a more precise categorisation of issues typically encountered with a lesson. 
This label set is available on all Carpentries lesson repositories and lessons [built from one of our repository templates](https://carpentries.github.io/lesson-development-training/infrastructure.html#creating-a-lesson-repository).

::::::::::::::::::::::::::::::::::::::::::::::::: instructor

### Example Issues
Use your example repository to demonstrate how to label issues, and to discuss the appropriate use of some important labels here.

If you are using example repositories [generated with the accompanying script](instructors/instructor-notes.md),
I recommend the following labels:

* Issue 1 ("Typos in recipe instructions"): `type:typo text`, `good first issue`, `help wanted`
* Issue 2 ("Cinnamon rolls burnt 🔥"): `type:bug`, `good first issue`, `help wanted`
* Issue 3 ("Alternative to sourdough cinnamon rolls"): `status:refer to cac`, `type:discussion`

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

## Inviting Community Contributions
Lesson repositories are open source and publicly-visible, and you can expect some spontaneous contributions from the wider community.
However, in some circumstances, you may want to bring particular items to the attention of community members.

:::::::::::::::::::::::::::::::::::::::::::::::::::: spoiler

### For Maintainers of official Carpentries lessons: Refer to CAC
When you want or need to [refer an issue/contribution to the Curriculum Advisory Committee](https://carpentries.github.io/maintainer-onboarding/04-communicate-advisors.html) for your lesson, you should add the `status:refer to cac` label, and mention the CAC in the relevant issue/pull request discussion thread (e.g. `@datacarpentry/curriculum-advisors-image`).

Adding this label will help members of the CAC more easily identify and browse through the items they need to discuss, increasing the likelihood that you will receive a timely response.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

### Help Wanted & Good First Issue
The `help wanted` and `good first issue` labels can be useful to draw attention from new contributors.
In particular, the `help wanted` label can be used to flag issues that the Maintainers would particularly appreciate external support on.

The `good first issue` label is used to identify issues that do not require in-depth knowledge of the project and its infrastructure, etc.
Newcomers to the project can use this label to find opportunities to make their first contribution.
GitHub provides a view of all of a repository's issues with the `good first issue` label on the `/contribute` page for that repository, e.g. https://github.com/github/docs/contribute

::: spoiler

### Batch Labelling
Labels can be applied to issues in batches from the issue listing page.
Check the box next to each issue you want to apply a given label to, then click the "Label" dropdown in the top bar of the listing, and choose the label(s) you want to apply to these issues.

:::

## Planning Your Next Iteration
Developing a lesson is a project and, like most projects, it consists of multiple tasks. 
Keeping track of the list of tasks the team has to do, their progress on each, prioritising tasks for future development, sprints and releases, etc.,  quickly becomes a non-trivial task in itself. 
Without a project management tool/framework, it can be hard to keep track of what’s done, or what needs doing, and particularly difficult to convey that to others in the team or share the responsibilities.

Different tools and platforms exist to help you with project planning and management -- 
for example, [Asana](https://www.asana.com), [Trello](https://www.trello.com), [Miro](https://miro.com/), GitHub itself, even sticky notes on a white board. 
Different tools will work best for different teams of collaborators, but making sure you use a tool to plan and manage work on your lesson development project is better than making it up as you go along.

### Milestones
Carpentries lessons are developed in GitHub so it is convenient to use its features to keep track of different components of the project and their current status. 

GitHub offers two features for task/project management: _Projects_ and _Milestones_.
Projects offer a more advanced set of functions and are particularly useful when you need to work on related tasks spread across multiple repositories.
[Milestones](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones) are comparatively simple and a great place to start, especially if your efforts are focused on a single repository.
The focus will be on Milestones in this session but we recommend that you [learn more about Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) if you want to take advantage of the full range of GitHub's features for project management.

Milestones are a way of organising issues on your project into smaller units of work (e.g. deliverables) that have deadlines and the progress of which needs to be closely tracked (e.g. release management). 
They are good for managing time-bound, structured iterations and working in short sprints on batches of issues, which makes them a great fit for [the iterative process of lesson development recommended in Collaborative Lesson Development Training](https://carpentries.github.io/lesson-development-training/lesson-design.html). 

Here are some helpful features of Milestones:

* You can add a title and description to the Milestone, e.g. _"Issues to be addressed before October pilot workshop"_ or _"Accessibility Enhancement Drive"_.
* The Milestone represents a subset of issues on your repository, e.g. the things you want to work on next or a set of issues that share a theme.
  Issues are assigned to a Milestone in a similar way to adding a label.
* The Milestone can be given a target completion date.
* A progress bar indicates how close you are to completing the Milestone in terms of the number of completed issues versus the total number of issues.
* The order of issues listed in the Milestone can be adjusted manually by dragging the issue up and down the list, e.g. to indicate task priority to yourself and your collaborators.


:::::::::::::::::::::::::::::::::::::: testimonial

### Community members' perspectives on project management

Sven van der Burg, Research Software Engineer at the Netherlands eScience Center, describes his group's approach to piloting and contributing back to someone else's lesson in The Carpentries Incubator:

> *"At the [Netherlands eScience Center](https://www.esciencecenter.nl/) we teach ['Intermediate Research Software Development'](https://carpentries-incubator.github.io/python-intermediate-development/) 2-3 times per year. 
> After every workshop we have a short meeting to distill the most important improvements we can make for the next time that we teach. 
> We open issues for improvements to the lesson material (for example [issue-349](https://github.com/carpentries-incubator/python-intermediate-development/issues/349) and [issue-347](https://github.com/carpentries-incubator/python-intermediate-development/issues/347)).* 

> *We are not direct maintainers of the lesson, but these issues are important for us to fix before teaching the next edition of the workshop, because we don't want to run into them again. 
> Of course other users of the lesson would also benefit from the issues being fixed.*

> *Therefore, we organised a one-day sprint in which we gathered together colleagues from different teams to work on improving the lesson. 
> By all working together on one day, together in the same room, we were able to focus and get a lot done in a short amount of time, while not being distracted by the hundreds of other things we are all working on. 
> Of course, we contacted the lesson maintainers to make sure that our efforts would be welcome by opening [an issue in their lesson repository](https://github.com/carpentries-incubator/python-intermediate-development/issues/343).*

> *We used a Microsoft Planner board to organise our work and keep track of what needs to happen:*

> ![Microsoft Planner project management board](https://github.com/carpentries/lesson-development-training/assets/9945255/7705b6a8-2387-4e00-a8b8-1eaa2a512260){
alt='Microsoft Planner project management board displaying TO-DO tasks, tasks being worked on, tasks ready for internal review and completed tasks'
}

> *We bundled our contributions in [a fork of the lesson from The Carpentries Incubator in our own GitHub organization](https://github.com/esciencecenter-digital-skills/python-intermediate-development). 
> We created pull requests from that fork to a dedicated branch ([sprint-May2024](https://github.com/carpentries-incubator/python-intermediate-development/tree/sprint-May2024)) in the lesson repository. 
> We reviewed each other's work first before a final review from the lesson maintainers.*

> *In this way, we could adapt the lesson to our own needs and contribute to the lesson in The Carpentries Incubator in a smooth way that does not take away focus on other projects of me and my colleagues."*

Renata Curty, Research Facilitator for Social Sciences at UCSB, describes her group's approach:

> *Our group uses issues and labels and sets milestones in GitHub to organize our lesson development work.*
> *We also use a spreadsheet to track higher-level decisions, tasks, and assignees and record ideas and discussion points in our meeting notes before converting them into more detailed issues.*
> *We have been meeting regularly (weekly or biweekly) to maintain momentum, which helps us to make small but steady progress.*
> *We are currently working on a modularized version of the workshop that will allow instructors to choose what to teach based on the time, cohort needs, and learners’ entry knowledge.*

::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::: callout

### Referencing issues
It can be helpful to refer to issues and pull requests in conversations elsewhere in a repository.
Every issue and PR has a unique number (based on the order in which they were created). These numbers can be used, preceded by `#`, to reference a given issue or PR.

Additionally, pull requests (and commit messages) that include particular phrases will trigger the automatic closure of an issue:

- "closes"
- "fixes"
- "resolves"

One of the above words followed with the `#` and the number of an issue, e.g. _"fixes #34"_, included in the description of a pull request (the first comment in the PR discussion thread) will tell GitHub that the issue can be automatically closed if the pull request is merged.

::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::: keypoints

- Labelling issues can help you prioritise issues and bring them to the community's attention.
- Labels can be added to an issue using the right sidebar menu of the GitHub web interface.
- The Carpentries provides a recommended set of labels, and has systems and processes that work with some of these.

::::::::::::::::::::::::::::::::::::::::::::::::

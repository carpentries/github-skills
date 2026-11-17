---
title: "Reviewing Pull Requests"
teaching: 30
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- What features does GitHub provide to facilitate reviewing pull requests?
- What are the different options for the outcome of a pull request review, and when should I use each one?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After following this section, participants will be able to:

- Create comments on particular lines and ranges of lines in the changes proposed by a pull request.
- Suggest specific changes to a pull request.
- Select the "approve", "comment", or "request changes" outcomes of a pull request review.

::::::::::::::::::::::::::::::::::::::::::::::::

Reviewing pull requests is one of the most important tasks for a maintainer.
The way you review a pull request, and communicate with the person who opened it, can have an enormous impact on their motivation to contribute again.
It also sets expectations for them and others about your priorities and quality standards for the project.
When done well, reviews can be an enjoyable, educational, collaborative experience for both maintainer and contributor.

GitHub provides several features that can improve your experience as a reviewer, and make it easier for contributors to follow up on your review.

## Title and description
A good title and description for a pull request should give the reviewer an immediate impression of the goal(s) and scope of the changes it contains.
[Pull request templates, covered later](./collaborating_newcomers.md#guide-contributors-with-issue-and-pull-request-templates), are one way to help contributors provide this information.

## Line-by-line comments
The specific changes proposed in a pull request can be viewed in its _Files Changed_ tab.
It is usually most helpful to provide feedback and ask questions on the lines that have been changed.
You can comment on a particular line by hovering the cursor over it and clicking the `+` button on the left-hand side.
Comments can be added on their own, or as part of a _Review_: a commentary on the pull request as a whole. When choosing the latter, comments are only published after the reviewer has finished the whole review.
To comment on a range of lines, click-and-hold the `+` button for the first line in the range, drag your cursor down the range, then release.

## Suggesting changes
As well as adding comments line-by-line, you can also suggest specific changes, e.g. to fix a typo, suggest improved wording, etc.
To do this, take the same approach to start a comment on a line or range of lines, then click the "add a suggestion" button (plus/minus symbol inside a document icon), and edit the source content that appears in the input box with your suggested improvement.
Suggesting specific changes makes it much easier for contributors to a) understand your suggestions, and b) implement them.
Suggested changes will be commited to the pull request branch as co-authored by the pull request author and reviewer.

## Finishing a review
When you have finished commenting on particular lines, and suggesting changes, you can finish your review by clicking the "Review changes" or "Finish your review" button near the top-right of the screen.
This is the place to add general comments and questions, and to summarise your review.
If nothing else, do not forget to thank the contributor for taking the time to contribute!
Choose one of the three options:

- "Comment" - a general comment, with no firm outcome. This option can be a good choice if you plan to close the pull request after completing your review.
- "Approve" - approve the PR for merging. Some people use this when suggesting only very minor or optional changes - if you want to do this, make sure you are explicit about what changes you are suggesting etc before the PR can be merged
- "Request changes" - indicates that changes would be required to the PR before you would be willing to merge it. It also requires another review before the changes can be merged if the `main` branch has been protected (see branch protection rules below).

## Agree with your team how you will use reviews
When collaborating regularly with other developers/maintainers on a project, it can be helpful to discuss and agree upon when and how you will use pull requests and reviews in your development process.
Where quality control and shared ownership is important, teams may prefer for all changes to pass through pull requests, perhaps even requiring at least one approving review before changes can be merged.
([Branch protection rules](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches) can be set in GitHub to enforce such requirements.)
Other teams prefer less formal process, with pull requests used only when a team members specifically wants to invite feedback and discussion on their changes.

However you decide to integrate pull requests into your development process, we recommend discussing it as a team and making agreements about how you will work together.


::::::::::::::::::::::::::::::::::::::::::::::::: instructor

### Reviewing Example Pull Requests

Use the example repository to show an example of reviewing a pull request, demonstrating:

* line-specific comments
* suggesting a change
* approving/requesting changes at the end of the review

If you are using example repositories [generated with the accompanying script](instructors/instructor-notes.md),
I recommend using the "Add detail to the project README" pull request
to demonstrate line-by-line commenting and suggesting changes:
you can suggest that the contributor uses a different email address, for example.

The purpose of the other two pull requests is to:

1. Repeat the reviewing workflow two more times,
   giving you a chance to emphasise the important steps
   and encourage good communications practices.
2. Create a merge conflict that can be resolved in the GitHub web browser interface
   (see the Instructor Note for the next episode).

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::


::: spoiler

## Saved Replies

- You can add "saved replies" to your GitHub account
- These can be used to automatically input a template response, on issues, PRs, etc
- Use these if you find that you are often saying the same or similar things to people

:::

:::::::::::::::::::::::::::::::::::::: keypoints

- Use line-specific comments and suggestions, and indicate the outcome of your review to help the contributor respond effectively.
- The "approve" and "request changes" options on a review can help the contributor understand if they need to take further action.

::::::::::::::::::::::::::::::::::::::::::::::::

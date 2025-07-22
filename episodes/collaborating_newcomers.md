---
title: "Collaborating with Newcomers"
teaching: 30
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- What can I do to attract contributors to my project?
- How can I help them make good contributions when they get there?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After following this section, participants will be able to:

- adjust a repository to attract potential new collaborators.
- create and modify issue and pull request templates in GitHub.
- identify channels they can use to attract contributions from relevant community members.

::::::::::::::::::::::::::::::::::::::::::::::::

## Maintain a welcoming repository
It is important to make collaborative projects as welcoming and as easy to get involved in as possible for newcomers.

### Document your project
One way to make sure you achieve this is to spend time on ‘external-facing’ features, such as documentation, that will make the project more accessible to newcomers. 
Such documentation will be useful to yourself and other team members as well, e.g. if you are trying to come back to the project after a break or are reusing it for a new collaboration in the future.

Your lesson documentation should contain the following information, which should be kept up to date:

:::::::::::::::::::::: instructor

#### Share an example of a good README
It is helpful to share an example of a README when teaching this section.
Use your own example if you have one, or otherwise share [the README from the source repository of this training curriculum](https://github.com/carpentries/lesson-development-training/blob/main/README.md).
We try to keep it updated and aligned with the recommendations here.
Please let the Maintainers know by [opening an issue](https://github.com/carpentries/lesson-development-training/issues/new/choose) or [a pull request](https://github.com/carpentries/lesson-development-training/edit/main/README.md) if you identify anything that could be improved.

:::::::::::::::::::::::::::::::::

* A structured, up-to-date README. 
  The README, often a `README.md` or `README.txt` file, represents the first piece of documentation that people will find when they arrive at your lesson repository.
  You should aim to capture all the information that a potential contibutor or user might need to understand what the project is and how to work with it.
  Consider including the following information:
    - **lesson title**
    - **lesson description**
    - **information about how to use the project** - this might be a link to the rendered version of the lesson or to further documentation, or installation instructions and some examples of usage
    - **list of maintainers** - let people know who is responsible for the project and how to contact them
    - **contributing information** - summarise the kinds of contributions you are seeking and how to get involved, linking to the repository `CONTRIBUTING.md` file for more details
    - **credits/acknowledgements** - acknowledging past maintainers and others who have helped build the project and templates and resources you have used and adapted gives would-be contibutors confidence that their efforts will be credited too
    - **citation** - tell people how they should cite your project. This could be a sumamry of the detailed information you provide in a separate `CITATION.cff` file (see below)
    - **license** - summarise the licensing terms of the project, linking to the project's full license file (see below).
* A up-to-date `CITATION.cff` file.
  A file containing information about the authors of the project, other projects and resources it is based on or refers to, its license, the DOI of the latest version, etc, in [Citation File Format (CFF)](https://github.com/citation-file-format/citation-file-format) (a specialised kind of YAML file).
  If your lesson repository contains a `CITATION.cff` file, GitHub will automatically show the citation information in the sidebar. 
  CFF is also recognised and supported by other platforms including [Zenodo](https://zenodo.org/) and the [Zotero reference manager](https://www.zotero.org/).
* `CONTRIBUTING.md`. 
  A contributing guide describing how people can send their contributions, what kinds of contribution will be credited and in what ways. 
  Carpentries lesson repositories already have a generic Carpentries `CONTRIBUTING.md` file to get you started, which you should review and modify to fit the needs of your project and team.
* `LICENSE.md`.
  A file containing the licensing terms of the project, including the conditions under which others may re-use, adapt, and distribute its contents.
  Without a license other people cannot use your material at all.
  Use GitHub's license choosing tool or find another pre-existing license that fits your needs (e.g. from Creative Commons).
  Do not write your own!

:::::::::::::::::::::::::::::::::::::::::: spoiler

#### Templates for lesson developers

We have prepared the following templates to help lesson developers get started with writing the README and contributing guide for their project:

* [`README.md` template](https://github.com/carpentries/lesson-development-training/blob/main/files/templates/README-template.md?plain=1)
* [`CONTRIBUTING.md` template](https://github.com/carpentries/lesson-development-training/blob/main/files/templates/CONTRIBUTING-template.md?plain=1)

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::: callout

#### Digital Object Identifiers
We recommend that lesson developers obtain a [Digital Object Identifier (DOI)](https://the-turing-way.netlify.app/communication/citable/citable-steps.html?highlight=doi#dois) as soon as feels appropriate, at the latest when the lesson reaches the beta phase. You can use this DOI in the citation information (e.g. [in the `identifiers` field of your `CITATION.cff`](https://github.com/citation-file-format/citation-file-format/blob/main/schema-guide.md#identifiers)), to allow people to cite a particular version of your lesson, e.g. a snapshot of the lesson when it entered beta testing, captured as a Zenodo record.

::::::::::::::::::::::::::::::::::::::::::::::::::


### Cultivate and present a welcoming project culture
Many potential contributors will "lurk" on an open source project before making their first contribution and many occasional contributors are probably paying attention to activity on the repository too.
People often feel intimidated about contributing to a project for the first time and anything you can do to reduce that barrier and encourage them to participate will help you grow the community around your project.

#### Be intentional about your public communications
All projects have a culture, much of which will be visible on a public GitHub repository, whether maintainers try to actively establish and nurture it or not.
Investing time and energy in communicating in a polite and friendly way, even among a small group of team members who collaborate with each other all the time, shows newcomers how they can expect to be received when they make their first contribution.
Modeling respectful behaviour between maintainers demonstrates to anybody watching (or looking back at past discussion threads) something important about the culture of your project.

Discuss with your team members how you want to work together then establish those norms and work to maintain them.

#### Be responsive
It helps to process and respond to contributions quickly, especially when somebody is participating in the project for the first time.
Longs delays between opening an issue or pull request and a first response from a maintainer can be demotivating.
Similarly, after waiting a long time for a response, the contributor may no longer have time to follow up, having moved on to other tasks and projects.

Make sure that you have [configured notifications for your project](./collaborators_team.md#staying-in-the-loop) so that you will know about it when somebody gets involved.

#### Say _"no"_ when you need to

Not every contribution is a good fit for a project and you probably will not want to accept every suggested change, especially in its later stages.
If you receive a pull request or issue that does not fit to your lesson, consider the following points to help you politely decline without demotivating the contributor:

1. **Thank them** for taking the time to contribute.
2. **Explain why the contribution does not fit** into the lesson, and offer suggestions for improvement if you're able to.
3. **Link to relevant documentation**, if you have it.
    Notes about the design and scope of the project and any relevant discussion threads can be very helpful here.
   If you notice similar repeated requests/contributions, you might want to address them in your documentation (e.g. in the `CONTRIBUTING.md` file) to save yourself time in future.
4. **Close the request**.

The advice above is taken from [The Carpentries Maintainer Onboarding curriculum](https://carpentries.github.io/maintainer-onboarding/02-communicate-contributors.html), and based on [the _Best Practices for Maintainers_ guide from GitHub](https://opensource.guide/best-practices/#learning-to-say-no).

## Encourage impactful contributions
Your project will benefit most when newcomers make meaningful contributions and they will feel more motivated to get involved when they can see that their contributions will be welcomed and make an impact.

### Boost visibility for newcomers
Anything you can do to draw attention to issues where new contributions would be easy and/or particularly impactful can help to get newcomers involved in your project.
The Carpentries provides a number of ways to further raise the visibility of the lesson among the broader community and encourage community members to contribute to its further development.

  - Maintaining a list of issues with the `help wanted` and `good first issue` labels from lesson repositories on [The Carpentries website](https://carpentries.org/help-wanted-issues/).
  - Featuring projects [The Carpentries blog and newsletter](https://docs.carpentries.org/handbooks/lesson_developers.html#promoting-your-project-in-the-incubator-lesson-spotlight).
  - Helping maintainers organise and promote collaborative development sessions for their projects.

The examples listed above can be adapted to other project settings: the important takeaway message is that maintainers should invest time in outreach, rather than passively hoping for newcomers to spontaneously appear.

The Carpentries community handbook includes a set of [recommendations for organising and running a lesson sprint](https://docs.carpentries.org/resources/curriculum/lesson-sprint-recommendations.html), most of which applies equally well to the co-creation of other kinds of (open source) projects.

### Curate issues on your repository
Long discussion threads with no clear resolution or action steps can be another barrier for would-be contributors to overcome.
One good technique for maintainers to mitigate this is to periodically summarise the current state of a discussion, to make it easier for newcomers to understand what is needed to make progress on a given issue or pull request.
(Other contributors may find this helpful too!)
As the context and details of an issue change and become clearer over time, it can be similarly helpful to adjust the title and opening comment of the discussion. 
Bear in mind that editing an existing comment will not trigger a notification to those subscribed to the thread in the same way that a new comment would: you should post a new comment to make sure that everyone involved is aware of your changes.

### Guide contributors with issue and pull request templates
[Templates for new issues and pull requests](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository) can guide newcomers and experienced contributors to provide the information you need to be able to process and respond to their contributions efficiently.

A pull request template specifies Markdown content that will be present by default in the description box of any new pull request on the project.
Use it to prompt contributors to provide any information that will help you process and review their proposed changes.
Issue templates can also contain a default description for a new issue or define a more structured set of prompts for contributors to respond to by templating a form that contributors must complete to open an issue.

Multiple templates can be specified for issues and pull requests on a project, providing different guidance for contributors making different kinds of contributions (e.g. reporting a bug, asking a question, providing feedback from a pilot workshop, etc).

Issue and pull request templates are kept in the `.github` folder of a repository. 
([Templates can also be configured at the organization level](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file#creating-a-repository-for-default-files).)

Issue form templates are specified with YAML and saved with the `.yml` filename extension.
GitHub's web interface has some built-in checks and syntax highlighting to help you compose them.
Pull request templates and non-form issue templates are written as Markdown files (`.md` extension) with metadata such as default labels and assignee for the resulting issue specified as YAML front matter at the top of the file.

:::::::::::::::::::::::::::::::::::::: keypoints

- Encourage newcomers to get involved by maintaining good documentation and a welcoming atmosphere in your project.
- Help contributors make an impact on your project with detailed issues, issue and pull request templates, and a detailed contributing guide.

::::::::::::::::::::::::::::::::::::::::::::::::

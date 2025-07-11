---
title: "Collaborating with Newcomers"
teaching: 30
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- Q1
- Q2
- Q3

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After following this section, participants will be able to:

- adjust a repository to attract potential new collaborators.
- create and modify issue and pull request templates in GitHub.
- identify channels they can use to attract contributions from relevant community members.

::::::::::::::::::::::::::::::::::::::::::::::::

## Maintaining a Welcoming Repository
It is important to make collaborative projects as welcoming and as easy to get involved in as possible for newcomers.

### Documenting Your Lesson
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
* Issue and pull request templates.
  [Templates for new issues and pull requests](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository) can guide newcomers and experienced contributors to provide the information you need to be able to process and respond to their contributions efficiently.

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


::::::::::::::::::::::::::::::::::::::  challenge

## Exercise: preparing your repository for collaboration (15 minutes)

Spend some time doing **one of the following**:

1. Modify the `README.md` and `CONTRIBUTING.md` files in your repository
   to provide the relevant information for would-be contributors to your lesson:
   - the name(s) of the current developer(s), linked to their GitHub profile(s) (README)
   - contact information (README, CONTRIBUTING)
   - guidance on how people should contribute, and what kinds of contribution you are most interested in receiving (CONTRIBUTING)
   - links to any important background information (README)
   - links to any funding bodies or host institutes that are supporting the development of the lesson (README)
2. Create a new issue or pull request template, or modify an existing one,
   to guide contributors on how best to begin collaborating with you on GitHub.
3. Using [the `cffinit` webtool](https://citation-file-format.github.io/cff-initializer-javascript/), create a `CITATION.cff` with information appropriate to your project (listing authors, including the lesson title, repository URL, etc) and overwrite the current placeholder content with the result.

Groups of collaborators taking this skill-up together should discuss first how they will assign these tasks between them.

::::::::::::::::::::::::::::::::::::::::::::::::::

### Presenting a Welcoming Project Culture


## Attracting Impactful Contributions
Content goes here.

:::::::::::::::::::::::::::::::::::::: keypoints

- KP1
- KP2
- KP3

::::::::::::::::::::::::::::::::::::::::::::::::

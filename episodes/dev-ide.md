---
title: "Working in the github.dev IDE"
teaching: 25
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- What is the github.dev IDE?
- When might it be helpful to use the github.dev IDE?
- How can I open pull requests from the github.dev IDE?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

After following this section, participants will be able to:

- Open a repository in the github.dev IDE.
- Create branches, modify and commit files, and open pull requests from the github.dev IDE.
- Populate a `CITATION.cff` file for their project with the cff-init webtool.

::::::::::::::::::::::::::::::::::::::::::::::::

## Another Way to Work
The GitHub browser interface is great for looking through files and folders, viewing the project history and details of specific changes, and managing issues and pull requests.
But it has some limitations, such as needing to commit changes each time we modify a single file:
it is common in practice to want to "package together" changes to multiple files as a single commit.
Developers often clone a project locally to obtain more flexibility in how they work with a repository, to preview changes before they commit, etc.
However, it can be cumbersome to make a clone of every project you want to contribute to.

In recent years, GitHub has provided something like a middle ground: 
an [integrated development environment (IDE)](https://glosario.carpentries.org/en/#ide) to work with your repositor without leaving the web browser.
This IDE interface, called github.dev, is available on all GitHub repositories.
There are a few different ways to access it:

1. Navigate in the standard GitHub interface to a file you want to modify.
   Select the downward arrow next to the edit button (pencil icon), and choose "github.dev" from the dropdown list.
   ![](fig/edit-dropdown.png){alt='the edit dropdown menu'}
2. Edit the URL in your browser address bar to replace github**.com** with github**.dev** then hit <kbd>Enter</kbd>.
3. Press the <kbd>.</kbd> key while viewing the contents of any file or directory in your repository (including the repo home page).

After taking any of the steps above, the IDE interface will launch in our browser tab.
It can take a few moments to get started but then you should find yourself in an IDE view of the repository.

TODO demo creating CFF and adding a citation info to README
create a branch, view diff, commit changes, open PR from IDE
switch back to standard interface to merge changes

TODO 

:::::::::::::::::::::::::::::::::::::: keypoints

- The github.dev IDE is a more flexible interface for working with repositories in the web browser.
- The IDE interface can be helpful when you need to make substantial changes to a repository but it is inconvenient or impossible to clone it locally.
- Changes can be staged and commited, and pull requests opened, from the version control sidebar tab of the IDE interface.

::::::::::::::::::::::::::::::::::::::::::::::::

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
But it has some limitations.
It is common practice to edit multiple files in one go and package them together in one commit, but the GitHub browser interface can only edit and commit single files at a time.
It can be helpful to refer to the contents of other files even when only making edits to a single file.

Developers often clone a project locally to obtain more flexibility in how they work with a repository, to preview changes before they commit, etc.
However, it can be cumbersome to make a clone of every project you want to contribute to.

In recent years, GitHub has provided something like a middle ground: 
an [integrated development environment (IDE)](https://glosario.carpentries.org/en/#ide) to work with your repository without leaving the web browser.
This IDE interface, called github.dev, is available on all GitHub repositories.

### Launching the github.dev IDE
There are a few different ways to access the IDE interface:

1. Navigate in the standard GitHub interface to a file you want to modify.
   Select the downward arrow next to the edit button (pencil icon), and choose "github.dev" from the dropdown list.
   ![](fig/edit-dropdown.png){alt='the edit dropdown menu'}
2. Edit the URL in your browser address bar to replace github**.com** with github**.dev** then hit <kbd>Enter</kbd>.
3. Press the <kbd>.</kbd> key while viewing the contents of any file or directory in your repository (including the repo home page).

After taking any of the steps above, the IDE interface will launch in our browser tab.
It can take a few moments to get started but then you should find yourself in an IDE view of the repository.

The new interface will feel familiar to participants who are already making frequent use of an IDE, especially VS Code.
For those less familair, a short tour of the interface:

* The window is arranged in panels. 
* The main, central panel provides an editing view of the source files you open, and can display a rendered preview of Markdown files.
  At launch, this central panel will display a preview of the rendered `README.md`.
   * To open such a Markdown preview, right-click on a `.md` file in the sidebar and select "Open Preview".
* The left side of the screen includes a sidebar with a series of icons to switch between different menus/tools in this sidebar.
  At launch, the sidebar displays a file explorer tool, from which you can open existing files for editing, create new directories and files, etc.
  Other modes of that sidebar provide an interface to search, version control, the extension marketplace for VS Code, GitHub, etc.
* The bottom panel includes a console and a terminal interface.
  These can be used to run shell commands and source code in the repository, see the output/error messages, etc.

:::::::::::::::::::::::::::::::::::::::::::::::::: discussion

### Editing files in the github.dev IDE

The `CITATION.cff` file in your example repository is a placeholder populated mostly by FIXMEs.
Let's update it and add a link to [the _Acknowledgements and Citations_ page it produces](https://carpentries.github.io/sandpaper-docs/editing.html#making-your-lesson-citable) to the README file.

#### 1. Edit `CITATION.cff`

1. Visit [CFF INIT](https://citation-file-format.github.io/cff-initializer-javascript/#/) and select _Update_.
2. Paste the current contents of `CITATION.cff` into the box and select _Parse_ then _Start Editing_.
   For the purposes of Citation File Format, our lesson repository is a _Dataset_.
3. Adjust a few fields in this edit interface, e.g. _Title of the dataset_, the author (use your own details or make some up), the abstract, etc.
4. When you are done editing, select _Copy to clipboard_ near the top-right, and paste the new contents into your `CITATION.cff` file (replacing the current content).

#### 2. Link to the Lesson Citation page from `README.md`

1. Open your `README.md` for editing.
   (You cannot edit the file from the preview that was opened by deault when we launched the IDE interface.)
2. Add a new section heading at the bottom of the file, e.g. `## Cite this Project`
3. Add a link under that heading, pointing to the _Acknowledgements and Citations_ page of the lesson site.
   The URL to that page is `<base url of your lesson site>/citation.html`.

#### 3. Commit the changes and open a pull request

1. Open the version control interface in the left sidebar. 
   The two modified files are staged for commit by default, but **we do not want to commit the changes yet**. 
   We should first switch to a new branch, so that we can open a pull request and get the changes reviewed before they are merged.
2. Find `main` in the toolbar right at the bottom of the screen.
   Select that part of the toolbar and choose _Create new branch_ from the dropdown that appears at the top of the window.
   Enter a name for the new branch, e.g. `citation-page`.
   Confirm that you want to switch to that new branch.
3. Now commit the changes in the version control sidebar.
   Write a short commit message, e.g. "populated CFF and linked to citation page", then select _Commit & Push_.
4. Open a pull request to merge these changes into the `main` branch.
   Select the three dots at the top-right of the version control sidebar interface, then select _Pull Request_ -> _Create Pull Request_.
   Provide a title and description for the PR then select _Create Pull Request_.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

To return to GitHub's standard repository web interace, select _GitHub_ from the very bottom-left of the window, then _Go to Repository_ from the dropdown that opens at the top of the window.
From here, you can find the newly-opened PR, review and merge it as discussed earlier.

## Codespaces: preview changes to your lesson in the browser
Repositories that contain a `.devcontainer` directory can be launched in a _codespace_: a configured development environment running inside a container, hosted on GitHub's systems in the cloud.
That directory includes files that specify the configuration of the codespace environment.
(`.devcontainer` use is not limited to Codespaces: the same directory can be used to setup an equivalent environment for development in a local version of VS Code.)
Our lesson template includes a `.devcontainer` describing the software required running The Carpentries Workbench, which means that we can launch a Codespace running the lesson infrastructure in the github.dev IDE.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

### While you are waiting...
The codespace can take a bit of time to launch.
This is a good opportunity to answer any questions participants have, and/or to point them towards the installation instructions for the Workbench so that they have another way to build their lessons locally.
You could also talk more about the contents of `.devcontainer/Dockerfile`, if the participants have sufficient technical expertise to follow that.

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

1. From the home page of your lesson repository, select _Code_ -> _Codespaces_ -> _Create Codespace on main_.
   This will launch the github.dev interface again, but this time in an environment that includes The Carpentries Workbench R packages.
   The initial launch can take a few minutes to complete.
2. Once the IDE has finished setting up, you will get a similar IDE interface but with a console prompt starting with `rstudio@codespaces-`.
   Typing `R` into that console prompt and pressing <kbd>Enter</kbd> will launch an R session.
3. In that R session, run the following commands to build the lesson and launch a server to provide live previews of the lesson as we make changes:
   
   ```R
   library(sandpaper)
   sandpaper::serve()
   ```

   This lesson preview will appear in a new browser tab.
   The URL is shareable, so you can use it to show your colleagues/co-maintainers how some new version of the lesson would look after changes on your working branch have been merged.
4. Let's test it out!
   Make some changes to the `index.md` of the lesson, or one of the episode source files.
   This will trigger a rebuild of the relevant pages and, after a short time, the preview will refresh, with the new changes visible.

This kind of live preview can be very helpful for source repositories of GitHub Pages websites.
A similar approach, with `.devcontainer` and codespaces, can be valuable for software projects as well: providing a fully configured development environment for the software, with unit tests etc, dramatically reducing the barrier for new contributors to engage with the project.

::::::::::::::::::::::::::::::::::::::::: caution

### Codespaces can cost money!
It can cost you money to run these codespaces on GitHub's systems: [users and organisations have quotas of free usage](https://docs.github.com/en/billing/concepts/product-billing/github-codespaces), which is tracked in terms of time and storage space.
Minor usage typically falls below the limits of these quotas but if you do exceed them, you will either be unable to keep using your codespaces until the next billing period begins, or you will be charged for continued usage.
We recommend that you review the billing documentation linked above, and consider the following advice:

1. [**Keep track of your usage** and billing settings with GitHub](https://github.com/settings/billing/usage).
2. **Stop your codespaces** when you are not using them.
   Back in the standard web interface of your repository, select _Code_ -> _Codespaces_ then use the three dot menu next to a running Codespace.
   Choose _Stop codespace_ when you have finished working with the codespace.
3. **Delete unused codespaces**.
   If you do not expect to need it again, select _Auto-delete codespace_ so that a codespace does not accrue storage costs after it has been stopped.
   You can view a list of all codespaces for a repository by selecting _Code_ -> _Codespaces_ -> three dot menu -> _Manage codespaces_ and clean up old Codespaces from that listing.

:::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::::: discussion

### Stop and delete your codespace
Following the steps described in the callout above, stop the codespace you launched while following this episode, and select _Auto-delete codespace_ to ensure that it is not stored.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::: keypoints

- The github.dev IDE is a more flexible interface for working with repositories in the web browser.
- The IDE interface can be helpful when you need to make substantial changes to a repository but it is inconvenient or impossible to clone it locally.
- Changes can be staged and commited, and pull requests opened, from the version control sidebar tab of the IDE interface.

::::::::::::::::::::::::::::::::::::::::::::::::

<div align=center>

<img src=/assets/Git-Logo.eps>

</div>

- [Introduction to Git](#introduction-to-git)
  - [What is "Git"?](#what-is-git)
  - [Instalation](#instalation)
  - [Remote repositories](#remote-repositories)
    - [What is GitHub, GitLab and Bitbucket?](#what-is-github-gitlab-and-bitbucket)
- [Git commands](#git-commands)
  - [Start](#start)
    - [Clone a existing project](#clone-a-existing-project)
    - [Create a git project from scratch](#create-a-git-project-from-scratch)
    - [Create a new local repository](#create-a-new-local-repository)
  - [Commit Changes](#commit-changes)
    - [Add a commit](#add-a-commit)
    - [Show a commit](#show-a-commit)
    - [Add local changes to repository](#add-local-changes-to-repository)
  - [Delete the file from project and stage the removal for commit](#delete-the-file-from-project-and-stage-the-removal-for-commit)
  - [Change a existing file path and stage the move](#change-a-existing-file-path-and-stage-the-move)
  - [Branches](#branches)
    - [Create a new branch](#create-a-new-branch)
    - [Switch to another branch and check it out into your working directory](#switch-to-another-branch-and-check-it-out-into-your-working-directory)
  - [Commit history](#commit-history)
    - [Show all commits in the actual branch and all files](#show-all-commits-in-the-actual-branch-and-all-files)
    - [Show all changes for a specific file](#show-all-changes-for-a-specific-file)
    - [Diff of what is changed but not staged](#diff-of-what-is-changed-but-not-staged)
    - [Commit your staged content as a new commit snapshot](#commit-your-staged-content-as-a-new-commit-snapshot)
  - [Undo](#undo)
    - [Discard all local changes](#discard-all-local-changes)
  - [Tags](#tags)
    - [Add a tag in current branch](#add-a-tag-in-current-branch)
- [Readme in other languages](#readme-in-other-languages)
- [Other tools and tips](#other-tools-and-tips)
  - [Graph](#graph)
  - [GUI Clients](#gui-clients)
    - [What is a "GUI" for git?](#what-is-a-gui-for-git)
  - [Visual Studio Code: extensions](#visual-studio-code-extensions)
- [Contributors](#contributors)

# Introduction to Git
## What is "Git"?

Git is the main **version control system** used in the world. Version control is a system that *records changes to a file or set of files over time so that you can recall specific versions later*.

This provides many advantages like multiple people working on the same project asynchronously, testing changes to a system without having to worry about reverting to a previous state if necessary, compare changes in files, maintaining different versions of the same system on the same place but separate, keep a history of changes for future reference, among others.

[Official page](https://git-scm.com/)

## Instalation

Debian/Ubuntu:
> `apt-get update`

> `apt-get install git`

Arch Linux:
> `pacman -S git`

[Other Distributions](https://git-scm.com/download/linux)

-------

## Remote repositories

It is entirely possible to work with git locally on your machine without other contributors, since some of the benefits of git are keeping track of changes in time, so to clarify there's a separation between git and platforms like GitHub, GitLab, or Bitbucket; but teams and companies always work with remote repositories, and developing alone makes it so you never run into some of the problems git is great at solving, so it is important to understand how to work with those as well.

### What is GitHub, GitLab and Bitbucket?

They are all platforms that provide internet hosting for version control using Git. They also provide further tools for software development management like source code management, access management, bug tracking, feature requests, task management, continuous integration and documentation hosting, to name a few.

They let you upload code either publicly or on private repositories and integrate with git to use its many benefits.

<div align=center>

[GitHub](https://github.com/about) |
[GitLab](https://about.gitlab.com/) |
[Bitbucket](https://bitbucket.org/product/)

</div>

# Git commands

<img align=center src=/assets/terminal.png>

## Start
### Clone a existing project

Once you have the repository url you clone it (which will download its main/master branch) with:
> `git clone <repository-url>`

This will create a folder with the repository name wherever you are. If you want to specify a path or a folder name, simply add it as a argument:

> `git clone <repository-url> /path/to/git_folder`

### Create a git project from scratch

Go to the directory with the project code (or an empty directory to start from zero) and run:

> `git init`

This will create a new project where all files and subfolders are

> `git remote set-url origin https://github.com/Cygnus-Software/intro-git.git`

*Note:* The remote url is generally the https repository url with a `.git` at the end

### Create a new local repository


---
## Commit Changes

> `git status`

### Add a commit

> `git commit -m "Tittle commit example" -m "Commit description"`

Note: The second commit message (`-m` flag) is optional

### Show a commit

> `git show <tag-commit>`

### Add local changes to repository

> `git add`

## Delete the file from project and stage the removal for commit

> `git rm <name-file>`

## Change a existing file path and stage the move

> `git mv <existing-path> <new-path>`

## Branches

### Create a new branch

> `git branch <name-branch>`

### Switch to another branch and check it out into your working directory

> `git checkout <name-branch>`

## Commit history

### Show all commits in the actual branch and all files

> `git log`

### Show all changes for a specific file

> `git log -p <file>`

### Diff of what is changed but not staged

> `git diff`

### Commit your staged content as a new commit snapshot

> `git diff --staged`

## Undo

### Discard all local changes

> `git reset --hard <commit>`

## Tags

### Add a tag in current branch

> `git tag <tag-name>`

# Readme in other languages

[README ES](/README_ES.md)


---

# Other tools and tips

## Graph

> `sudo apt install gitk`

## GUI Clients
### What is a "GUI" for git?

https://git-scm.com/download/gui/linux

## Visual Studio Code: extensions

---

# Contributors


TEST
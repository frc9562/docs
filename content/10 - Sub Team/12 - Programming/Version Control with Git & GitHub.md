---
title: Version Control with Git & GitHub
aliases:
created: 2025/12/03
modified: 2026-01-20T15:12:21-05:00
tags:
  - programming
  - config
draft: false
todo: true
---
> [!warning] This Note is Unfinished!
> 
> This note is missing information, if you have information to help finish this note, share with the [[10 - Sub Team/15 - Documentation/index|Documentation Team]] and help out!

## Introduction to Git: Version Control and You
**Git** is a piece of version control software used across the programming world to keep track of contributions and version history of software projects. It allows people to see when changes were made and who made them. It serves as a backup to allow us to revert back to old code if a change breaks something.

**GitHub** is a website which stores Git repositories. It serves as a central storage place for our code, which we can pull and push from at will.

## Installing Git
##### Windows
Go to https://git-scm.com/install/windows and download "Git for Windows/x64 Setup".
Run the setup program to install Git.
##### Mac
This assumes you have the Homebrew package manager installed.
Open a terminal and run `brew install git`.
##### Linux
You already have Git or you at the very least know how to install it.

## Configuring Git
Run the following command in an appropriate terminal (standard macOS/Linux shell, or Git Bash if using Windows - NOT Command Prompt or Git CMD). This is needed to ensure that your files are in the correct format. Your contributions cannot be merged properly without this.
```bash
git config --global core.autocrlf input
```

## Installing GitHub Desktop
It's possible to damage the code repositories if using the Git from the command line if you don't know what you're doing. For this reason, all team members are required to use GitHub Desktop, a graphical app which is both easier and safer to use. Download it [here](https://desktop.github.com/download/) for the appropriate platform.

> [!info]
> GitHub Desktop isn't available for Linux. If you're using Linux, you probably know what you're doing on the command line anyways, so just speak to the programming leads for some reminders and guidelines, after which you can use the command line.

## Basics of Git Version Control & Using GitHub Desktop
> [!todo]

## Git Guidelines - Rules for Git
Only specific people are allowed to make changes to the `main`/`master` branch of our Git repositories: programming mentors and programming leads. All of your work should be pushed to a branch dedicated to the specific thing you're working on. The branch should be named with your first and last initials, followed by what is being developed on the branch. For example, if you're writing a subsystem for the arm and your name is John Smith, your branch should be named `JS-ArmSubsystem`.

When the time comes to merge your changes from your branch into the `main`/`master` branch, open a Pull Request on GitHub. This will automatically prepare for your changes to be merged. A programming mentor or lead will then review your code, ensure it follows the [[Code Style Guide]], make necessary changes or provide feedback, and then merge it. Mentors and leads please note that all merges must use the "Rebase and merge" mode rather than merge commits or squashed merges to preserve commit history.

One final note: force-pushes (`git push --force`) are strictly prohibited unless you're a lead or mentor, you have backups **OUTSIDE OF GIT**, and you know *exactly* what you're doing.

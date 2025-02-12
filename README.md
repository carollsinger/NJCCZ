# Git Basics for High School Students

Welcome to **Git Basics for High School Students**! This repository is designed to introduce you to version control using Git. Whether you're completely new to Git or just need a refresher, this guide will help you learn how to use basic Git commands like **push**, **pull**, **commit**, and **checkout**.

---

## Table of Contents

- [Introduction](#introduction)
- [What is Git?](#what-is-git)
- [Getting Started](#getting-started)
- [Basic Git Commands](#basic-git-commands)
  - [git init](#git-init)
  - [git clone](#git-clone)
  - [git add](#git-add)
  - [git commit](#git-commit)
  - [git push](#git-push)
  - [git pull](#git-pull)
  - [git checkout](#git-checkout)
- [Example Workflow](#example-workflow)
- [Troubleshooting](#troubleshooting)
- [Additional Resources](#additional-resources)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

Version control is a fundamental skill for anyone working on computer projects, and **Git** is one of the most popular version control systems out there. This guide is meant for high school students and beginners, breaking down the basic Git commands and workflows to help you manage your projects and collaborate with others.

---

## What is Git?

Git is a **distributed version control system** that allows you to track changes in your code or documents over time. It enables multiple people to work on a project simultaneously without overwriting each other's changes. With Git, you can:

- **Save snapshots** of your work
- **Collaborate** with peers
- **Undo mistakes** easily

---

## Getting Started

### 1. Install Git

Before you can use Git, you need to install it on your computer. Download Git from the [official website](https://git-scm.com/downloads) and follow the installation instructions for your operating system.

### 2. Configure Git

After installing Git, set up your name and email. Open your terminal or command prompt and run:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Basic Git Commands
Let's dive into some of the core commands you'll use when working with Git.

### git init
Initializes a new Git repository in your project directory.

```bash
git init
```

### git clone
Creates a local copy of an existing repository from GitHub (or another remote).

```bash
git clone https://github.com/username/repository.git
```

### git add
Adds your changes to the staging area. Use this command to tell Git which changes you want to include in your next commit.

```bash
git add .
```
Tip: Replace . with a specific filename to add just one file (e.g., git add filename).

### git commit
Commits your staged changes to the repository with a descriptive message.

```bash
git commit -m "Your commit message"
```

### git push
Uploads your committed changes to a remote repository (e.g., GitHub).

```bash
git push origin main
```

Note: Replace main with your branch name if you’re working on a different branch.

### git pull
Fetches and merges changes from the remote repository into your current branch.

```bash
git pull origin main
```

### git checkout
Switches between branches or restores files to a previous state.

To switch to an existing branch:

```bash
git checkout branch-name
```
To create a new branch and switch to it:

```bash
git checkout -b new-branch
```

## Example Workflow
Here's a simple example to show how these commands work together:

### 1. Clone the Repository
```bash
git clone https://github.com/username/repository.git
```

### 2. Create a New Branch
```bash
git checkout -b my-feature
```

### 3. Make Changes
Edit files in your favorite text editor or IDE.

### 4. Stage Your Changes
```bash
git add .
```

### 5. Commit Your Changes
```bash
git commit -m "Add new feature"
```

### 6. Push Your Branch to GitHub
```bash
git push origin my-feature
```

### 7. Create a Pull Request on GitHub

Go to GitHub and open a pull request to merge your changes into the main branch.

---

## Troubleshooting
### Merge Conflicts:
If you encounter conflicts when pulling changes, Git will mark the conflicting parts in your files. Open the files, resolve the conflicts, stage the changes with git add, and then commit.

### Detached HEAD:
If you check out a commit instead of a branch, you might see a "detached HEAD" message. To fix this, create a new branch:

```bash
git checkout -b new-branch
```

## Additional Resources
- [Git Official Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Learn Git Branching](https://learngitbranching.js.org/)

Happy coding and enjoy learning Git!
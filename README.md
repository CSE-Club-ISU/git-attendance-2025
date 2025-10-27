# CSE Git Attendance 2025

## So we can *Git* to know you, and you can *Git* to know Git

Welcome to the CSE Club's attendance repository! This is a fun little way to get familiar with Git and GitHub while tracking attendance.

# [If you're new to Git! (CLICK ME)](#if-youre-new-to-git)

## How to Mark Your Attendance

1. [Fork and clone this repository](#forking-and-cloning-the-repository).
2. Find the folder named by the date of the meeting you're attending (e.g. `2025-09-08`).
3. Create a new file inside the folder named `<first>_<last>`
4. In the file, answer the Question of the Week listed in the folder's `README.md`.
5. [Add, commit, and push](#6-basic-git-commands) your changes to your local fork.
6. Create a pull request for us to review and merge into the main repository by clicking the "New Pull Request" button in the top
right corner of the repository.
7. Success!

## Table of Contents

- [How to Mark Your Attendance](#how-to-mark-your-attendance)
- [If you're new to Git](#if-youre-new-to-git)
  - [1. Getting a terminal](#1-getting-a-terminal)
  - [2. Installing Git](#2-installing-git)
  - [3. Forking and Cloning the Repository](#3-forking-and-cloning-the-repository)
  - [4. Authenticating with GitHub](#4-authenticating-with-github)
  - [5. Create your attendence file](#5-create-your-attendence-file)
  - [6. Basic Git Commands](#6-basic-git-commands)
  - [7. Create a Pull Request](#7-create-a-pull-request)
- [Contributing](#contributing)

## If you're new to Git

Follow these steps to setup and get the repository on your local machine. Note, there are no Linux instructions; if you're on Linux, you don't need to
follow this guide. There are also several hyperlinks to documentation to provide additional context to better your understanding throughout the process.

### 1. Getting a terminal

What is a terminal? A _terminal_ or _terminal emulator_ is a convenient text-based way to interact with a computer. Some common examples of this are Windows Command Prompt (Windows), Powershell (Windows), iTerm (macOs). A terminal allows you to do things like navigate your filesystem, edit files, manage packages, and more.

- **macOS**: macOS has several terminal options. Using the default Terminal app is fine. Another popular option is [iTerm2](https://www.iterm2.com/).
- **Windows**: Windows has a built-in terminal called [Command Prompt](https://en.wikipedia.org/wiki/Cmd.exe). You can also use Git Bash, which is bundled with Git.
> Once you have your selected terminal, open it! Any text that looks like the example below is meant to be executed in this terminal!

`example command`

### 2. Installing Git

- **macOS**: You can install Git with [Homebrew](https://brew.sh/) by running `brew install git`. Homebrew is the most popular package manager for macOS.
- **Windows**: Download and install [Git for Windows](https://git-scm.com/download/win).

### 3. Forking and Cloning the Repository

To get a copy of this project on your machine, you can ["clone"](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone) it.

1. First, you'll need to [create a GitHub account](https://github.com/join).
2. Now, create a fork of the repository on GitHub by clicking the "Fork" button in the top right corner of this page.
  > For context, this will create a copy of the repository in your own GitHub account which you can make changes to.
  > This is necessary because you don't (and shouldn't) have write access to the main repository.
3. Click the green `<> Code` button on the repository page.
4. Click on the https tab if you set up Github CLI with https (by default you will be using HTTPS).
5. Copy the clone URL.
6. In your terminal type `git clone ` and paste your URL afterwards with a space to clone the repository.

Here is an example:
```bash
git clone https://github.com/<your-github-username>/git-attendance-2025.git
```
This will create a new directory called `git-attendance-2025` in the directory you ran the command in.
In the future you might want to make a programming folder in your home directory to copy it into.

## 4. Authenticating with GitHub

Now you'll need to authenticate with GitHub.

### GitHub CLI (Simplest)

Install the [GitHub CLI](https://cli.github.com/)

Run the following command to authenticate with GitHub:

```bash
gh auth login
```

This will open a browser window where you can log in to GitHub. An example of the output is shown below.

![Github auth picture](https://github.com/tuvus/git-attendance-2025/blob/main/Docs/Screenshot%202025-10-02%20183805.png)

### Other

See official [GitHub docs](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github#authenticating-with-the-command-line) for alternate authentication methods

## 5. Create your attendence file

1. Open your file explorer (can also be named finder or dolphin).
2. Navigate to your git-attendance-2025 directory.

In Windows it it usually C:\Users\<Your_Name>\git-attendance-2025.

In Mac and Linux it is /home/<Your_Name>/git-attendence-2025.

4. Find the folder named by the date of the meeting you're attending (e.g. `2025-09-08`).
5. Create a new file inside the folder named `<first>_<last>`
6. In the file, answer the Question of the Week listed in the folder's `README.md`.

## 6. Basic Git Commands

Once you've successfully cloned the repository and made your changes (answered the QOTW!), you can use the following commands to 
push your changes to your fork and create a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

1. Navigate into your project directory

```bash
cd git-attendance-2025
```

2.  [Add your changes to the staging](https://www.atlassian.com/git/tutorials/saving-changes) area:

```bash
git add .
```
  > adds your changes in the current working directory to the staging area

2. [Commit](https://www.atlassian.com/git/tutorials/saving-changes/git-commit) your changes:

```bash
git commit -m "your commit message"
```
  > commits your changes in the staging area with the given message

3. [Push](https://www.atlassian.com/git/tutorials/syncing/git-push) your changes to your [remote](https://docs.github.com/en/get-started/git-basics/about-remote-repositories):
```bash
git push origin main
```
  > pushes the committed changes to the main branch of your fork

These three commands are Git's' bread and butter! If you're confused about any of these, please refer to the [official Git documentation](https://git-scm.com/doc). It's great!

## 7. Create a Pull Request

Now that you have pushed your changes to your repository you need to create a pull request to the CSE repository.

1. Go back to your git attendence fork at https://github.com/<your-github-username>/git-attendance-2025
2. You should see that your branch is ahead of CSE-Club-ISU/git-attendence-2025-main. Press the contribute button and open a pull request.
![Open pull request](https://github.com/tuvus/git-attendance-2025/blob/main/Docs/Screenshot_20251002_195327.png)
4. Now add a descriptive title and description in the pull request tab.
![Fill out pull request](https://github.com/tuvus/git-attendance-2025/blob/main/Docs/Screenshot_20251002_195454.png)
6. Then click create pull request to complete it.

Now the pull request has been made and needs to be merged in. Only some of the officers have merge privliges so please contact them.

## Contributing

If you encounter any issues, bugs, typos, or have any suggestions, please feel free to open an issue or submit a pull request! This is 
a great way to *Git* more Git experience and help us improve the activity. Thank you!

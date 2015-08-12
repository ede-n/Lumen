# ProGit

## Technical Jargon
* _origin_ -
* _master_ -
* _head_ -

## Cheat Sheet
* _Branching_
 * _Create_: `git branch <branchName>`
 * _Switch_: `git checkout <branchName>`
 * _Create and Switch_: `git checkout -b <branchName>`

## 1. Getting Started
### 1.6 First Time Git Setup

## 2. Basics
### 2.5 Working with Remotes

## 3. Git Branching
**Creating a new branch**
* `git branch <branchName>` This command only creates a branch, it does not switch to the branch.
* Default branch in git is called _master_. `git init` command creates it by default and can be changed.
* How does git know what branch you are currently on?
>Git maintains a special pointer called `head`.
* To see where the branch pointers are pointing use `git log --oneline --decorate --graph --all`

**Switching Branches**
* `git checkout <branchName>` switches to an existing branch. This moves `Head` to point to `branchName`.
* Switching branches changes files in your working directory.

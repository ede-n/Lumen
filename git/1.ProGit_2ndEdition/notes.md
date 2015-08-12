# ProGit

## Technical Jargon
* **origin** -
* **master** -
* **head** -
* **fast forward** - You’ll notice the phrase “fast-forward” in some merge output log. Because the commit pointed to by the branch you merged in was directly upstream of the commit you’re on, Git simply moves the pointer forward. To phrase that another way, when you try to merge one commit with a commit that can be reached by following the first commit’s history, Git simplifies things by moving the pointer forward because there is no divergent work to merge together – this is called a “fast-forward.”(See [fig 3.13][1] and [fig 3.14][2]). `master` is fast-forwarded to `hot-fix`.

## Cheat Sheet
* _Branching_
 * _Create_: `git branch <branchName>`
 * _Switch_: `git checkout <branchName>`
 * _Create and Switch_: `git checkout -b <branchName>`
 * _Delete_: `git branch -d <branchName>`
* _Merging_
  * `git checkout <branchToMergeInto> && git merge <branchName>`


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
* Switches to an existing branch(moves `Head` to point to `branchName`).
> `git checkout <branchName>`
* Switching branches changes files in your working directory.

**Merging**
* Workflow
  * Switch to the branch you want to merge into.
  >`git checkout <master>`
  * Merge
  >`git merge <branchToBeMerged>`
  * Delete branch, if it is not needed.
  >`git branch -d <branchName>`


[1]: https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
[2]: https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

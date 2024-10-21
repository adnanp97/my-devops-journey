# Git notes

What is Git?
- A distrubted version control system (VCS) that enables multiple users to collaboarate on projects, tracking changes in files and directories while proviidng a history of snapshots and the ability to manage different branches and merge code changes efficiently.
(Tracking and managing changes in software projects, contains details history on code changes)

Why is Git important?
- For collaboration and managing code efficiently: work simulatenously on branches, develop new features, fix bugs, experiment new ideas

What is a README and what is the importance of one?
- Cruicial document that provides an overview of your project, it's purpose and how to use it.
- useful for those new to the project to understand the goals and functionality
- first point of reference for users and contributors, helping in understanding the project structure, how to get started and guidelines for contributing
- How to set up development environments
- written in markdown format for easy formatting and readability

Git workflow

- Git clone copies remote repo to local repo
- local repo has a working directory 
- then placed in staging area (Git add .)
- then Git commit
- then push it to git (Git push pushes it to remote repo)
- update local using git pull (makes sure you have the upto date version)
- history (shows your previous commands)

  
![Screenshot 2024-10-02 at 22 31 47](https://github.com/user-attachments/assets/6aa3f09a-dfca-4a9e-a194-0ac439d03026)

git status : shows you your branch and see changes to be committed and modified



commits
prupose?
- provide code quality and enables feedback in merge requests.
- allows detailed record, changes, when and by who
- describe changes and reasons (helps everyone understand purpose of each change)
- creates audit trail, easy to understand
- documents changes, making history robust
- easier to track modification, makes trouble shooting easier

Good commit practices
- commit often (capture incremental progress of work and track changes)
- write clear messages (descriptive and explain the change which was made)
- use command style messages (e.g. fix bug not fixed bug)
- test code before committing
- avoid committing generated file (can use git ignore)
- break down large changes into smaller commits
- use tickets/issues (easier to know what commit is directly link to)

Branching
Pros of Branching
- allows developers to work on different features simultaneously without affect prod environment
- each feature developed in its own branch, easier to test
- isolate deveoplemnt (doesn't interefere with ongoing work)
- allows experiment new ideas
- test new functionalities then merge into main branch (only stable and tested features will be integrated)
- can make dedicated branch for bug fix (focused trouble shooting)
- git checkout branch name (to switch to branch)

Purpose of branching?


Simple branch workflow
![Screenshot 2024-10-02 at 23 02 51](https://github.com/user-attachments/assets/83750113-e4bf-4f2e-9fe9-3053938c7dfa)

complex workflow
![Screenshot 2024-10-02 at 23 05 12](https://github.com/user-attachments/assets/4bdd8f6c-436c-4c6a-a2a7-85ee3dc2665d)


Pull requests
purpose?
- allows team members to review code changes before they get merged into the main branch
- keeps a detail of all changes and discussions (can see history and context of changes)
- providing important info into each modification

Doubts: don't fully understand how pull requests guarantees the above, I thought it was only for pulling main branch to local repo.


Merge conflicts
- make sure to do git pull to avoid this as you will be working on an old version of a code leading to conflicts
- happens when git cannot reconcile differences between two commits and needs manual resolution
- 

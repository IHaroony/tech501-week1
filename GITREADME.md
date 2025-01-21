# Git Learning README 
- This README document will contain what i have learned about git today and it will explain my understanding of it 

## What is Git?

1. Git is a tool that helps track changes in files, especially code files. It’s mainly used by developers to manage projects and keep a history of all changes.

    * Git is a version control system, which means it keeps track of every change made to files in a project.

    * It helps manage changes so you can go back to previous versions if needed.

    * Developers use Git to collaborate on projects without interfering with each other’s work.



    ## What are Repositories?


A repository (or repo) is like a folder where Git tracks changes to your files. There are two main types of repositories:

- **Local Repository**: This is the repository on your computer.
- **Remote Repository**: This is the repository stored on a platform like GitHub so others can access it.

A repository is where all your project’s files and the history of changes are stored.

<BR>

## The 3 Stages of Git
Git has three main stages that files go through:

1. **Working Directory**:
   - This is where you make changes to your files. Any new or edited files are in this stage.
   - Command: `git status` helps you check what’s happening in your working directory.

2. **Staging Area**:
   - Before committing, you can prepare files by adding them to the staging area. It’s like saying, “These are the changes I want to save.”
   - Command: `git add <file>` adds a file to the staging area. To add all files, you can use `git add .`.

3. **Repository (Committed State)**:
   - When you commit, your changes are saved permanently in the Git repository.
   - Command: `git commit -m "Your message"` saves the staged changes with a description.



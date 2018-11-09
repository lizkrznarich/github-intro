# github-intro
Intro to Git + Github workshop materials

## Slides

[https://lizkrznarich.github.io/github-intro/slides](https://lizkrznarich.github.io/github-intro/slides)

## Tutorial
### Create a GitHub account
1. Sign up at [https://github.com](https://github.com)
### Create a new repository
1. Follow steps 1-6 in [https://help.github.com/articles/create-a-repo](https://help.github.com/articles/create-a-repo)
### Set up Git
1. Download and install Git [https://git-scm.com/downloads](https://git-scm.com/downloads)

2. Check that Git is installed

        git --version

3. Add your name

        git config --global user.name "YOUR NAME"

4. And the email attached to your GitHub account

        git config --global user.email "YOUR EMAIL"

### Clone your repo locally
    git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
### Making changes
1. Change directory into your local repo

        cd YOUR-REPOSITORY

2. Edit README.md and save the changes

        vim README.md

3. Check to see what changes Git has noticed
        
        git status

4. Add changed files to the Index

        git add README.md

5. Added something you didn't intend to? Remove the file from the index

        git reset README.md

6. Commit your changes

        git commit -m "added README file"

7. Push your changes to your remote repository

        git push origin master
        
### Reverting changes
### Branching
### Merging

## Handout
https://education.github.com/git-cheat-sheet-education.pdf



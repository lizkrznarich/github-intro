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

### Clone your repo
1. Clone your repo to your local machine

        git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY

2. Change directory into your local repo

        cd YOUR-REPOSITORY
3. What's in there?

        ls -la

### Making changes
2. Edit README.md and save the changes

        vim README.md

3. Check to see what changes Git has noticed
        
        git status
        On branch master
        Your branch is up-to-date with 'origin/master'.
        Changes not staged for commit:
          (use "git add ..." to update what will be committed)
          (use "git checkout -- ..." to discard changes in working directory)

    modified:   README.md

4. Add changed files to the Index

        git add README.md

5. Added something you didn't intend to? Remove the file from the index

        git reset README.md

6. Commit your changes

        git commit -m "added README file"

7. Push your changes to your remote repository

        git push origin master

### Reverting changes
1. Show a list of recent commits

        git log
        commit 9abfae533f4fcd5c2e68ac4e5eb4179a452532cc
        Author: Liz Krznarich 
        Date:   Thu Nov 8 20:05:20 2018 -0600

            this was a terrible idea

        commit 603c619cf90dd9520c141d65d0f3697973bc9a8d
        Author: Liz Krznarich 
        Date:   Thu Nov 8 19:02:52 2018 -0600

            Initial commit

2. Revert to a specific commit

        git reset 603c619cf90dd9520c141d65d0f3697973bc9a8d

3. Things gone terribly wrong? Reset local to match remote

        git reset --hard origin master

### Branching
1. Create a new local branch

        git checkout -b new-branch-name

2. Make and commit some changes

        vim README.md
        git add README.md
        git commit -m "editing that readme again"

3. Push your local changes to a new branch in your remote repo

        git push origin new-branch-name

### Merging
1. Open a Pull Request [https://help.github.com/articles/about-pull-requests](https://help.github.com/articles/about-pull-requests)
2. Merge a Pull Request [https://help.github.com/articles/merging-a-pull-request](https://help.github.com/articles/merging-a-pull-request/)

### Syncing
1. Switch to the master branch
        
        git checkout master

2. Pull the latest code from the remote repo

        git pull origin

## Handout
https://education.github.com/git-cheat-sheet-education.pdf



<!SLIDE title-slide>

# Understanding Git
## An introduction

<!SLIDE small incremental transition=fade>
.notes Use command line to demonstrate

# Getting Started

* Repository setup
  - Create new Git repository: `git init`
  - Copy an existing Git repository: `git clone`
  - Configure Git installation: `git config`
* Saving changes
  - Track / add file to staging area: `git add`
  - Add staged snapshot to project history: `git commit`
* Inspecting a repository
  - Display state of working directory and staging area: `git status`
  - List project history: `git log`

<!SLIDE small transition=turnUp>

* Undoing changes
  - Undo a commit, generating a new commit: `git revert`
  - Remove file/commit: `git reset`
  - Remove untracked files: `git clean`
* Collaborating
  - Manage repositories: `git remote`
  - Import remote commits: `git fetch`
  - Import and integrate remote repository: `git pull`
  - Update remote repository: `git push`
* Using branches
  - Manage branches: `git branch`
  - Switch branch / Restore file: `git checkout`
  - Join histories: `git merge`
  - Move branch to new base commit: `git rebase`


<!SLIDE supplemental exercises>
# Exercise ~~~SECTION:MAJOR~~~.~~~SECTION:MINOR~~~: Getting started Exercise

## Objective: Create a new Git repository and populate with sample files

    @@@ bash
    git init
    echo "Test" > sample.txt
    git add sample.txt
    git commit -m "Initial commit."

## Objective: Start a new feature branch and add a sample file

    @@@ bash
    git checkout -b new-feature master
    git add new-feature-file.txt
    git commit -m "Added new feature file."

## Objective: Merge in the new feature branch

    @@@ bash
    git checkout master
    git merge new-feature
    git branch -d new-feature

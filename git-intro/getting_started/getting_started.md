<!SLIDE title-slide>

# Understanding Git
## An introduction

<!SLIDE small incremental transition=fade>
.notes Use command line to demonstrate

# Getting Started

* Repository setup
  - git init
  - git clone
  - git config
* Saving changes
  - git add
  - git commit
* Inspecting a repository
  - git status
  - git log

<!SLIDE small transition=turnUp>

* Undoing changes
  - git revert
  - git reset
  - git clean
* Collaborating
  - git remote
  - git fetch
  - git pull
  - git push
* Using branches 
  - git branch
  - git checkout
  - git merge | rebase  


<!SLIDE supplemental exercises>
# Exercise ~~~SECTION:MAJOR~~~.~~~SECTION:MINOR~~~: Getting started Exercise
## Objective: Create a new Git repository and populate with sample files

    git init
    echo "Test" > sample.txt
    git add sample.txt
    git commit -m "Initial commit."

## Objective: Start a new feature branch and add a sample file

    git checkout -b new-feature master
    git add new-feature-file.txt
    git commit -m "Added new feature file."

## Objective: Merge in the new feature branch

    git checkout master
    git merge new-feature
    git branch -d new-feature

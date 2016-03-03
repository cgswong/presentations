<!SLIDE bullet incremental smaller transition=fade>

# Some Guides

* Use **[rebase](https://www.atlassian.com/git/images/articles/simple-git-workflow-is-simple/rebase-on-feature.gif)** for local copy to stay current with remote upstream

* Use **merge** to combine finalized branches (for example **master** and “**feature**”)

* Use dependency management tool to handle project dependencies
  - Maven, npm

* Leverage Git hooks
  - Executable scripts in .git/hooks
  - Implement commit policy / template
  - Continuous Integration and/or Continuous Deployment workflows
  - Notifications

* Ignore files / paths using .gitignore

<!SLIDE supplemental exercises>
# Exercise ~~~SECTION:MAJOR~~~.~~~SECTION:MINOR~~~: Rebase and Merge Exercise
## Objective: Test doing a rebase on your local branch

    @@@ bash
    git fetch origin
    git rebase origin/master
    git log

## Objective: Test doing a merge onto your master branch from a created feature branch

    @@@ bash
    git checkout master
    git pull origin master
    git merge new-feature
    git log


~~~SECTION:handouts~~~

A merge is the simplest method and should be used until rebase is better understood. A merge is perfectly acceptable in most cases with a rebase being introduced to provide better historical ordering and tracking of work done on the master relevant to your branch (i.e. cleaner project history). Note that a rebase should never be done directly on public branches as doing so disrupts work being doing by collaborators.

~~~ENDSECTION~~~

<!SLIDE bullet small transition=fade>

# Git Platform Features

* **Issues:** Lightweight issue tracking
  - Create issues/tasks and assignments
  - Milestones
  - Labels
* **Merge Requests:** Review and discuss code before merge
  - Assign to issues, people, referenced
  - Attach milestones
* **Wiki:** Separate system for documentation
  - Alternative to keeping in code (`/docs`)
* **Snippets:** Bits of code or text
  - Small bits of regularly referenced text/code
  - Too small for full repo
* **Groups:** Group projects into directories and give users access to several projects at once


~~~SECTION:notes~~~

This section is not specific to GitLab or GitHub but holds true generally for most, if not all, Web UIs for Git.

It is a team choice as to using the Issues functionality if an existing ticketing system is already in place. Ideally they should be linked but regardless the GitLab Issue function can be used in conjunction with an existing system to ensure issues are tracked within the same tool and make better usage of the Merge Requests function.

In our OSS GitLab implementation groups are not LDAP based. Also, authentication outside of the main domain is done via local account as the implementation does not support a multi-domain LDAP setup.

Currently, GitHub is the preferred option though certain challenges remain, notable around account provisioning.

~~~ENDSECTION~~~

<!SLIDE bullet small transition=fade>

# Git Platform Features

* **Issues:** Lightweight issue tracking
  - Make tickets and assignments
  - Milestones
  - Labels
* **Merge Requests:** Review and discuss code before merge
  - Assign to issues, people, referenced
  - Attach milestones
* **Wiki:** Separate system for documentation
  - Alternative to keeping in code
* **Snippets:** Bits of code or text
  - Text referenced regularly but does not belong in source control
* **Groups:** Group projects into directories and give users access to several projects at once


~~~SECTION:notes~~~

This section is not specific to GitLab but holds true generally for most, if not all, Web UIs for Git.

It is a team choice as to using the Issues functionality if an existing ticketing system is already in place. Ideally they should be linked but regardless the GitLab Issue function can be used in conjunction with an existing system to ensure issues are tracked within the same tool and make better usage of the Merge Requests function.

In our OSS GitLab implementation groups are not LDAP based. Also, authentication outside of the main domain is done via local account as the implemetnation does not support a multi-domain LDAP setup.

~~~ENDSECTION~~~

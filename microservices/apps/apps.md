<!SLIDE bullet small transition=fade>

# Designing Microservice Applications

* **Keep Code at a Similar Level of Maturity**
  - immutable infrastructure
  - if you need to add or rewrite some of the code in a deployed microservice that’s working well, create a new microservice for the new or changed code, leaving the existing microservice in place.
  - iteratively deploy and test the new code until it is bug free and maximally efficient, without risking failure or performance degradation in the existing microservice

* **Do a separate build for each microservice**
  - pull in component files from the repository at the revision levels appropriate to it
  - sometimes leads to various microservices pull in a similar set of files, but at different revision levels

* **Deploy in containers**
  - just need just one tool to deploy everything

~~~SECTION:notes~~~

* Separate builds can make it more difficult to clean up your codebase by decommissioning old file versions because you have to verify more carefully that a revision is no longer being used, but that’s an acceptable trade-off for how easy it is to add new files as you build new microservices.

~~~ENDSECTION~~~

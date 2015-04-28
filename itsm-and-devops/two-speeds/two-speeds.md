<!SLIDE bullet small transition=fade>

# Two Speeds

* **Only two speeds?**
- Model driven
- Emergent

* **All changes lead to CM change**
  - Configuration Management change triggered by Service Registry reconfiguration
  - All changes tracked centrally
  - Performance issues?

~~~SECTION:notes~~~

* Example of CM triggered by SR change is a consul change, such as adding new web server, triggering a Puppet run to update proxy server configuration.

* CM runs are typically scheduled so quick change are not possible. On-demand is an option (automated into workflow) but may also pose a challenge due to frequency of runs.

~~~ENDSECTION~~~

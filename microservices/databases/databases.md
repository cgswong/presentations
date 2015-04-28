<!SLIDE bullet small transition=fade>

# Designing Microservice databases

* **Create a separate data store for each microservice**
  - The team for each microservice should choose the database that best suits the service.
  - May seem reasonable to share (reducing duplication of work), but if one team updates a database structure, other services that also use that structure have to be changed


* **Use Master Data Management (MDM)**
  - Breaking apart data can make data management more complicated
    - separate storage systems can more easily get out sync
    - foreign keys can change unexpectedly
  - a tool that performs master data management (MDM) operates in the background to find and fix inconsistencies
  - Write your own tool or buy one


~~~SECTION:notes~~~

* An MDM tool will, for example, examine every database that stores customer IDs, to verify that the same IDs exist in all of them (there are not missing or extra IDs in any one database).

* In terms of COTS offerings, many commercial relational database management systems (RDBMSs) usually impose too many requirements for coupling, and so don’t scale.

~~~ENDSECTION~~~

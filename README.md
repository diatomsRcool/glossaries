glossaries
--------------------

Contribution
----------
If you want to contribute, you can do so by 
* using OTO, which populates this repository programmatically
* Manually update the repository following the conventions outlined below

The glossaries are stored as CSV in a directory structure where
* The first level directory name specifies the `glossary type`
* The second level directory name specifies the `glossary version`
* The second level directory contains the `term_category` and `syns` glossary files. These are to be named as:
  * `glossary type`_glossary_term_category.csv
  * `glossary type`_glossary_syns.csv
* A latest directory must exist on the second level with a duplicate of the files of the latest version

If you create a new `term_category` please follow the following schema, where the `glossary version` and `glossary type` are required. All lines are required, and hence line number 10 would contain the first data.
```
#Version: `glossary version`
#Glossary type: `glossary type`
#Source: 
#Finalized by: 
#Date:
#Reviewers: 
#Source producer: 

"term","category","hasSyn","sourceDataset","termID"
"my term", "my category", "0", "my source dataset", "some id"
...
```

Likewise for `syns`
```
#Version: `glossary version`
#Glossary type: `glossary type`
#Source: 
#Finalized by: 
#Date:
#Reviewers: 
#Source producer: 

"term","category","synonym","termID"
"my term", "my category", "my synonym", "some id"
...
```



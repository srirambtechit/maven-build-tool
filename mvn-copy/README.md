# Maven Project for copying dependencies of JARs

It is a special eclipse project designed for copying dependent
JARs of projects. 

## How to use this project
1. Add dependency details in `<dependencies>`
2. Then run the pom.xml as explained as stated below

## How to run in eclipse

1. Configuration:
..* Right click on __pom.xml__ 
....* -> Run As 
....* -> Run configurations... 
....* -> Define goal as __dependency:copy-dependencies__
....* -> add parameter in below settings by click Add
....* -> param name is __outputDirectory__
....* -> param value is __lib__
2. Execute pom.xml
Right click on __pom.xml__
    -> Run As
    -> Maven build
3. __lib__ folder will be created and dependencies were generated


1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

## Command line usage
`mvn -DoutputDirectory=alternativeLocation dependency:copy-dependencies` 
# Maven Project for copying dependencies of JARs

It is a special eclipse project designed for copying dependent
JARs of projects. 

## How to use this project
1. Add dependency details in `<dependencies>`
2. Then run the pom.xml as explained as stated below

## How to run in eclipse

1) Configuration:<br/>
Right click on __pom.xml__ <br/> 
    -> Run As <br/>
    -> Run configurations...<br/> 
    -> Define goal as __dependency:copy-dependencies__<br/>
    -> add parameter in below settings by click Add<br/>
    -> param name is __outputDirectory__<br/>
    -> param value is __lib__<br/>
2) Execute pom.xml<br/>
Right click on __pom.xml__<br/>
    -> Run As<br/>
    -> Maven build<br/>
3) __lib__ folder will be created and dependencies were generated<br/>


## Command line usage
`mvn -DoutputDirectory=alternativeLocation dependency:copy-dependencies` 
## Simple project using Spring MVC (using annotation), hsqldb, maven application

## Installation

#### Build project and import into Eclipse

```
$mvn clean package
```

Then import to your favourite IDE (mine is Eclipse)

```
$mvn eclipse:eclipse
```

then from Eclipse, File->Import

#### Build and deploy using Maven to Apache Tomcat

To actually run it just use the supplied script

```
build-and-deploy.sh
```
Start Tomcat, then point your browser to [http://localhost:8080/springmvc-hsqldb-hibernate-example/](http://localhost:8080/springmvc-hsqldb-hibernate-example/)

    #!/bin/bash
    mvn clean package
    # NOTE: edit this to suite your deployment environment
    export DEPLOYMENT_DIR=$TOMCAT_HOME/webapps
    cp target/springmvc-hsqldb-hibernate-example.war $DEPLOYMENT_DIR

## Author

[Burin Choomnuan](https://github.com/agilecoders)
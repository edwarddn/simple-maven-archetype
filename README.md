# Simple maven archetype

## Summary
The project is a Maven archetype for Java console application.

## Prerequisites

- JDK 17 (tested with Java 17)
- Maven 3 (tested with 3.8.5)

## Create a project

```bash
  mvn archetype:generate \
    -DarchetypeGroupId=br.com.edward.archetypes \
    -DarchetypeArtifactId=simple-maven-archetype \
    -DarchetypeVersion=1.0.0 \
    -DgroupId=br.com.myname.myproject \
    -DartifactId=my-project-name \
    -Dversion=0.0.1-SNAPSHOT \
    -DarchetypeRepository=http://edwarddn.github.io/simple-maven-archetype
```

Note: The above command will bootstrap a project using the archetype published here: http://edwarddn.github.io/simple-maven-archetype

## Create a new project in IntelliJ

* Create new project `File > New > Project`
* Click Maven on the left hand side of the new project dialog
* Check `Create from archetype`
* Click the `Add Archetype` button
* Set `Group Id` to `br.com.edward.archetypes`
* Set `Artifact Id` to `simple-maven-archetype`
* Set `Version` to `1.0.0`
* Set `Repository` to `http://edwarddn.github.io/simple-maven-archetype`
* Click next and create the project

Note: If you would like to create a project using archetype published in your local repository, skip repository field and make sure it is installed locally (see below).

## Install archetype locally

To install the archetype in your local repository execute the following commands:

```bash
  git clone git@github.com:edwarddn/simple-maven-archetype.git
  cd simple-maven-archetype
  mvn clean install
```

## Create a project from a local repository

Create a new empty directory for your project and navigate into it and then run:

```bash
  mvn archetype:generate \
    -DarchetypeGroupId=br.com.edward.archetypes \
    -DarchetypeArtifactId=simple-maven-archetype \
    -DarchetypeVersion=1.0.0 \
    -DgroupId=br.com.myname.myproject \
    -DartifactId=my-project-name \
    -Dversion=0.0.1-SNAPSHOT
```
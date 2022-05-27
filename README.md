Simple maven archetype
======================================

Summary
-------
The project is a Maven archetype for Java console application.

Prerequisites
-------------

- JDK 17 (tested with Java 17)
- Maven 3 (tested with 3.8.5)

Install archetype locally
-------------------------

To install the archetype in your local repository execute the following commands:

```bash
  git clone git@github.com:edwarddn/simple-maven-archetype.git
  cd simple-maven-archetype
  mvn clean install
```

Create a project from a local repository
----------------------------------------

Create a new empty directory for your project and navigate into it and then run:

```bash
  mkdir my-project-name
  cd my-project-name
  mvn archetype:generate \
    -DarchetypeGroupId=br.com.edward.archetypes \
    -DarchetypeArtifactId=simple-maven-archetype \
    -DarchetypeVersion=1.0.0 \
    -DgroupId=br.com.myname.myproject \
    -DartifactId=my-project-name \
    -Dversion=0.0.1-SNAPSHOT
```
# rest-api-java-jersey

Minimalistic RESTful Web Services in *Java*(*Jersey*)

## Direct ancestors

Absent

## Direct descendants

Yet absent

## Requirements

* [*Java 7*](https://www.oracle.com/technetwork/java/javase/downloads/java-archive-downloads-javase7-521261.html)
* [*Jersey 2.x*](https://jersey.github.io/)
* [*Apache Maven*](https://maven.apache.org/)

Оther dependencies are transitive and therefore installed under the hood.

## Code generation

All code of this repository is generated.
To create a source code for Servlet container deployable *Jersey 2.28* web-service,
use

```sh
mvn archetype:generate -DarchetypeGroupId=org.glassfish.jersey.archetypes -DarchetypeArtifactId=jersey-quickstart-webapp -DarchetypeVersion=2.28
```

After several questions and relevant answers, the source code of the web
service will be generated.

## Build

Being in the just generated web-service directory, run:

```sh
mvn clean install
```

As a result, a distribution *war*-file will be obtained.

## Installation

The *war* distribution then should be deployed on any *Java* servlet
container: *Tomcat*, *Jetty*, ...

## Running

The service can be tested from the browser by typing the corresponding URL
(depends on the servlet container specific) in its address bar.

## Authors

[Alexander Lapygin](https://github.com/AlexanderLapygin)

## Inspired by

[*Jersey 2.28* mvn archetype generation](https://jersey.github.io/download.html)

### License

Licensed under the [MIT license](./LICENSE). 

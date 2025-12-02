---

title: 'Apache Maven Coordinates'
weight: 13

menu:
  main:
    name: "Maven Coordinates"
    identifier: "get-started-maven"
    pre: "The most commonly used Apache Maven Coordinates for CadenzaFlow."

---

This page lists the most commonly used Apache Maven Coordinates for CadenzaFlow.

Most CadenzaFlow artifacts are pushed to [maven central](https://central.sonatype.com/).


# CadenzaFlow BOM (Bill of Materials)

## Community Edition

```xml
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>org.cadenzaflow.bpm</groupId>
      <artifactId>cadenzaflow-bom</artifactId>
      <version>1.0.1</version>
      <scope>import</scope>
      <type>pom</type>
    </dependency>
  </dependencies>
</dependencyManagement>
```


# CadenzaFlow Engine

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm</groupId>
  <artifactId>cadenzaflow-engine</artifactId>
</dependency>
```


# CadenzaFlow Engine Spring Integration

The `cadenzaflow-engine` Spring integration for Spring Framework 5:

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm</groupId>
  <artifactId>cadenzaflow-engine-spring</artifactId>
</dependency>
```

The `cadenzaflow-engine` Spring integration for Spring Framework 6:

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm</groupId>
  <artifactId>cadenzaflow-engine-spring-6</artifactId>
</dependency>
```

# CadenzaFlow Engine CDI Integration

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm</groupId>
  <artifactId>cadenzaflow-engine-cdi</artifactId>
</dependency>
```

# CadenzaFlow DMN Engine BOM (Bill of Materials)
This BOM allows to use the DMN engine standalone without the BPMN engine and the rest of the CadenzaFlow Platform.

```xml
<dependencyManagement>
  <dependency>
    <groupId>org.cadenzaflow.bpm.dmn</groupId>
    <artifactId>cadenzaflow-engine-dmn-bom</artifactId>
    <version>1.0.1</version>
    <type>pom</type>
    <scope>import</scope>
  </dependency>
</dependencyManagement>
```

# CadenzaFlow DMN
This dependency allows to use DMN engine standalone without the BPMN engine and the rest of the CadenzaFlow Platform.
It is not needed when using `cadenzaflow-engine` because that already contains the DMN engine.

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm.dmn</groupId>
  <artifactId>cadenzaflow-engine-dmn</artifactId>
</dependency>
```

# Process Application EJB Client

```xml
<dependency>
  <groupId>org.cadenzaflow.bpm.javaee</groupId>
  <artifactId>cadenzaflow-ejb-client</artifactId>
</dependency>
```

# CadenzaFlow Artifact Storage

## Artifactory

CadenzaFlow relies on Nexus Artifactory to provide CadenzaFlow artifacts to users at [nexus.cadenzaflow.com](https://nexus.cadenzaflow.com/). The artifact data is stored in [Amazon S3](https://aws.amazon.com/s3/) storage and gets served by [nexus.cadenzaflow.com](https://nexus.cadenzaflow.com/) via redirects to AWS S3. Users must be able to connect to both endpoints for artifact retrieval.

### Community Edition

```xml
<repositories>
  <repository>
    <id>cadenzaflow-bpm-nexus</id>
    <name>cadenzaflow-bpm-nexus</name>
    <url>
        https://nexus.cadenzaflow.com/repository/cadenzaflow-nexus/
    </url>
  </repository>
</repositories>
```


### Browse CadenzaFlow Artifact Storage
In order to browse the CadenzaFlow artifacts, here are the links which you can use.

#### Community Edition
This link helps you to browse the artifacts of CadenzaFlow Platform community edition.

https://nexus.cadenzaflow.com/service/rest/repository/browse/cadenzaflow-nexus/org/cadenzaflow/bpm/


### Known issues

#### cURL artifacts
The files are hosted in AWS S3, therefore, Artifactory rewrites the requests to S3 and sends a 302 as the first response. For cURL this means to add the "`-L`" or "`--location`" option to follow the response.

Example:
```
curl -LO http://nexus.cadenzaflow.com:443/repository/cadenzaflow-nexus/org/cadenzaflow/bpm/cadenzaflow-engine-rest/1.0.1/cadenzaflow-engine-rest-1.0.1.war
```

# Other CadenzaFlow Modules:

* [DMN Engine](/manual/latest/user-guide/dmn-engine/embed/#maven-coordinates)
* [CadenzaFlow Spin](/manual/latest/reference/spin)
* [CadenzaFlow Connect](/manual/latest/reference/connect/#maven-coordinates)
* [Templating Engines](/manual/latest/user-guide/process-engine/templating/#install-a-template-engine-for-an-embedded-process-engine)
* [Spring Boot Integration](/manual/latest/user-guide/spring-boot-integration/)

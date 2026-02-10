---
title: "Security Notices v1.1.0"
weight: 70

menu:
  main:
    name: "Security Notices v1.1.0"
    parent: "security-notices"
    identifier: "notices-v110"
    pre: "Security Notices v1.1.0"
---


# Notices CadenzaFlow v1.1.0
Since CadenzaFlow v1.1.0 is forked from Camunda 7.24 community edition, this section lists related security notices keeping the original notice numbering (from Camunda) the same inherited from Camunda 7.24

Please note that since Cawemo and Optimize are NOT continued by Cadenzaflow (alternatives to be provided as part of roadmap), here below only the related notices for continued capabilities will be listed.

For further details specific to notices on Camunda, please refer to [Camunda Docs/Security](https://docs.camunda.org/security/).


## Notice 145

**Publication Date: September 1st, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of spring-webmvc shipped with Camunda 7 Run was affected by the following vulnerability:

 - https://nvd.nist.gov/vuln/detail/CVE-2025-41242

**How to determine if the installation is affected**

You disabled security features in the production.yml configuration AND you use the following Camunda Run versions or lower: 7.23.4, 7.22.7, 7.21.12.

**Solution**

Camunda has provided the following releases, which contain a fix:

Camunda 7.23.5, 7.22.8, 7.21.13.


## Notice 141

**Publication Date: July 30th, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of Tomcat shipped with the Camunda 7 Tomcat and Run Docker Images was affected by the following vulnerability:

- https://nvd.nist.gov/vuln/detail/CVE-2025-53506

**How to determine if the installation is affected**

* You use the Camunda 7 Tomcat or Run Docker images **AND** you enabled HTTP2 in your Tomcat configuration.
* You use the following Camunda 7 versions or lower: 7.24.0-alpha1, 7.23.3, 7.22.6, 7.21.11.

**Solution**

Camunda has provided the following releases, which contain a fix:

Camunda 7.24.0-alpha2, 7.23.4, 7.22.7, 7.21.12.

## Notice 140

**Publication Date: July 30th, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of Tomcat shipped with the Camunda 7 Tomcat and Run Docker Images was affected by the following vulnerability:

- https://nvd.nist.gov/vuln/detail/CVE-2025-48988

**How to determine if the installation is affected**

* You use the Camunda 7 Tomcat or Run Docker images.
* You use the following Camunda 7 versions or lower: 7.24.0-alpha1, 7.23.2, 7.22.5, 7.21.10.

**Solution**

Camunda has provided the following releases, which contain a fix:

7.24.0-alpha2, 7.23.3, 7.22.6, 7.21.11.


## Other Notices

Notices inherited/related/fixed from Camunda 7.22 and earlier versions already detailed on [Camunda Docs/Security](https://docs.camunda.org/security/) and will NOT be repeated here.


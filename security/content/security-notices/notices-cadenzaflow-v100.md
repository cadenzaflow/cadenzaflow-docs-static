---
title: "Security Notices v1.0.0"
weight: 70

menu:
  main:
    name: "Security Notices v1.0.0"
    parent: "security-notices"
    identifier: "notices-v100"
    pre: "Security Notices v1.0.0"
---


# Notices CadenzaFlow v1.0.0
Since CadenzaFlow v1.0.0 is forked from Camunda 7.24 community edition, this section lists related security notices keeping the original notice numbering (from Camunda) the same inherited from Camunda 7.24

Please note that since Cawemo and Optimize are NOT continued by Cadenzaflow (alternatives to be provided as part of roadmap), herebelow only the related notices for continued capabilities will be listed.

For further details specific to notices on Camunda, please refer to [Camunda Docs/Security](https://docs.camunda.org/security/).


## Notice 133

**Publication Date: April 9th, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of Spring Security shipped with Camunda 7 Run was affected by the following vulnerability:

- https://nvd.nist.gov/vuln/detail/CVE-2025-22228

**How to determine if the installation is affected**

* You use Camunda 7 Run with the `--oauth2` flag on startup.
  * E.g., `./start.sh --webapps --rest --oauth2`
* You use the following Camunda 7 versions or lower: 7.22.3, 7.23.0-alpha4

**Solution**

Camunda has provided the following releases, which contain a fix:

Camunda 7.22.4, 7.23.0



## Notice 130

**Publication Date: March 10th, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of Tomcat shipped with the Camunda 7 Tomcat and Run Docker Images was affected by the following vulnerabilities:

- https://nvd.nist.gov/vuln/detail/CVE-2024-56337
- https://nvd.nist.gov/vuln/detail/CVE-2024-50379

**How to determine if the installation is affected**

* You use the Camunda 7 Tomcat or Run Docker images.
* You use the following Camunda 7 versions or lower: 7.20.10, 7.21.7, 7.22.2, 7.23.0-alpha3

**Solution**

Camunda has provided the following releases, which contain a fix:

Camunda 7.20.11, 7.21.8, 7.22.3, 7.23.0-alpha4

## Notice 129

**Publication Date: March 10th, 2025**

**Product affected:**

Camunda 7

**Impact:**

The version of `DOMPurify` shipped with the Camunda 7 Webapps was affected by the following vulnerabilities:

- https://nvd.nist.gov/vuln/detail/CVE-2024-45801
- https://nvd.nist.gov/vuln/detail/CVE-2024-47875

**How to determine if the installation is affected**

* You use the Camunda 7 Webapps.
* You use the following Camunda 7 versions or lower: 7.20.10, 7.21.7, 7.22.2, 7.23.0-alpha3

**Solution**

Camunda has provided the following releases, which contain a fix:

Camunda 7.20.11, 7.21.8, 7.22.3, 7.23.0-alpha4



## Notice 124

**Publication Date: December 10th, 2024**

**Product affected:**

Camunda 7

**Impact:**

The version of Bootstrap, included in the Camunda web applications, had Cross-Site-Scripting (XSS) vulnerabilities:

- https://nvd.nist.gov/vuln/detail/CVE-2024-6484
- https://nvd.nist.gov/vuln/detail/CVE-2024-6485
- https://nvd.nist.gov/vuln/detail/CVE-2024-6531

**How to determine if the installation is affected**

- You use the Camunda 7 web applications.
- You use a custom plugin that utilizes the following components of Bootstrap:
  - Carousel component where the attributes `data-slide` and `data-slide-to` can be exploited through the `href` attribute.
  - Button compenent which can be exploited through the `data-loading-text` attribute.
- An attacker can provide forged input to the custom plugin that passes it to the `href` or `data-loading-text` attributes.

**Solution**

Camunda has provided the following releases which contain a fix:
Camunda 7.20.9, 7.21.6, 7.22.1, 7.23.0-alpha2.

## Notice 123

**Publication Date: December 10th, 2024**

**Product affected:**

Camunda 7

**Impact:**

The version of AngularJS, included in the Camunda web applications, had two content spoofing vulnerabilities:

- https://nvd.nist.gov/vuln/detail/CVE-2024-8372
- https://nvd.nist.gov/vuln/detail/CVE-2024-8373

**How to determine if the installation is affected**

- You use the Camunda 7 web applications.
- You use a custom plugin that utilizes the `<source>` HTML tag or the AngularJS `ng-srcset` directive.
- An attacker can provide forged input to the custom plugin that passes it to the `<source>` HTML tag or the `ng-srcset` directive.

**Solution**

Camunda has provided the following releases which contain a fix:
Camunda 7.20.9, 7.21.6, 7.22.1, 7.23.0-alpha2.

## Other Notices

Notices inherited/related/fixed from Camunda 7.22 and earlier versions already detailed on [Camunda Docs/Security](https://docs.camunda.org/security/) and will NOT be repeated here.


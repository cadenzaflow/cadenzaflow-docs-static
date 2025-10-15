---

title: 'Download and Installation'
weight: 10

menu:
  main:
    name: "Download and Installation"
    parent: "get-started-dmn"
    identifier: "get-started-dmn-install"
    pre: "Install the CadenzaFlow Platform and CadenzaFlow Modeler on your machine."

aliases: [/dmn11/install/]
robotsdisallow: true
---

First you need to set up your development environment and install the CadenzaFlow Platform and the CadenzaFlow Modeler.


# Prerequisites

Make sure you have the following set of tools installed:

* Java JDK 11+,
* Apache Maven (optional, if not installed you can use embedded Maven inside Eclipse.)
* A modern web browser (recent Firefox, Chrome or Microsoft Edge will work fine)
* Eclipse integrated development environment (IDE)


# CadenzaFlow Platform

First, download a distribution of the CadenzaFlow Platform. You can choose from different distributions for various application servers. In this tutorial, we will use the Apache Tomcat based distribution. Download it from [the download page](https://cadenzaflow.com/download).

After having downloaded the distribution, unpack it inside a directory of your choice. We will call that directory `$CAMUNDA_HOME`.

After you have successfully unpacked your distribution of the CadenzaFlow Platform, execute the script named `start-cadenzaflow.bat` (for Windows users), respectively `start-cadenzaflow.sh` (for Unix users).

This script will start the application server and open a welcome screen in your web browser. If the page does not open, go to [http://localhost:8080/cadenzaflow-welcome/index.html](http://localhost:8080/cadenzaflow-welcome/index.html).

{{< note title="Getting Help" class="info" >}}
If you have trouble setting up the CadenzaFlow Platform, you can ask for assistance in the [CadenzaFlow Users Forum](https://forum.cadenzaflow.com/).
{{< /note >}}

# CadenzaFlow Modeler

Follow the instructions in the [CadenzaFlow Modeler](https://docs.cadenzaflow.org/manual/latest/installation/cadenzaflow-modeler/) section.

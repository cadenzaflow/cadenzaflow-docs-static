---

title: 'Download and Installation (1/6)'
weight: 10

menu:
  main:
    name: "Download and Installation"
    parent: "get-started-quick-start"
    identifier: "get-started-quick-start-install"
    pre: "Install the CadenzaFlow Platform and CadenzaFlow Modeler on your machine."

robotsdisallow: true
---

First, you need to install the CadenzaFlow Platform and the CadenzaFlow Modeler.

In the following section, we'll describe how to install the CadenzaFlow Platform locally on your machine.

{{< note title="Hint" class="info" >}}
If you prefer, you can also run the CadenzaFlow Platform with Docker:

```sh
docker pull cadenzaflow/cadenzaflow-bpm-platform:run-latest
docker run -d --name cadenzaflow -p 8080:8080 cadenzaflow/cadenzaflow-bpm-platform:run-latest
```

Afterwards, you can [install the CadenzaFlow Modeler](#cadenzaflow-modeler).
{{< /note >}}


# Prerequisites

Please make sure you have the following installed:

* Java Runtime Environment 17

You can verify this by using your terminal, shell, or command line:

```sh
java -version
```
If you need to install Java Runtime Environment, you can [find the download from Oracle here](https://www.oracle.com/technetwork/java/javase/downloads/index.html). 

{{< note class="info" title="Supported Java versions" >}}
Make sure to use a Java version from [CadenzaFlow's list of supported environments](/manual/latest/introduction/supported-environments/#java-runtime).
{{< /note >}}

# CadenzaFlow Platform

First, download a distribution of the CadenzaFlow Platform. You can choose from different distributions for [various application servers](/manual/latest/installation/full/). In this tutorial, we'll use CadenzaFlow Platform Run. Download it from [the download page](https://cadenzaflow.com/download/platform-7).

After downloading the distribution, unpack it inside a directory of your choice.

After you've successfully unpacked your distribution of the CadenzaFlow Platform, execute the script named `start.bat` (for Windows users) or `start.sh` (for Unix users).

This script will start the application server. Open your web browser and navigate to [http://localhost:8080/](http://localhost:8080/) to visit the Welcome Page. 

# CadenzaFlow Modeler

Download the CadenzaFlow Modeler from [the download page](https://cadenzaflow.com/download/modeler/).

After downloading the Modeler, simply unzip the download in a folder of your choice.

After you have successfully unpacked the zip, run `cadenzaflow-modeler.exe` (for Windows users), `cadenzaflow-modeler.app` (for Mac users), or `cadenzaflow-modeler.sh` (for Linux users).

{{< note title="Next Step" class="info" >}}
Once you've installed the CadenzaFlow Platform and the CadenzaFlow Modeler, you can move to the next step to [model and execute your first process](/get-started/quick-start/service-task/).
{{< /note >}}

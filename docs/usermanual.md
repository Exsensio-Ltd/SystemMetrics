# User Guide Lines

[Back](/README.md#usage)

## Setup

To set up the full system you need three component: Fiware, OEEMicroservice, OEEGrafanaVisualizer.

1. At the first step should be installed Fiware context broker. More information can be found [here](https://github.com/Exsensio-Ltd/OEEMicroservice/blob/master/docs/installationguide.md#orion-context-broker).

2. [OEEMicroservice](https://github.com/Exsensio-Ltd/OEEMicroservice) can be run in a few ways, with Docker or build the project with .NET 5. After starting the OEEMicroservice, you will see the following screen:

    ![Startup](/docs/images/OEEMicroservice.jpg)

    If you see "Connected" followed by version and uptime, the connections between OEEMicroservice and Fiware are ok and the microservice is ready to work.

3. [OEEGrafanaVisualizer](https://github.com/Exsensio-Ltd/OEEGrafanaVisualizer) is available to install the plugin to existing Grafana or can be run as on directly with Docker. The plugin should be configured (Data Source URL) by setting the endpoint of OEEMicroservice. If all services are running and all connections are established you will see the following screen:

    ![Startup](/docs/images/OEEGrafanaVisualizer.jpg)


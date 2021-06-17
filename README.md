![GitHub](https://img.shields.io/github/license/Exsensio-Ltd/SystemMetrics)

# Key Performance Indicators in Automation Systems for Manufacturing

In Manufacturing Operations we have key index's that is worthwhile monitoring , One such index is the OEE which stands for Overall Equipment Effectiveness . This is one of the most favourite measurement in the manufacturing operations , OEE index is an indicator for the efficency for work units or the entire work center.
the microservice allows you to capture and analyze OEE of Station / cell in Manufacturing line. This Microservice can be used with existing software systems along with orion context broker. the Graphana Pluggin allows you to visualize the OEE Metric ( Availablity , Quality and Performance indicators) by a given station and a given product.

The vision here is that no matter what the product or the station in the prodcution line , we will be able to capture the OEE and this value will help the operation mangers see the bottle necks int the production line and also usage of the equipments .

## Architecture

Defenition of the architecture:

Information about the architecture of the OEE sdk can be found in the [Architecture documentation](docs/architecture.md).

## Usage

How to use the component

Information about how to use the OEE sdk can be found in the [User & Programmers Manual](docs/usermanual.md).

## OEEMicroservice

The microservice allows you to capture and analyze OEE of Station / cell in Manufacturing line. This Microservice can be used with existing software systems along with orion context broker. The Graphana Pluggin allows you to visually the OEE Metric (Availablity, Quality and Performance indicators) by a given station and a given product.

| :movie_camera: [Introduction<br>to OEEMicroservice](https://www.youtube.com) | :books: [OEEMicroservice Tutorial<br>Documentation](https://github.com/Exsensio-Ltd/OEEMicroservice) |
| -------------------------------------------------------------------- | --- |

## OEEGrafanaVisualizer

The plugin built with React.js for Grafana Panel and provides representation of the results of OEE (Overall Equipment Effectiveness) for specific device in bar chart and additionnaly lines for `Availability`, `Performance`, `Quality`.

| :movie_camera: [Introduction<br>to OEEGrafanaVisualizer](https://www.youtube.com) | :books: [OEEGrafanaVisualizer<br>Documentation](https://github.com/Exsensio-Ltd/OEEGrafanaVisualizer) |
| -------------------------------------------------------------------- | --- |

## OEEDataModel

OEE Data Model is represent the data that can be used in [OEEMicroservice](https://github.com/Exsensio-Ltd/OEEMicroservice) that is directly communicate with Fiware context broker.

| :books: [OEEDataModel<br>Documentation](https://github.com/Exsensio-Ltd/OEEDataModel) |
| -------------------------------------------------------------------- |

## Install

To download the full set of projects, simply clone this repository:

```console
git clone https://github.com/Exsensio-Ltd/SystemMetrics.git
cd SystemMetrics/
git submodule update --init --recursive
```

The **OEEMicroservice** and **OEEGrafanaVisualizer** projects are then available under the `OEEMicroservice` and `OEEGrafanaVisualizer` directories respectively.

### Postman <img src="https://www.postman.com/favicon-32x32.png" align="left"  height="30" width="30">

The tutorials which use HTTP requests supply a collection for use with the Postman utility. Postman is a testing
framework for REST APIs. The tool can be downloaded from [www.postman.com/](https://www.postman.com/). All the OEEMicroservice
Postman collections can downloaded directly from the
[Postman API network](https://documenter.getpostman.com/view/16273471/TzeWJ91y)

## License

[Apache2.0](LICENSE) © Exsensio Ltd

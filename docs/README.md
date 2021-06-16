# Mid-Term Review

## Contents

-   [Background](#background)
    -   [Use Case Description](#use-case-description)
    -   [Proposed Solution](#proposed-solution)
-   [Mid-Term Setup Implementation Description](#mid-term-setup-implementation-description)
-   [Demo](#demo)
    -   [Install](#install)
    -   [Usage](#usage)
    -   [API](#api)
    -   [Testing](#testing)
-   [License](#license)

## Background

#### Use Case Description

OEE (Overall Equipment Effectiveness) is the gold standard for measuring manufacturing productivity. Simply put – it identifies the percentage of manufacturing time that is truly productive. An OEE score of 100% means you are manufacturing only Good Parts, as fast as possible, with no Stop Time. In the language of OEE that means 100% Quality (only Good Parts), 100% Performance (as fast as possible), and 100% Availability (no Stop Time).

Measuring OEE is a manufacturing best practice. By measuring OEE and the underlying losses, you will gain important insights on how to systematically improve your manufacturing process. OEE is the single best metric for identifying losses, benchmarking progress, and improving the productivity of manufacturing equipment (i.e., eliminating waste).

--extract from oee.com


#### Proposed Solution

In this Experiment we are developing an sdk that allows you to capture and the required data to analyze OEE of Station / cell in Manufacturing line.
This .NET sdk can be used directly with existing software systems to extract the data and push the payload to an orion context broker. the Graphana Pluggin then alanysis the NGSI data and calculates the OEE and Visually represents them. 

In this Experiment We use a cobot to pick and place DUT into the Manual Test Fixture , All the CPS is controlled by Exsensio test automation framwork and excutes the test on the Device under test , the framework uses the OEE SDK to populate the required data and push them to the orion context broker . The OEE Grafana plugin will then analyse the data from the the orion context broker and calculate the OEE metrics for that Station ( in this case its a Test Station)

Similary we will use the same cobot in a assembly station for assistive assmemly and also be able to capture OEE for that station . 

The vision here is that no matter what the product or the station in the prodcution line , we will be able to capture the OEE and this value will help the operation mangers see the bottle necks int the production line and also usage of the equipments .

#### Architecture
A more detailed description of this architecture is available here [Architecture Description](architecture.md)

## Demo
#### Install
In order to install the components of our demo, follow the instructions provided in this file: [Installation & Administration Guide](installationguide.md)

#### Usage
Information about how to use the demo components can be found in the [User & Programmers Manual](getting-started.md).

#### API
Detailed descriptions of the demo component APIs are available in the [API documentation](api.md)

## License

[MIT](LICENSE) © <TTE>

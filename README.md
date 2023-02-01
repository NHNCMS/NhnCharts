# Software and Microservices Deployment Chart

## Introduction
This Helm chart provides an easy way to deploy the NHN project and its associated microservices on a Kubernetes cluster.

## Requirements
- Kubernetes cluster
- Helm version 3.x or later

## Installation
To install the chart, run the following command:

helm install [RELEASE_NAME] [CHART_NAME]

## Usage
This chart deploys the NHN project and its microservices using the following resources:
- Deployments
- Services
- ConfigMaps
- Ingress

## Dependencies
The chart requires the following dependencies:
- Kafka 3.3.x or later
- Mongodb 4.4.x or later

## Configuration
The following parameters can be configured in the `values.yaml` file:
- `categories.image`: image name of the "categories" microservice.
- `categories.ingressPrefix`:  ingress prefix for the "categories" microservice.
- `tags.image`: tag of the "tags" microservice image to be deployed.
- `tags.ingressPrefix`: ingress prefix for the "tags" microservice.
- `ingress.host`: base hostname for the entire application.

## Contributing
Contributions to the chart are welcome. 💕

## License
This chart is released under the MIT license.

## Troubleshooting
If you encounter any issues with the deployment, consult the troubleshooting guide for possible solutions.

## Credits
This chart uses resources from the Kubernetes project and was created by the NHN guild.

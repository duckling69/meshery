# Meshery

A service mesh playground to faciliate learning about functionality and performance of different service meshes. Meshery incorporates the collection and display of metrics from applications running in the playground.

Meshery is written in `Go` (Golang) and leverages Go Modules. The `deployment_yaml` folder contains the configuration yaml to deploy Meshery on Kubernetes, which includes a Deployment, Service, Service Entries and Virtual Services configurations.

## Prequisites
1. Docker engine (e.g. Docker for Desktop).
1. Kubernetes cluster (preferably version 1.10+).

## Istio Playground App
A sample Istio app is included in Meshery. 

### Running Meshery
#### Prerequisites
1. Istio version 1.0.3+ in `istio-system` namespace along with the Istio ingress gateway.
1. The canonical Istio _bookinfo_ sample application deployed in the `default` namespace.

#### Run
To run the service mesh playground:
1. Clone this repository (`git clone https://github.com/layer5io/meshery.git`).
1. Build the Meshery Docker image (`docker build .`).
1. Deploy Meshers (`kubectl apply -f deployment_yamls/deployment.yaml`).

## Linkerd Playground App
_coming soon_
### Running Meshery
#### Prerequisites
#### Run

### Building Meshery
A sample Makefile is included to build and package the app as a Docker image.
1. `Docker` to build the image.
1. `Go` version 1.11+ installed if you want to make changes to the existing code.

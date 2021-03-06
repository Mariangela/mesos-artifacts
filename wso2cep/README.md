# Mesos Artifacts for WSO2 Complex Event Processor

These Mesos Artifacts provide the resources and instructions to deploy WSO2 Complex Event Processor on Mesos DC/OS.

## Getting Started

To deploy a WSO2 product on Mesos DC/OS, follow the below steps:

* Build WSO2 Complex Event Processor Docker images using [WSO2 Dockerfiles](https://github.com/wso2/dockerfiles).
* Load above Docker images to Mesos slave nodes or import them to a central Docker registry.
* If a central Docker registry is used, update Docker image tags accordingly in WSO2 Complex Event Processor Marathon applications.
* Run `deploy.sh` found inside this folder. It will deploy following containers:
   * Marathon load balancer container
   * WSO2 Governance Registry database container
   * WSO2 User Management database container
   * WSO2 Complex Event Processor Configuration Registry database container
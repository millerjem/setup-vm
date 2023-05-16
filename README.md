# Virtual Machine Installation

Follow this guide to deploy Istio using the IstioLifecycleManager and connect a virtual machine to it.

```
./setup-vm

  Usage: setup-vm [options]
    -c --cluster    Cluster name the default values is $CLUSTER_NAME
    -i --istio      Deploys Istio using IstioLifecycleManager
    -g --gateway    Deploys Istio using GatewayLifecycleManager
    -r --rev        Sets the Istio revision number the default value is $ISTIO_REVISION
    -t --tag        Sets the Istio image tag the default value is $ISTIO_IMAGE_TAG
    -v --vm         Deploys VM
    -s --sample     Deploys a sample application helloworld
    -e --external   Deploys the external service
    -d --debug      Prints debug commands
    -h --help       Prints usage
```

Example
```
# To install Istio on the management cluster
./setup-vm -i -c mgmt-cluster

# To perform a dry run
./setup-vm -i -c mgmt-cluster -d
```

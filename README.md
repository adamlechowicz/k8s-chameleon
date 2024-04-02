# Deploy a Kubernetes cluster

This profile creates a Kubernetes cluster with Kubespray, either at KVM@TACC on [Chameleon](https://chameleoncloud.org/) or on [FABRIC](https://portal.fabric-testbed.net/). (Note: [CloudLab](https://www.cloudlab.us/) has an [officially supported profile](https://www.cloudlab.us/p/emulab-ops/k8s) for deploying a Kubernetes cluster.)

It is intended as a general-purpose "recipe" for use in teaching cloud computing.

It uses 3 `m1.large` VMs (and 1 floating IP, if you are using Chameleon).

Follow the instructions in `reserve_kvm/index.md` (Chameleon) or `reserve_fabric/index.md` (FABRIC) to launch your Kubernetes cluster.

> [!WARNING]
> If you're using FABRIC, you won't be able to directly visit a web service deployed on your Kubernetes cluster in your own browser, since it is behind a bastion host for security. You will have to first set up an SSH tunnel to the bastion host to view your web service. 

---
This material is based upon work supported by the National Science Foundation under Grant No. 2230079. 

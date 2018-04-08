# Azure Container Services (AKS) - Hands-on Lab Script

Mark Harrison : 7 Apr 2018

![](Images/AKS.png)

- [Part 1 - Azure Container Service (AKS)](aks-1.md)
- [Part 2 - Helm Package Management](aks-2.md)  ... this document
- [Part 3 - Monitoring Kubernetes](aks-3.md)

## Helm

[Kubernetes Helm](https://github.com/kubernetes/helm) is a tool for installing packages of pre-configured Kubernetes resources.

### Install

To install Helm on Windows, use the Chocolately package at https://chocolatey.org/packages/kubernetes-helm 

![](Images/HelmChocolatey.png)

Helm has two parts: a client (Helm) and a server (Tiller)
Tiller runs inside of your Kubernetes cluster, and manages releases (installations) of your charts.

To install the Tiller, use the command:

```text
helm init
```

We can see that the Tiller has been installed as a Pod 

![](Images/HelmTiller.png)

---
[Home](aks-0.md) | [Prev](aks-1.md) | [Next](aks-3.md)
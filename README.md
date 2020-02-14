# Random Bunch of Apps for Demo
This repo is a consolidation of different kubernetes applications that can be used for testing/poc.

All the yamls are tested to be working with **PKS 1.5.0** running **Kubernetes v1.14.5**

Each folder consist of different application deployment yamls that can be use to test different deployment config.

**Disclaimer: All the applications in this repo are not developed by me.**

Applications are categorized as follows:

| Apps | Folder |
| ------ | ------ |
| nginx demo app | [nginx-app/](https://github.com/Physium/temp-pks-demo/tree/master/nginx-app) |
| yelb demo app | [yelb-demo/](https://github.com/Physium/temp-pks-demo/tree/master/yelb-demo) |

# nginx demo app
This folder consist of various nginx k8s configuration.

### base.yml
A basic nginx deployment just to test pod deployment and pod services accessibility.

Uses Loadbalancer as a service.

### kuard.yml
Another basic nginx deployment that is commonly used to show pod deployment statstics.

Uses Contour as an ingress.

### cafe-app-example
Not exactly an application but a series of nginx deployment to show case ingress routing with https.
Uses Contour as an ingress.

Reference:
[https://code.vmware.com/samples/5595/Running-Contour-as-Ingress-on-Enterprise-PKS-k8s-clusters-with-NSX-T](https://code.vmware.com/samples/5595/Running-Contour-as-Ingress-on-Enterprise-PKS-k8s-clusters-with-NSX-T)

[https://code.vmware.com/samples/5502/running-nginx-ingress-on-pks-k8s-clusters-with-nsx-t](https://code.vmware.com/samples/5502/running-nginx-ingress-on-pks-k8s-clusters-with-nsx-t)

# yelb demo app
This is a basic microservice application which can be use to showcase various k8 deployment concepts. 

YAMLs in this folder are tweak and edited accordingly to how I would deploy or showcase it.

All original content and credits goes to [https://github.com/mreferre/yelb](https://github.com/mreferre/yelb).

### yelb-app
Showcases various k8 deployment config with a mixture of the following:
* ingress
* load balancer
* network policy

### yelb-app-pvc
Similar to yelb-app but showcases the deployment yelb-app with dynamic pvc.

# More randoms apps - Untested
Consolidating more demo apps found over time

[VMware Cloud Advocacy - ACME Fitness](https://github.com/vmwarecloudadvocacy/acme_fitness_demo)

[GCP Microservics Demo - Hipster Shop](https://github.com/GoogleCloudPlatform/microservices-demo)

[Project Pacific Demo Apps](https://github.com/dstamen/Kubernetes/tree/master/demo-applications)

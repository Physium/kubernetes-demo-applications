# Random Bunch of Apps for Demo
This repo is a consolidation of different k8 applications that can be used for testing/poc. Each folder consist of different k8 yamls that can be use to test different kubernetes deployment config.

Disclaimer: All the applications in this repo are not developed by me. 

Applications are categorized as follows:

| Apps | Folder |
| ------ | ------ |
| nginx demo app | [nginx-app/](https://github.com/Physium/temp-pks-demo/tree/master/nginx-app) |
| yelb demo app | [yelb-demo-wj/](https://github.com/Physium/temp-pks-demo/tree/master/yelb-demo-wj) |

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

# yelb demo app
This is one of the most comprehesion applications that showcases the fundamental concepts of a microservice application. This applications can be use to showcase various concepts on k8 deployment.

All credits goes to [https://github.com/mreferre/yelb](https://github.com/mreferre/yelb).

### yelb-app
Showcases various k8 deployment config with a mixture of the following:
* ingress
* load balancer
* network policy

### yelb-app-pvc
Similar to yelb-app but showcases the deployment of deploying yelb-app with dynamic pvc.
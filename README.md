# openshift-post-config
This repository contains OpenShift cluster level configuration which is being orchestrated and managed by GitOps.
There are a host of applications being managed by gitops, as well as an example tenant (mnaas-tenant) in which applications can be deployed from.

In order to deploy this configuration into a fresh instance of OpenShift, there are some steps which must be followed:
## 1 Install gitops operator on the cluster
## 2 run the comman 'oc apply -k .' inside of the applications/overlay/dev folder
Once these simple steps have been followed, gitops will create a series of applications and install quite a few components - this may take up to 15 minutes to complete.
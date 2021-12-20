# openshift-post-config
This repository contains OpenShift cluster level configuration which is being orchestrated and managed by GitOps.
There are a host of applications being managed by gitops, as well as an example tenant (mnaas-tenant) in which applications can be deployed from.

# Prerequisites
In order to create this project, the user must have the following installed on their local machine
oc cli - can be downloaded from: https://access.redhat.com/downloads/content/290/
kustomize cli - can be downloaded from: https://kubectl.docs.kubernetes.io/installation/kustomize/

In order to deploy this configuration into a fresh instance of OpenShift, there are some steps which must be followed:
1. Install gitops operator on the cluster
2. run the command code(kustomize build . | oc apply -f -) inside of the applications/overlay/dev folder
Once these simple steps have been followed, gitops will create a series of applications and install quite a few components - this may take up to 15 minutes to complete.
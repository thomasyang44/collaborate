# Thomas Reference for OCP and CP4BA


## OC Login
```bash
# Login
oc login -u ocadmin

# Login with password
oc login -u ocadmin -p ibmrhocp

# Login with node and password
oc login https://api.labs.ihost.com:6443 -u ocadmin -p ibmrhocp
```

## oc get nodes
```bash
oc get nodes

compute0.ocp.ibm.edu
compute1.ocp.ibm.edu
compute2.ocp.ibm.edu
compute3.ocp.ibm.edu
control0.ocp.ibm.edu
control1.ocp.ibm.edu
control2.ocp.ibm.edu
infra0.ocp.ibm.edu  
infra1.ocp.ibm.edu  
storage0.ocp.ibm.edu
storage1.ocp.ibm.edu
storage2.ocp.ibm.edu
```

## oc get deploy - icp4adeploy pods
```bash
oc get deploy -o name | grep icp4adeploy

deployment.apps/icp4adeploy-ads-credentials-service
deployment.apps/icp4adeploy-ads-git-service
deployment.apps/icp4adeploy-ads-parsing-service
deployment.apps/icp4adeploy-ads-rest-api
deployment.apps/icp4adeploy-ads-run-service
deployment.apps/icp4adeploy-ads-runtime-service
deployment.apps/icp4adeploy-cdra-deploy
deployment.apps/icp4adeploy-cds-deploy
deployment.apps/icp4adeploy-classifyprocess-classify
deployment.apps/icp4adeploy-cmis-deploy
deployment.apps/icp4adeploy-cpds-deploy
deployment.apps/icp4adeploy-cpe-deploy
deployment.apps/icp4adeploy-cpe-watcher
deployment.apps/icp4adeploy-css-deploy-1
deployment.apps/icp4adeploy-deep-learning
deployment.apps/icp4adeploy-gitgateway-deploy
deployment.apps/icp4adeploy-graphql-deploy
deployment.apps/icp4adeploy-ier-deploy
deployment.apps/icp4adeploy-insights-engine-cockpit
deployment.apps/icp4adeploy-insights-engine-flink
deployment.apps/icp4adeploy-insights-engine-flink-taskmanager
deployment.apps/icp4adeploy-insights-engine-management
deployment.apps/icp4adeploy-mls-itp
deployment.apps/icp4adeploy-mls-wfi
deployment.apps/icp4adeploy-mongo-deploy
deployment.apps/icp4adeploy-natural-language-extractor
deployment.apps/icp4adeploy-navigator-deploy
deployment.apps/icp4adeploy-navigator-watcher
deployment.apps/icp4adeploy-ocr-extraction
deployment.apps/icp4adeploy-odm-decisioncenter
deployment.apps/icp4adeploy-odm-decisionrunner
deployment.apps/icp4adeploy-odm-decisionserverconsole
deployment.apps/icp4adeploy-odm-decisionserverruntime
deployment.apps/icp4adeploy-pbk-ae-deployment
deployment.apps/icp4adeploy-postprocessing
deployment.apps/icp4adeploy-processing-extraction
deployment.apps/icp4adeploy-setup
deployment.apps/icp4adeploy-spbackend
deployment.apps/icp4adeploy-tm-deploy
deployment.apps/icp4adeploy-viewone-deploy
deployment.apps/icp4adeploy-wdu-extraction
deployment.apps/icp4adeploy-wdu-runtime
deployment.apps/icp4adeploy-webhook
deployment.apps/icp4adeploy-workspace-aae-ae-deployment
````

## oc get sts - icp4adeploy pods (Security Token Service)
```bash
oc get sts -o name | grep icp4adeploy

## oc get sts - icp4adeploy pods (Security Token Service)
```bash
oc get sts -o name | grep icp4adeploy
````





for i in `oc get deploy -o name |grep icp4adeploy`; do oc scale $i --replicas=0; done







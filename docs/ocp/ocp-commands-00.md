#  OpenShift Container Platform CLI tools OpenShift CLI (oc) OpenShift CLI developer command reference 
#### https://docs.openshift.com/container-platform/4.16/cli_reference/openshift_cli/developer-cli-commands.html


  ## cluster-info
  ```bash
  # Print the address of the control plane and cluster services
  oc cluster-info

  Kubernetes control plane is running at https://api.ocp.ibm.edu:6443
  ```

  ## oc config get-clusters
  ```bash
  # List the clusters that oc knows about
  oc conf ig get-clusters
  
  NAME
  api-ocp-ibm-edu:6443
  ```

  ## Describe a node
  oc describe nodes kubernetes-node-emt8.c.myproject.internal

  ## Describe a pod
  oc describe pods/nginx

  ## Describe a pod identified by type and name in "pod.json"
  oc describe -f pod.json

  ## Describe all pods
  oc describe pods

  ## Describe pods by label name=myLabel
  oc describe pods -l name=myLabel

  ## Describe all pods managed by the 'frontend' replication controller (rc-created pods get the name of the rc as a prefix in the pod name)
  oc describe pods frontend


  
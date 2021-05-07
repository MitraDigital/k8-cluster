# Kubernetes Cluster Deployment with Kubespray
Below diagram depicts the setup that has been configured with this version of script.
![Setup Diagram](images/setup-diagram.png)

| Component | Description |
| ------ | ------ |
| External Node | Host that will be the entry point of this execution from where scripts will be executed to remote |
| Kubespray Terraform Script | Used provision the needed servers in the Google Cloud Platform |
| Kubespray Ansible Playbook| [Used to deploy and configure the K8s Cluster in the provisioned servers |
| Kubectl | Kubectl client installed to manage the kubernetes Cluster from the External Node. |
| Google Cloud Platform | Servers were provisioned and for this setup it uses 3-Control Plane Nodes ( ETCD setup done within them ) and 3-Worker Nodes where the nginx proxy setup done for the communication between Worker to API servers happens in a load balanced way. |

# k8s
All about k8s

Kubernetes has 2 nodes mainly

* Control plane nodes
  * Kubectl: Command-line application for Kubernetes, that allows you to manage your resources and K8s cluster nodes. Its primary responsibility is providing a simple interface to the end user while interacting with the
    API server in the control plane
  * API Server - This is the Kubernetes cluster API endpoint that provides unified access to end users for Kubernetes management. You can manage your Kubernetes resources or maintain Kubernetes nodes through this component
    with the help of kubectl
  * Scheduler - Whenever you try to deploy a pod, it will be scheduled to an available node based on resource requirements.
     <p>The filtering and scoring phases are implemented by two types of components: predicates and priorities. Predicates are boolean functions that return true or false for each node. They are used to implement the filtering logic. Priorities are  
     numeric functions that return a score between 0 and 10 for each node. They are used to implement the scoring logic.</p>
  * Controller manager - The Kubernetes Controller Manager runs control loops that ensure the cluster's actual state matches the desired state, handling tasks like node health, pod replicas, and service accounts.
  * etcd - In Kubernetes, etcd is a distributed key-value store that holds the entire cluster state, including nodes, pods, services, and configurations. It ensures consistency and reliability using the Raft consensus algorithm.
* Worker nodes

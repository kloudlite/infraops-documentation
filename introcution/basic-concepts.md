# Basic Concepts

## **Cloud Providers**

A cloud provider delivers a suite of cloud computing services that include provisioning of virtualized computing resources such as compute instances, storage options, and networking capabilities. These services are accessible via the internet, enabling users to deploy, manage, and scale applications in a cloud environment seamlessly.

[add-your-cloud-provider.md](getting-started/add-your-cloud-provider.md "mention")

## **Kubernetes Clusters**

Kubernetes clusters are collections of nodes (servers) that run containerized applications. They provide a robust environment for deploying, scaling, and managing applications across a distributed compute infrastructure, ensuring high availability and efficient resource utilization.

[create-your-first-kloudlite-cluster.md](getting-started/create-your-first-kloudlite-cluster.md "mention")

## **NodePools**

Within the Kloudlite platform, NodePools facilitate the organization of nodes into distinct groups. These groups can be defined based on various criteria, including hardware characteristics, geographical locations (availability zones), or specific application needs. NodePools are instrumental in optimizing resource management and simplifying the process of scaling resources to meet application demands.

[setup-nodepools.md](getting-started/setup-nodepools.md "mention")

## **Helm Charts**

Helm charts are packages that facilitate the definition, installation, and upgrade of Kubernetes applications. They package together Kubernetes resources such as deployments, services, and ingresses, making it easier to deploy and manage complex applications across Kubernetes clusters. Kloudlite supports the deployment and configuration of Helm charts directly through its dashboard, streamlining application deployment and management processes.

[create-helm-charts.md](getting-started/create-helm-charts.md "mention")

## Build your own kubernetes cluster

The "Build Your Own Kubernetes" feature empowers users to manually construct their own Kubernetes clusters.

[build-your-own-kubernetes-cluster.md](getting-started/build-your-own-kubernetes-cluster.md "mention")

## Cluster Managed Services <a href="#managed-services" id="managed-services"></a>

**Managed Services** are key services that your application relies on to function. Kloudlite simplifies the process of setting up, managing, and maintaining these services, including:

* **MongoDB** (available in both Cluster and Standalone modes)
* **MySQL** (available in both Cluster and Standalone modes)
* **Redis** (available in both Cluster and Standalone modes)

These services are managed by Kloudlite to free you from manual setup and maintenance, ensuring your applications have the support they need. We're always working to add more services.

[create-cluster-managed-service.md](getting-started/create-cluster-managed-service.md "mention")

## **Wireguard Integration**

Kloudlite integrates Wireguard, a modern VPN protocol, to provide secure access to services running within Kubernetes clusters. The Kloudlite command-line interface (CLI), known as `kli`, enables users to establish a Wireguard VPN connection from their local machine to the cluster. This connection offers a secure, encrypted pathway to cluster services, facilitating development and operational tasks by providing direct access to internal cluster resources.

[wireguard-connect.md](../cluster-details/wireguard-connect.md "mention")


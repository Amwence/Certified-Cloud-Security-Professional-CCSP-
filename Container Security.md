# Container Security

## Managed Kubernetes

- ***Container hosts*** are cloud-based virtual machines. (This is where containers run)

- Most CSPs offer ***Hosted Kubernetes Service***, handles critical tasks like health monitoring and maintenance for you. (Platform-as-a-Service)

- You pay only for the agent nodes within your clusters, not for the management cluster. 

- Major CSPs also offer a monitoring solution that will identify at least some potential security concerns

> Shares Many of the concerns of server virtualization, but must enforce ***isolation*** of network, data, storage access at container level

*** EXAMPLES: Azure Kubernetes Service or AKS (Microsoft), Elastic Kubernetes Service or EKS (Amazon Web Services), Google Kubernetes Engine or GKE (Google Cloud Platform)***
# Elasticsearch Kubernetes Cluster with Search Guard

This is forked from [pires/kubernetes-elasticsearch-cluster](https://github.com/pires/kubernetes-elasticsearch-cluster) and adds search-guard into the cluster.

It is ready to go with the plugin and you can simply follow the below instructions (TODO) to play with search-guard using the sample configuration.

All the images are installed with search-guard, and you can find it [here](https://github.com/xanthous-tech/docker-es-k8s-search-guard). The kibana with search-guard plugin is [here](https://github.com/xanthous-tech/docker-kibana-k8s-search-guard).

DISCLAIMER: **It requires configuration before using in production.** I would suggest working FROM our [docker image](https://hub.docker.com/r/xanthoustech/es-k8s-search-guard/) and add in proper configurations after reading [the search-guard documentation](https://docs.search-guard.com/latest/index) and following the instructions on how to configure proper SSL access methods, and user permission modeling. The current configuration is exactly the demo configuration for search-guard, which is not safe for production use and needs to be updated before putting the cluster in public network.

# Initial Default Configuration

Please treat the below configuration as samples on how to configure a medium-sized cluster on GKE. Make sure you update the params before using.

Cluster:

- 12 x 4 CPU 15GB nodes
- 20TiB SSDs

Elasticsearch:

- 5 masters
- 10 data nodes
- 2 ingest nodes

# Deployment

- create a new cluster on GKE UI.

TODO: more instructions

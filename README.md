# OpenShift Custom Catalog Templates

This repository contain Red Hat OpenShift custom catalog templates

- Apache Kafka
- ElasticSearch
- File Drive
- LogStash
- MinIO
- Neo4j
- Redash

All catalog template in this repository is using images from [https://hub.docker.com/r/dimaskiddo](https://hub.docker.com/r/dimaskiddo) repository.



## How to Use

To use and apply the catalog template you need at least admin privileges and have access to **openshift** project, after that you can apply it using OpenShift Client command line tools

```sh
oc create -f <CATALOG_NAME>/<CATALOG_NAME>-<VOLUME_TYPES>.yml -n openshift
```

Example:

```sh
oc create -f MinIO/minio-ephemeral.yml -n openshift
```


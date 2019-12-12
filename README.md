# OpenShift Custom Catalog Templates

This repository contain custom catalog template for Red Hat OpenShift

- Apache Kafka
- ElasticSearch
- File Drive
- LogStash
- Minio
- Neo4j
- OpenShift (System)
- Redash
- Etc

All catalog template in this repository is using [TelkomIndonesia](https://hub.docker.com/r/telkomindonesia) Docker images, since TelkomIndonesia Docker repository is based on [DimasKiddo](https://hub.docker.com/r/dimaskiddo) Docker repository you can change it to DimasKiddo one.



## How to Use

To use and apply the catalog template you need at least admin privileges to **openshift namespace**, after that you can apply it using oc command-line tools

```sh
oc create -f <CATALOG_NAME>/<CATALOG_NAME>-<VOLUME_TYPES>.yml -n openshift
```

Example:

```sh
oc create -f Minio/minio-ephemeral.yml -n openshift
```


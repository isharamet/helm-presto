# Presto Chart

[Presto](http://prestosql.io/) is a high performance, distributed SQL query engine for big data.

## Chart Details

This chart will do the following:

* Install a single server which acts both as coordinator and worker
* Install a configmap for it
* Install a service

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ cd helm-presto
$ helm install my-release .
```

## Configuration

Configurable values are documented in the `values.yaml`.

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`.

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

```bash
$ cd helm-presto
$ helm install my-release -f values.yaml .
```

> **Tip**: You can use the default [values.yaml](values.yaml)

## Deploying Chart in minikube

Default minikube memory and CPU settings can be insufficient, so in order to run chart locally increase CPU and memory values:
 
```bash
minikube start --cpus 6 --memory 8192
```


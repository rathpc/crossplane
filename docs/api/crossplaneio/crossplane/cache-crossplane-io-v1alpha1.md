# cache.crossplane.io/v1alpha1 API Reference

Package v1alpha1 contains portable resource claims for caching services such as Redis clusters.

This API group contains the following Crossplane resources:

* [RedisCluster](#RedisCluster)
* [RedisClusterClass](#RedisClusterClass)

## RedisCluster

A RedisCluster is a portable resource claim that may be satisfied by binding to a Redis managed resource such as a GCP CloudMemorystore instance or an AWS ReplicationGroup. Despite the name RedisCluster claims may bind to Redis managed resources that are a single node, or not in cluster mode.


Name | Type | Description
-----|------|------------
`apiVersion` | string | `cache.crossplane.io/v1alpha1`
`kind` | string | `RedisCluster`
`metadata` | [meta/v1.ObjectMeta](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.15/#objectmeta-v1-meta) | Kubernetes object metadata.
`spec` | [RedisClusterSpec](#RedisClusterSpec) | RedisClusterSpec specifies the desired state of a RedisCluster.
`status` | [v1alpha1.ResourceClaimStatus](../crossplane-runtime/core-crossplane-io-v1alpha1.md#resourceclaimstatus) | 



## RedisClusterClass

RedisClusterClass contains a namespace-scoped portable class for RedisCluster


Name | Type | Description
-----|------|------------
`apiVersion` | string | `cache.crossplane.io/v1alpha1`
`kind` | string | `RedisClusterClass`
`metadata` | [meta/v1.ObjectMeta](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.15/#objectmeta-v1-meta) | Kubernetes object metadata.


RedisClusterClass supports all fields of:

* [v1alpha1.PortableClass](../crossplane-runtime/core-crossplane-io-v1alpha1.md#portableclass)


## RedisClusterSpec

RedisClusterSpec specifies the desired state of a RedisCluster.

Appears in:

* [RedisCluster](#RedisCluster)


Name | Type | Description
-----|------|------------
`engineVersion` | string | EngineVersion specifies the desired Redis version.


RedisClusterSpec supports all fields of:

* [v1alpha1.ResourceClaimSpec](../crossplane-runtime/core-crossplane-io-v1alpha1.md#resourceclaimspec)


This API documentation was generated by `crossdocs`.
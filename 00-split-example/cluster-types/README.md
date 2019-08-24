# ClusterTypes

ClusterTypes define cluster level ResourceGroups and Namespaces that need to be created.

Configuration defined at the root of cluster-types/ applies to all clusters

A ClusterType is denoted by a path `product/dev` or `internal`

A Cluster can be given a ClusterType that isn't represented by config in the repository admiral
simply walks backwards through the path to find the nearest match.

Namespaces in the `namespace` section will be created and have an annotation set on them to note the
desired NamespaceType

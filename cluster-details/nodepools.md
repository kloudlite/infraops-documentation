---
description: >-
  Cluster Autoscaler - a component that automatically adjusts the size of a
  Kubernetes Cluster so that all pods have a place to run and there are no
  unneeded nodes. Supports several public cloud provide
---

# Nodepools

kloudlite support different type of nodepools for different type of cloud provider.

We can broadly categorize them using following properties

* application state types: `stateful`/`stateless`

{% hint style="info" %}
Node labels:

`kloudlite.io/pool.app-state-type: stateful/stateless`
{% endhint %}

* provisioning mode: `on-demand`/`spot`

{% hint style="info" %}
`Node labels:`

`kloudlite.io/pool.provision-mode: on-demand/spot`
{% endhint %}

* Auto scaling: `enabled`/`disabled`

{% hint style="info" %}
`Node labels:`

`kloudlite.io/pool.auto-scaling: enabled/disabled`
{% endhint %}

You can refer below url for more details

[https://github.com/kloudlite/autoscaler/tree/kloudlite](https://github.com/kloudlite/autoscaler/tree/kloudlite)

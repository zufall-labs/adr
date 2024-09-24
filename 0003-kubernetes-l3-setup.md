# 3. Kubernetes L3 setup

Date: 2024-09-24

## Status

Accepted

## Context

Kubernetes must be run either on a cloud provider's managed solution, or on a self managed cluster of resources. 

## Decision

We decided to self-host K3s on the Hetzner Cloud platform using the `k3s-hetzner` [CLI](https://github.com/vitobotta/hetzner-k3s/blob/main/docs/Setting%20up%20a%20cluster.md) and develop locally using Minikube or KinD.

## Consequences

Very affordable Kubernetes derivate for the startup phase in exchange for manual setup and administrative duties.

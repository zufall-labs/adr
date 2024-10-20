# 5. CPU intensive

Date: 2024-10-20

## Status

Accepted

## Context

The `API Gateway` and the `MQTT Bridge` are connected by the `Entropy service`. This service has two responsibilities:

1. handling the incoming and outgoing communication
2. doing calculations and adjustments to the data

## Decision

We decided on a `Java` application for working with the data.
We haven't yet fully decided on which framework and JDK vendor we will be using.
Most likely it will be [GraalVM](https://www.graalvm.org/) with [Micronaut](https://micronaut.io/)
or [Quarkus](https://quarkus.io/). Perhaps even plain `Java` without any framework.

## Consequences

Due to how the JVM works and its long startup time, we will likely have the application always running.

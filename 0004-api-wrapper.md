# 4. API Wrapper

Date: 2024-10-20

## Status

Accepted

## Context

The `API Gateway` and the `MQTT Bridge` are connected by the `Entropy service`. This service has two responsibilities:
1. handling the incoming and outgoing communication
2. doing calculations and adjustments to the data

## Decision

We decided on a simple `Go` application for handling this communication.
We haven't yet fully decided on which framework we will be using. Most likely it will be the [Gin](https://gin-gonic.com/) framework.

## Consequences

As the `Go` application won't do any calculations or adjustments to the data, it will be as simple as possible. 

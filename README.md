# axiom-control-plane

## Purpose
The control plane manages configuration, metadata, and coordination for the Axiom platform.

It governs how the system operates without participating in the data path.

## Responsibilities
- Manage system metadata and configuration
- Control partitions, schemas, and retention policies
- Orchestrate safe operational changes
- Expose administrative APIs

## Non-Responsibilities
- Handling data plane traffic
- Event ingestion or processing
- Serving analytical queries
- High-throughput operations

## Failure Model
- Strong consistency is required
- Must remain available independently of data load
- Incorrect decisions are more dangerous than slow decisions

## Status
Week 0: Minimal HTTP server with `/health` endpoint.

# Emerald
The ergonomic and blazing fast ephemeral data service that provides KV storage, task queues, and task scheduling. Distributed, sharded, and durable. Made with Rust 🦀.

Emerald is designed to be used alongside a traditional persistent data store, like Postgres or Mongo, and provide commonly used functionality for ephemeral data. By ephemeral, we mean data that is not meant to be long-lived. In a practical sense, the goal of Emerald could be said to consolidate dependencies typically found on cloud-provider based solutions (SQS, GCP Tasks) into a single, open source augmentative solution. This use-case oriented design has a few functional implications:

- Emerald does not aim to provide a comprehensive API (eg such as the Redis API). Operations like `SCAN` may not even be implemented.
- While Emerald provides functionality for managing task queues and task scheduling, it does not handle execution of tasks but passes this off to clients.

## Goals
- **Fast.** Emerald should be competitive when compared to other in-memory data stores.
- **Light.** Emerald should have as small a footprint on resource consumption as possible.
- **Ergonomic.** Emerald should provide intuitive APIs for common uses.
- **Distributed.** Emerald should assume it is part of a cluster, and all features should support clustering.
- **Scaleable.** Emerald should scale seamlessly by adding new nodes.

## Target uses-cases
- Key-value cache
- Queue
- Task scheduling

## Name
The name _Emerald_ is derived from the words _ephemeral_ and _daemon_. Conveniently, it is also a shiny rock.

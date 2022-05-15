# emerald
The ergonomic and blazing fast ephemeral data store made for caches, queues, and scheduled tasks, with durability and clustering built-in. Written in Rust 🦀.

## Goals
- **Fast.** emerald should be competitive when compared to other in-memory data stores.
- **Light.** emerald should have as small a footprint on resource consumption as possible.
- **Ergonomic.** emerald should provide approachable abstractions for common uses.
- **Distributed.** emerald should assume it is part of a cluster, and all features should support clustering.

## Target uses-cases
- Key-value cache
- Queue
- Task scheduling

## Name
The name _emerald_ is derived from the words _ephemeral_ and _daemon_. Conveniently, it is also a shiny rock.

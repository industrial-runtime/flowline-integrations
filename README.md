# Flowline Integrations

This repository contains **integration adapters** for Flowline in **C# and C++**.
Adapters connect the station runtime to hardware, vendor SDKs, and external systems.

## Responsibilities
- Hardware/protocol access (C# and/or C++)
- Encapsulate vendor SDKs and low-level APIs
- Provide a stable boundary to `flowline-runtime` (IPC / network, as defined by contracts)
- Return status/measurements and execute commands as requested by the runtime

## Non-Responsibilities
- No process logic
- No state machine decisions
- No Poka-Yoke rules (those live in `flowline-core` / `flowline-runtime`)
- No UI responsibilities

## Documentation
Architecture and decisions: see `flowline-docs`.

## License
Apache License 2.0

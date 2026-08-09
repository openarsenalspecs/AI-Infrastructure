# QGuardian Registry

**QGuardian Registry - The Compatibility Layer for Quantum Hardware.**

QGuardian Registry is an open-source, vendor-neutral quantum hardware capability and compatibility platform designed to standardize how quantum devices publish, expose, and share their capabilities. The registry provides machine-readable hardware profiles containing native gate sets, qubit topology, fidelity metrics, calibration data, and device metadata, enabling automated hardware discovery and compatibility matching across the quantum computing ecosystem.

QGuardian Registry serves as the hardware intelligence layer for [QGuardian — Fidelity First](https://gitlab.com/Roxanne_Ardary/qguardian), allowing runtimes and applications to automatically identify the most suitable hardware for a given quantum workload while reducing transpilation overhead and improving execution reliability.

---

# Goals

- Standardize quantum hardware capability descriptions.
- Enable automatic hardware discovery and compatibility matching.
- Reduce circuit transpilation and execution errors.
- Improve hardware portability across providers.
- Support reproducible quantum experimentation.
- Create an open, vendor-neutral compatibility layer.
- Provide a long-term foundation for quantum hardware interoperability.

---

# Core Features

## Hardware Capability Profiles
- Standardized machine-readable device schemas.
- Hardware metadata definitions.
- Versioned capability profiles.
- Custom provider extensions.
- Hardware revision tracking.
- Capability validation.

## Native Gate Set Registry
- Native gate set indexing.
- Supported instruction set definitions.
- Parameterized gate metadata.
- Gate decomposition metadata.
- Native gate compatibility scoring.
- Gate version tracking.

## Hardware Compatibility Engine
- Circuit-to-hardware matching.
- Constraint evaluation.
- Device filtering.
- Hardware recommendation engine.
- Compatibility scoring.
- Hardware ranking.

## Fidelity & Performance Metrics
- Single-qubit gate fidelity tracking.
- Multi-qubit gate fidelity tracking.
- Measurement fidelity tracking.
- Error rate indexing.
- Reliability scoring.
- Historical performance records.

## Qubit Topology Management
- Coupling map definitions.
- Connectivity graph storage.
- Topology version tracking.
- Dynamic topology updates.
- Topology visualization metadata.

## Calibration Management
- Calibration timestamps.
- Historical calibration records.
- Device health tracking.
- Dynamic capability updates.
- Calibration snapshots.

## Coherence & Timing Metrics
- T1 coherence tracking.
- T2 coherence tracking.
- Gate duration metadata.
- Measurement timing information.
- Reset timing information.

## Hardware Benchmarking
- Quantum volume indexing.
- Benchmark repositories.
- Cross-provider comparisons.
- Historical benchmark tracking.
- Performance analytics.

## Dynamic Hardware Discovery
- Automatic device registration.
- Real-time capability updates.
- Availability tracking.
- Discovery APIs.
- Registry synchronization.

## Transpilation Intelligence
- Native gate matching.
- Transpilation cost estimation.
- Circuit adaptation metadata.
- Gate conversion analysis.
- Optimization recommendations.

## Device Health Monitoring
- Device uptime tracking.
- Maintenance schedules.
- Service status reporting.
- Reliability history.
- Incident tracking.

## Historical Device Archive
- Capability snapshots.
- Calibration history.
- Benchmark history.
- Hardware revision tracking.
- Long-term analytics.

---

# Modular Architecture

QGuardian Registry is designed as a fully modular platform for both hardware and software integration.

---

## Hardware Modules

Supports pluggable hardware definitions for:

- Superconducting quantum processors
- Trapped-ion quantum processors
- Neutral-atom quantum processors
- Photonic quantum processors
- Quantum annealers
- Topological quantum processors
- Quantum simulators
- Experimental hardware

Hardware modules may provide:

- Native gate sets
- Qubit topology
- Fidelity metrics
- Calibration data
- Benchmark information
- Device-specific metadata

---

## Provider Modules

Supports independent provider adapters.

Examples:

- IBM provider module
- IonQ provider module
- Rigetti provider module
- D-Wave provider module
- Academic hardware modules
- Private enterprise modules

Provider modules may provide:

- Device registration
- Capability synchronization
- Status updates
- Calibration updates
- Benchmark publication

---

## Software Modules

Supports integrations with:

- Quantum runtimes
- Quantum compilers
- Quantum simulators
- Benchmarking platforms
- Experiment management systems
- Workflow orchestration systems
- Research platforms

Software modules may provide:

- Compatibility engines
- Hardware recommendation systems
- Analytics tools
- Visualization systems
- Monitoring services
- Export utilities

---

## Registry Extensions

Supports optional extensions such as:

- Authentication modules
- Distributed registry services
- Monitoring systems
- Analytics engines
- Machine learning recommendation engines
- Performance prediction engines
- Transpilation estimators

---

## Storage Modules

Interchangeable storage backends:

- PostgreSQL
- SQLite
- Distributed SQL databases
- Graph databases
- Object storage systems
- In-memory databases

---

## Communication Modules

Supports multiple interfaces:

- REST APIs
- GraphQL APIs
- gRPC services
- Message queues
- Event streams
- WebSocket services

---

# Registry APIs

## Hardware Registration API
- Device registration
- Capability submission
- Metadata validation
- Version management

## Hardware Discovery API
- Device search
- Capability filtering
- Provider search
- Hardware queries

## Compatibility API
- Constraint validation
- Hardware recommendations
- Compatibility scoring
- Circuit matching

## Benchmark API
- Benchmark retrieval
- Historical comparisons
- Metrics aggregation
- Performance reporting

---

# Supported Metadata

## Device Information
- Device name
- Provider
- Architecture
- Hardware generation
- Geographic region

## Quantum Resources
- Qubit count
- Ancillary qubits
- Connectivity maps
- Native gate sets
- Measurement capabilities

## Performance Metrics
- Gate fidelities
- Readout errors
- Coherence times
- Error rates
- Queue information

## Runtime Information
- Availability
- Status
- Maintenance schedules
- Calibration timestamps
- Version information

---

# Example Use Cases

## Circuit Compatibility Matching
Determine which quantum devices can execute a circuit with minimal transpilation.

## Hardware Selection
Automatically identify hardware that satisfies circuit constraints.

## Hardware Benchmarking
Compare capabilities and performance across providers.

## Research Reproducibility
Record and share hardware capability snapshots.

## Multi-Provider Execution
Enable portable workloads across different quantum ecosystems.

## Analytics and Monitoring
Track device health and long-term performance.

---

# Integration with QGuardian
[https://roxanneardary.com/qguardian/](https://roxanneardary.com/qguardian/)

QGuardian Registry serves as the compatibility and discovery layer for:

- QGuardian — Fidelity First
- Quantum runtimes
- Quantum compilers
- Quantum simulators
- Benchmarking systems
- Experiment management platforms
- Research infrastructure

---

# Project Vision

QGuardian Registry aims to become the open, vendor-neutral source of truth for quantum hardware capabilities. By standardizing hardware descriptions and enabling automatic compatibility matching, the registry helps make quantum computing more portable, reliable, and accessible across the entire ecosystem.

---

**QGuardian Registry — The Compatibility Layer for Quantum Hardware.**
---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/qguardian-registry/](https://roxanneardary.com/qguardian-registry/)

---

## License & Notice Requirements

QGuardian Registry is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- QGuardian Registry specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

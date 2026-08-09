# QGuardian

**QGuardian - Fidelity First.**

QGuardian is an open-source quantum execution and fidelity management platform designed to improve the reliability, efficiency, and reproducibility of quantum computing workloads. It evaluates quantum circuits against hardware capabilities before execution, prioritizes native gate compatibility, enforces fidelity requirements, and selects suitable quantum hardware for each workload.

QGuardian is designed as a modular system. Essential functionality is contained within the core modules, while provider integrations, advanced optimization systems, monitoring services, and specialized tools can be added through optional plugins. This allows QGuardian to support different quantum architectures and software ecosystems without creating unnecessary dependencies within the core platform.

---

# Project Goals

- Improve quantum execution fidelity.
- Reduce unnecessary transpilation.
- Match circuits to compatible hardware.
- Minimize accumulated gate errors.
- Support multiple quantum hardware architectures.
- Provide hardware-independent execution logic.
- Improve reproducibility of quantum experiments.
- Enable modular provider and software integrations.
- Avoid vendor lock-in.
- Provide transparent hardware selection decisions.

---

# Architecture

QGuardian uses a modular architecture consisting of:

- Core Modules
- Optional Plugin Modules
- Provider Integrations
- Hardware Adapters
- Software Integrations

The core provides the fundamental execution intelligence required by QGuardian. Plugins extend those capabilities without requiring changes to the core architecture.

---

# Core Modules

## 1. Circuit Analysis Core

Analyzes quantum circuits before execution.

### Features

- Circuit parsing
- Gate identification
- Qubit count analysis
- Circuit depth analysis
- Gate frequency analysis
- Two-qubit operation analysis
- Measurement analysis
- Circuit complexity estimation
- Circuit resource estimation
- Unsupported operation detection

The Circuit Analysis Core creates a normalized representation of the workload that can be evaluated against hardware capabilities.

---

## 2. Fidelity Enforcement Core

The Fidelity Enforcement Core is the primary reliability engine of QGuardian.

### Features

- Minimum fidelity thresholds
- Single-qubit fidelity requirements
- Multi-qubit fidelity requirements
- Measurement fidelity requirements
- Error threshold enforcement
- Circuit reliability estimation
- Fidelity-based execution approval
- Fidelity-based execution rejection
- Hardware reliability scoring

Example requirements may specify:

- Minimum single-qubit fidelity
- Minimum two-qubit fidelity
- Minimum measurement fidelity
- Maximum acceptable error rate

A circuit that does not satisfy the configured requirements can be rejected before execution.

---

## 3. Native Gate Matching Core

Determines how closely a circuit matches the native instruction set of available hardware.

### Features

- Native gate detection
- Native gate set comparison
- Unsupported gate identification
- Native gate ratio calculation
- Gate conversion analysis
- Transpilation overhead estimation
- Native execution preference
- Gate compatibility scoring

The core prioritizes hardware capable of executing more of the original circuit directly.

This reduces unnecessary transformations, circuit depth, and accumulated execution error.

---

## 4. Hardware Compatibility Core

Determines whether a quantum device is capable of executing a particular workload.

### Features

- Qubit count matching
- Native gate matching
- Topology matching
- Fidelity matching
- Hardware constraint validation
- Architecture compatibility
- Measurement compatibility
- Hardware capability filtering
- Compatibility scoring

The compatibility engine produces a structured assessment of whether a device is suitable for the workload.

---

## 5. Hardware Selection Core

Selects the most appropriate available hardware based on circuit requirements.

### Features

- Hardware ranking
- Compatibility scoring
- Fidelity weighting
- Native gate weighting
- Topology weighting
- Error-rate weighting
- Hardware availability consideration
- Execution suitability scoring
- Configurable selection policies

Hardware selection policies may prioritize:

- Highest fidelity
- Lowest error rate
- Maximum native gate compatibility
- Minimum transpilation
- Lowest circuit depth
- Best overall compatibility

---

## 6. Reliability Scoring Core

Calculates an overall execution reliability score.

### Features

- Gate reliability analysis
- Circuit-level error estimation
- Fidelity aggregation
- Error accumulation estimation
- Hardware reliability scoring
- Circuit reliability scoring
- Confidence scoring
- Configurable scoring models

The reliability score provides a standardized way to compare possible execution targets.

---

## 7. Transpilation Analysis Core

Evaluates the expected impact of converting a circuit to a hardware-specific instruction set.

### Features

- Unsupported gate detection
- Gate decomposition analysis
- Additional gate estimation
- Circuit depth increase estimation
- Two-qubit gate overhead estimation
- Transpilation cost scoring
- Hardware comparison

QGuardian can use this information before execution to avoid hardware that would require excessive circuit transformation.

---

## 8. Topology Compatibility Core

Evaluates the physical connectivity requirements of a circuit against available hardware.

### Features

- Qubit connectivity analysis
- Coupling map comparison
- Logical-to-physical qubit compatibility
- Routing overhead estimation
- SWAP overhead estimation
- Topology scoring
- Connectivity-aware hardware selection

Hardware with compatible connectivity receives a higher compatibility score.

---

## 9. Execution Policy Core

Controls the rules governing whether and how a circuit may execute.

### Features

- Fidelity thresholds
- Hardware requirements
- Native gate requirements
- Qubit requirements
- Topology requirements
- Error limits
- Reliability thresholds
- Execution approval rules
- Execution rejection rules
- Fallback policies

Policies can be configured globally, per project, or per workload.

---

## 10. Backend Abstraction Core

Provides a hardware-independent interface between QGuardian and quantum execution environments.

### Features

- Standardized backend interface
- Hardware capability interface
- Execution request interface
- Result normalization
- Backend status handling
- Capability querying
- Provider-independent execution logic

This allows the QGuardian core to remain independent of individual hardware providers.

---

## 11. Configuration Core

Provides centralized configuration for QGuardian.

### Features

- Fidelity configuration
- Hardware constraints
- Native gate requirements
- Topology requirements
- Execution policies
- Scoring policies
- Plugin configuration
- Provider configuration
- Environment configuration

---

## 12. Validation Core

Validates hardware profiles, circuit requirements, configurations, and execution requests.

### Features

- Schema validation
- Configuration validation
- Hardware profile validation
- Gate definition validation
- Capability validation
- Execution request validation
- Compatibility validation

---

# Optional Plugin Modules

Optional plugins extend QGuardian without increasing the dependency footprint of the core platform.

Plugins can be installed independently according to the user's requirements.

---

## Hardware Provider Plugins

Provider plugins connect QGuardian to individual quantum hardware ecosystems.

Examples include:

- IBM hardware plugin
- IonQ hardware plugin
- Rigetti hardware plugin
- D-Wave plugin
- Academic hardware plugins
- Private hardware plugins

### Capabilities

- Device discovery
- Hardware capability retrieval
- Calibration retrieval
- Backend status
- Execution submission
- Result retrieval

---

## QGuardian Registry Plugin

Provides integration with **QGuardian Registry — The Compatibility Layer for Quantum Hardware.**

### Capabilities

- Hardware discovery
- Native gate retrieval
- Topology retrieval
- Fidelity retrieval
- Calibration retrieval
- Device capability synchronization
- Hardware profile updates

This plugin allows QGuardian to use registry data when making hardware selection decisions.

---

## Quantum Software Plugins

Optional integrations can connect QGuardian to quantum software ecosystems.

Examples include:

- Qiskit integration
- Cirq integration
- PennyLane integration
- Braket integration
- Custom quantum SDK integrations

### Capabilities

- Circuit import
- Circuit export
- Circuit conversion
- Runtime integration
- Result normalization

---

## Transpiler Plugins

Advanced transpilation systems can be integrated as optional plugins.

### Capabilities

- Hardware-specific transpilation
- Circuit optimization
- Gate decomposition
- Routing
- Circuit rewriting
- Depth optimization

The core QGuardian system determines whether transpilation is desirable, while an optional transpiler plugin performs the transformation.

---

## Error Mitigation Plugins

Optional error mitigation systems can improve execution results.

### Capabilities

- Readout error mitigation
- Zero-noise extrapolation
- Probabilistic error cancellation
- Measurement correction
- Custom mitigation strategies

---

## Benchmarking Plugins

Provide advanced hardware benchmarking capabilities.

### Capabilities

- Quantum volume benchmarking
- Circuit fidelity benchmarking
- Hardware comparison
- Performance benchmarking
- Historical benchmarking
- Custom benchmark suites

---

## Predictive Performance Plugins

Optional predictive systems can estimate hardware performance before execution.

### Capabilities

- Execution success prediction
- Error prediction
- Circuit performance prediction
- Hardware performance forecasting
- Queue-aware selection
- Historical performance modeling

---

## Machine Learning Plugins

Optional machine learning systems can enhance hardware selection and optimization.

### Capabilities

- Hardware recommendation models
- Fidelity prediction
- Error prediction
- Performance classification
- Workload classification
- Adaptive hardware selection

Machine learning is optional and is not required by the QGuardian core.

---

## Monitoring Plugins

Provide real-time monitoring capabilities.

### Capabilities

- Backend monitoring
- Device health monitoring
- Calibration monitoring
- Error-rate monitoring
- Execution monitoring
- Alerting

---

## Visualization Plugins

Provide optional graphical interfaces and dashboards.

### Capabilities

- Circuit visualization
- Hardware topology visualization
- Fidelity dashboards
- Hardware comparison
- Compatibility reports
- Execution analytics

---

## Storage Plugins

Optional storage backends can extend QGuardian's persistence capabilities.

Examples include:

- SQLite
- PostgreSQL
- Graph databases
- Distributed databases
- Cloud storage

Storage plugins allow deployments to select the persistence architecture appropriate for their environment.

---

## API Plugins

Optional interfaces can expose QGuardian functionality to external applications.

Examples include:

- REST API
- GraphQL API
- gRPC API
- WebSocket interface

---

# Hardware Abstraction

QGuardian does not assume a single quantum computing architecture.

Hardware modules can describe:

- Superconducting processors
- Trapped-ion processors
- Neutral-atom processors
- Photonic processors
- Quantum annealers
- Topological systems
- Experimental processors
- Simulators

Each hardware integration implements the standardized backend interface required by the QGuardian core.

---

# Execution Pipeline

QGuardian uses the following general execution flow:

Circuit
↓
Circuit Analysis
↓
Hardware Discovery
↓
Native Gate Matching
↓
Topology Analysis
↓
Fidelity Evaluation
↓
Transpilation Cost Analysis
↓
Reliability Scoring
↓
Hardware Ranking
↓
Execution Policy Validation
↓
Hardware Selection
↓
Optional Transpilation
↓
Execution
↓
Result Validation
↓
Execution Report

---

# Hardware Selection Model

QGuardian can calculate a composite hardware suitability score using factors such as:

- Fidelity
- Native gate compatibility
- Circuit topology compatibility
- Expected transpilation overhead
- Error rate
- Qubit availability
- Hardware status
- Historical performance

Deployments can configure the weighting of individual factors.

---

# Example Configuration
```
{
  "execution": {
    "strategy": "fidelity_first",
    "min_qubits": 32,
    "min_gate_fidelity": 0.99,
    "native_gates": [
      "CNOT",
      "RX",
      "RZ"
    ]
  },
  "topology": {
    "require_compatible_connectivity": true
  },
  "transpilation": {
    "max_additional_gates": 20,
    "max_depth_increase": 10
  },
  "reliability": {
    "minimum_score": 0.95
  }
}
```
---

# Execution Modes

## Fidelity First

Selects hardware primarily according to fidelity and reliability.

## Native First

Prioritizes hardware requiring minimal transpilation.

## Balanced

Balances fidelity, native gates, topology, and performance.

## Custom

Allows users to define their own hardware selection weights and policies.

---

# Reliability Reports

QGuardian can generate execution assessments containing:

- Selected hardware
- Rejected hardware
- Fidelity metrics
- Native gate compatibility
- Topology compatibility
- Estimated transpilation overhead
- Reliability score
- Execution policy results
- Selection rationale

This provides transparency into why a particular backend was selected.

---

# Reproducibility

QGuardian supports reproducible quantum experimentation by recording relevant execution context.

Supported information includes:

- Circuit definition
- Hardware identifier
- Hardware capability profile
- Fidelity requirements
- Gate set
- Topology
- Calibration timestamp
- Selection policy
- Compatibility score
- Reliability score
- Execution configuration

---

# Security and Isolation

The core platform is designed to isolate provider-specific functionality from core execution logic.

Security features may include:

- Plugin isolation
- Credential separation
- Provider authentication
- Configuration validation
- Permission controls
- Secure backend communication
- Audit logging through optional plugins

---

# Design Principles

## Modular

Core functionality remains independent from optional integrations.

## Hardware Agnostic

QGuardian is designed to support multiple quantum hardware architectures.

## Provider Neutral

No individual quantum hardware provider is required by the core platform.

## Fidelity First

Execution reliability is a fundamental design priority.

## Native Gate Aware

Hardware-native execution is preferred whenever practical.

## Transparent

Hardware selection decisions should be explainable and inspectable.

## Extensible

New hardware, software, algorithms, and services can be added through plugins.

## Efficient

QGuardian aims to reduce unnecessary transpilation, routing, and execution overhead.

## Reproducible

Hardware and execution conditions can be recorded for repeatable experimentation.

## Vendor Neutral

The architecture avoids unnecessary dependence on a single provider or software ecosystem.

---

# Core vs Plugin Philosophy

The QGuardian core contains functionality required to perform its fundamental mission:

- Analyze circuits.
- Understand hardware requirements.
- Match native gates.
- Evaluate topology.
- Enforce fidelity.
- Score reliability.
- Select hardware.
- Apply execution policies.

Plugins provide functionality that is useful but not required for every deployment:

- Provider-specific integrations.
- Quantum SDK integrations.
- Advanced transpilers.
- Error mitigation.
- Machine learning.
- Monitoring.
- Visualization.
- Additional storage.
- External APIs.

This separation keeps the core lightweight while allowing QGuardian to scale into a complete quantum execution ecosystem.

---

# Project Ecosystem

QGuardian is designed to work as part of a larger open-source quantum infrastructure ecosystem.

## QGuardian

**QGuardian — Fidelity First.**

The fidelity enforcement and intelligent hardware selection engine.

## [QGuardian Registry](https://gitlab.com/Roxanne_Ardary/qguardian-registry)  

**QGuardian Registry — The Compatibility Layer for Quantum Hardware.**

The hardware capability and compatibility registry supporting QGuardian's hardware intelligence.

Together:
```
Circuit
↓
QGuardian Registry
↓
Hardware Compatibility
↓
QGuardian
↓
Fidelity Enforcement
↓
Hardware Selection
↓
Quantum Execution
```
---

# Future Development

Potential future modules include:

- Distributed hardware discovery
- Advanced circuit reliability prediction
- Adaptive hardware selection
- Cross-provider workload orchestration
- Real-time fidelity optimization
- Automated hardware benchmarking
- Predictive calibration analysis
- Federated hardware registries
- Quantum workload scheduling
- Advanced error-aware compilation

These capabilities should be implemented as core functionality only when they become fundamental to QGuardian's mission. Otherwise, they should remain optional plugins.  

---

# Vision

QGuardian is designed to make quantum execution more intelligent, reliable, and hardware-aware.

Rather than treating quantum hardware as interchangeable execution targets, QGuardian evaluates the actual capabilities and limitations of each system before committing a workload.  

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
  - [https://roxanneardary.com/qguardian/](https://roxanneardary.com/qguardian/)

---

## License & Notice Requirements

QGuardian is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- QGuardian specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

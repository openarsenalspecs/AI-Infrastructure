# Nix Flakes Configuration

A reproducible, modular Nix Flakes configuration for managing multiple desktops, laptops, build systems, cache servers, and self-hosted infrastructure from a declarative source of truth.

## Overview

Nixfiles is a personal multi-host Nix Flakes configuration designed to provide consistent, reproducible, and maintainable system environments across physical and remote machines. The configuration supports computers with different hardware profiles and infrastructure roles while allowing common functionality to be shared through reusable Nix modules.

The system is designed around declarative configuration, reproducible builds, modular components, and isolated development environments. Host-specific requirements can be combined with shared functionality without requiring each machine to maintain an independent configuration.

Nixfiles also provides development environments through Nix devShells. These environments make development tools and dependencies available without requiring permanent installation into the host system, helping maintain consistent workflows across machines.

## Design Principles

- Declarative system configuration
- Reproducible environments and builds
- Modular and reusable Nix components
- Shared functionality across hosts
- Host-specific configuration where required
- Isolated development environments
- Local and remote build support
- Build and cache infrastructure
- Minimal dependency on host-level configuration
- Support for rollback and reproducible system states
- Extensible architecture through optional plugins
- Avoidance of unnecessary vendor lock-in

## Core Modules

### Host Configuration

Provides the foundational configuration layer for individual machines.

Features include:

- Host-specific system configuration
- Hardware-specific settings
- Boot configuration
- Filesystem configuration
- Kernel configuration
- Network configuration
- User and group configuration
- System services
- Host-specific packages
- Shared configuration inheritance

The host configuration module allows each machine to retain its unique requirements while consuming common functionality from the rest of the system.

### Shared System Configuration

Provides common configuration that can be reused across multiple hosts.

Features include:

- Shared system packages
- Common system services
- Environment configuration
- Shell configuration
- System-wide defaults
- Common security settings
- Shared Nix configuration
- Consistent system behavior across hosts

### Package and Tooling Configuration

Provides declarative management of software and command-line tooling.

Features include:

- System packages
- Development utilities
- Build utilities
- Command-line tools
- Host-specific packages
- Shared package definitions
- Reproducible package selection

### Build Infrastructure

Provides configuration for distributed and dedicated build systems.

Features include:

- Local build support
- Remote build support
- Dedicated build hosts
- Backup builders
- Build resource distribution
- Reproducible build environments
- Integration with Nix build workflows

The build infrastructure allows computationally intensive builds to be distributed across available systems rather than requiring every host to perform every build locally.

### Cache Infrastructure

Provides support for binary caching and efficient distribution of previously built Nix packages.

Features include:

- Attic cache integration
- Remote binary caches
- Reduced rebuild requirements
- Faster system deployment
- Shared build artifacts
- Cache-oriented infrastructure configuration

### Development Shells

Provides reproducible development environments that can be entered independently of the host's permanent system configuration.

Development shells support:

- Isolated development dependencies
- Reproducible toolchains
- Project-specific development environments
- Consistent tooling across hosts
- Nix-based dependency management

### Rust Development Shell

Provides a dedicated Rust development environment for building and maintaining Rust software.

The Rust shell includes:

- Stable Rust toolchain
- `rustc`
- `cargo`
- `rustfmt`
- `clippy`
- `rust-analyzer`
- `cargo-watch`
- `cargo-expand`
- `cargo-outdated`
- System libraries commonly required by Rust crates
- Reproducible Rust development dependencies

The environment can be entered with `nix develop .#rust` and can be integrated with `direnv` for automatic project environment activation.

The Rust shell is isolated from the host system, allowing Rust development tools and dependencies to remain consistent without requiring a global Rust installation.

## Optional Plugin Modules

Optional plugin modules extend the core configuration without requiring additional functionality on every host.

### Additional Development Environments

Optional development shells can provide reproducible environments for additional programming languages, frameworks, and development workflows.

Potential integrations include:

- Python
- Node.js
- Go
- C and C++
- WebAssembly
- Cross-compilation
- Documentation tooling
- Language-specific development utilities

### Additional Build Backends

Optional build modules can extend the build infrastructure with additional builders and specialized build environments.

Possible functionality includes:

- Additional remote builders
- Architecture-specific builders
- Temporary build workers
- Specialized compilation environments
- CI-oriented build environments

### Additional Cache Backends

Optional cache modules can provide integrations with additional binary cache services and storage systems.

### Monitoring and Administration

Optional modules can provide additional monitoring, diagnostics, logging, and administrative functionality for hosts and infrastructure.

### Self-Hosted Services

Optional modules can define services intended for dedicated infrastructure hosts.

These modules can provide declarative configuration for services while keeping service-specific requirements separate from the core system configuration.

### Cross-Compilation

Optional cross-compilation modules can provide reproducible environments for building software for architectures and platforms different from the host.

## Reproducibility

Nixfiles is designed to make system configuration and development environments reproducible across supported hosts. Nix Flakes provide pinned inputs and declarative definitions that make it possible to recreate environments consistently.

This approach reduces configuration drift, simplifies system recovery, and makes it easier to move development workloads between machines.

## Multi-Host Infrastructure

The configuration supports a range of host roles, including:

- Primary desktop systems
- Laptop systems
- Backup build systems
- Dedicated build servers
- Binary cache servers
- Self-hosted application servers

Each host can consume shared modules while retaining configuration specific to its hardware and operational role.

## Rust Development

The Rust development shell provides a complete development environment without requiring Rust tooling to be installed globally on the host.

It combines the Rust compiler and Cargo package manager with formatting, linting, language-server support, Cargo utilities, and native libraries needed by common Rust projects. This makes it suitable for development, testing, dependency management, code inspection, and iterative compilation.

The environment can be launched with:

    nix develop .#rust

When used with direnv, the development environment can also be activated automatically when entering a project directory.

## Extensibility

The modular architecture allows additional functionality to be added without changing the fundamental design of the configuration.

Core modules provide the functionality required by the existing infrastructure, while optional plugin modules can introduce specialized capabilities when needed. This keeps the base configuration focused while providing a clear path for future expansion.

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
  - [https://roxanneardary.com/nixfiles/](https://roxanneardary.com/nixfiles/)

---

## License & Notice Requirements

nixfiles is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- nixfiles specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.  
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

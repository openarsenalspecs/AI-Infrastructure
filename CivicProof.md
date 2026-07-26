# CivicProof  
### A commons for identity verification.

CivicProof is an open-source identity verification and trust infrastructure designed as a public commons for the digital world. It replaces closed, centralized KYC and e-signature systems with a transparent, cryptographically verifiable, and user-controlled framework for proving identity, consent, and authenticity.

Built under the **AGPL 3.0+ license**, CivicProof ensures that identity infrastructure remains open, auditable, and resistant to monopolization—so verification becomes a shared public utility rather than a proprietary service.

---

## Mission

CivicProof exists to make identity verifiable without requiring centralized control, data extraction, or permanent surveillance. It enables individuals to generate cryptographic proofs of identity, document authenticity, and verification events while retaining full ownership of their data.

---

## Core Principles

- Identity is user-owned, not platform-owned  
- Verification is cryptographic, not institutional  
- Trust is proven, not assumed  
- AI assists verification but never defines truth  
- Systems must be open, forkable, and auditable  
- Data minimization is the default  

---

## Full Feature Set

### 1. Self-Sovereign Identity (SSI) Layer
- Decentralized Identifiers (DIDs)
- Verifiable Credentials (W3C standard)
- Local-first identity wallets
- Key rotation and recovery mechanisms
- Multi-device identity synchronization

---

### 2. Document Verification System
- Secure document upload and processing
- ID parsing (passports, licenses, national IDs)
- Structured data extraction from documents
- Tamper detection and integrity validation
- Cryptographic document hashing and signing

---

### 3. AI-Powered Verification Layer (Optional & Local-First)
- OCR-based document understanding
- Face detection and matching
- Identity embedding comparison
- Fraud pattern detection
- Document layout interpretation

Supported open models:
- PaddleOCR
- LayoutLMv3
- InsightFace
- MediaPipe
- YOLOv8
- DINOv2 (embeddings)

---

### 4. Liveness Detection System
- Active liveness challenges (blink, motion prompts)
- Passive liveness detection (no interaction required)
- Replay attack detection (screen/video spoofing prevention)
- Depth and motion consistency analysis
- On-device processing support

---

### 5. KYC Policy Engine (Modular)
- Configurable verification rules per use case
- Jurisdiction-based compliance profiles
- Pluggable identity verification providers
- Zero-knowledge verification modes (where applicable)
- Optional external API integration layer

---

### 6. Cryptographic Trust Layer
- Digital signatures (Ed25519 / secp256k1)
- Hash-based document integrity verification
- Post-quantum cryptography readiness (CRYSTALS-Dilithium, Falcon)
- Secure key management system
- Optional hardware wallet support

---

### 7. Zero-Knowledge & Privacy Systems
- Selective disclosure credentials
- Proof-of-attribute verification (e.g., age without identity exposure)
- Privacy-preserving verification outputs
- Minimal data exposure by default
- Ephemeral verification modes

---

### 8. Verification Output System (CVO Standard)
Every verification generates a structured object:

- Verification type (identity, document, liveness, age, etc.)
- Cryptographic signature
- Timestamp
- Expiration (optional)
- Scope of disclosure
- Verification method metadata

---

### 9. Identity Wallet System
- Store verifiable credentials locally
- Control disclosure permissions per verification
- Revoke or rotate credentials
- Export/import identity packages
- Cross-platform portability

---

### 10. Modular Architecture
CivicProof is fully composable:

- Identity ingestion module
- OCR/document parsing module
- Liveness detection module
- Face verification module
- Credential issuance module
- Policy engine module
- Cryptographic signing module

All modules are replaceable without breaking the system.

---

### 11. Interoperability Layer
- W3C DID & Verifiable Credentials compatibility
- OpenPGP integration support
- IPFS-compatible storage systems
- External KYC system adapters
- Future identity standard compatibility

---

### 12. Security Model
- Zero-trust verification architecture
- Client-side encryption by default
- Ephemeral processing where possible
- No required biometric storage
- Fully auditable verification pipelines

---

## System Philosophy

CivicProof is not a platform. It is a **verification commons**.

It is designed to function as:
- Public infrastructure for trust
- A cryptographic identity layer for the internet
- A forkable system that prevents monopoly over identity verification

---

## Threat Model

CivicProof is designed to resist:

- Deepfake identity spoofing  
- Document forgery and tampering  
- Replay attacks  
- Centralized identity harvesting  
- Silent biometric data collection  
- AI model manipulation in verification pipelines  

It does not attempt to solve:
- Physical coercion  
- Legal identity disputes outside cryptographic scope  
- Device-level compromise  

---

## Founding Principle

> Proof without exposure.

Identity must be verifiable without requiring unnecessary disclosure.

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
  - [https://roxanneardary.com/civicproof/](https://roxanneardary.com/civicproof/)

---

## License & Notice Requirements

CivicProof is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- CivicProof specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

# TruthInBilling

**Real Bills. Real Patterns. Real Transparency.**

TruthInBilling is an open-source, privacy-preserving public billing transparency platform designed to collect, verify, structure, and analyze documented discrepancies between advertised pricing, contractual terms, regulatory requirements, and actual billed charges.

The platform transforms individual billing records into a structured public dataset that can reveal recurring patterns across companies, industries, and jurisdictions while protecting the identity and sensitive information of contributors.

---

## Mission

TruthInBilling exists to make billing discrepancies measurable, verifiable, and visible.

Consumers frequently encounter unexpected fees, incorrect charges, pricing inconsistencies, and billing practices that may not match advertised rates or applicable requirements. Individual incidents can be difficult to evaluate in isolation.

TruthInBilling provides infrastructure for collecting documented evidence, verifying submissions, protecting contributor information, and identifying patterns across large numbers of billing records.

---

## Core Principles

- **Evidence over allegations**
- **Verification without public exposure**
- **Privacy by design**
- **Transparent methodology**
- **Structured public data**
- **Open-source infrastructure**
- **Human review and accountability**
- **No vendor lock-in**
- **Modular architecture**
- **Interoperable data**

---

# Specification

TruthInBilling is designed as a modular system consisting of independent core modules and optional plugin modules.

Core modules provide the foundational capabilities required to operate the TruthInBilling platform. Optional plugins extend the platform for specialized industries, verification providers, analytics systems, regulatory databases, storage systems, and external integrations.

Modules should communicate through documented interfaces and standardized data structures so that individual components can be replaced, extended, or independently maintained.

---

# Core Modules

## 1. Identity & Verification Module

Provides privacy-preserving verification of contributors.

### Features

- KYC-style contributor verification
- Verified account creation
- Identity verification status
- Separation of identity information from billing submissions
- Privacy-preserving contributor identifiers
- Duplicate account detection
- Verification lifecycle management
- Verification audit records
- Access controls for protected identity information

The public database does not expose contributor identities.

---

## 2. Submission Module

Provides the primary workflow for submitting billing discrepancy records.

### Features

- Billing discrepancy submissions
- Bill and invoice uploads
- Receipt uploads
- Supporting documentation
- Advertised pricing documentation
- Contractual pricing information
- Relevant regulatory references
- Structured discrepancy descriptions
- Submission status tracking
- Draft submissions
- Submission validation
- Submission version history

---

## 3. Document Security Module

Provides secure handling of submitted billing documentation.

### Features

- Encrypted document storage
- Encryption at rest
- TLS-protected transmission
- Secure document processing
- File integrity verification
- Cryptographic document hashing
- Tamper-evident records
- Document access controls
- Secure deletion workflows
- Document metadata management

---

## 4. Privacy & Redaction Module

Protects sensitive information contained in submitted documents.

### Features

- Client-side redaction
- Automated sensitive-data detection
- Personally identifiable information detection
- Account number detection
- Address detection
- Telephone number detection
- Email detection
- Payment information detection
- Manual redaction controls
- Redaction verification
- Separation of public and private document representations

---

## 5. Billing Data Module

Provides the standardized data model for billing records.

### Features

- Company identification
- Industry classification
- Service classification
- Geographic classification
- State and jurisdiction information
- Billing period
- Advertised amount
- Contracted amount
- Actual billed amount
- Difference calculations
- Fee classification
- Tax classification
- Discount classification
- Discrepancy categorization
- Evidence references
- Record status

The billing data model should remain industry-neutral while supporting industry-specific extensions.

---

## 6. Evidence & Provenance Module

Maintains the relationship between reported discrepancies and supporting evidence.

### Features

- Evidence attachment
- Source references
- Document hashes
- Evidence timestamps
- Submission provenance
- Source classification
- Evidence status
- Evidence verification
- Chain-of-custody metadata
- Historical evidence versions
- Public evidence summaries

TruthInBilling records what has been submitted and verified rather than automatically declaring that a company has violated a law.

---

## 7. Regulatory Reference Module

Provides structured references to laws, regulations, tariffs, orders, and other authoritative requirements.

### Features

- State law references
- Federal law references
- Administrative regulations
- Regulatory orders
- Utility tariffs
- Public regulatory documents
- Regulatory citation metadata
- Jurisdiction classification
- Effective dates
- Expiration dates
- Source URLs
- Regulatory evidence relationships

---

## 8. Pricing & Rate Comparison Module

Compares documented pricing information against actual billing records.

### Features

- Advertised rate comparison
- Contract rate comparison
- Published rate comparison
- Promotional rate comparison
- Actual billed rate comparison
- Fee comparison
- Rate history
- Effective-date tracking
- Pricing source references
- Difference calculations
- Percentage variance calculations

---

## 9. Discrepancy Analysis Module

Provides structured analysis of reported billing differences.

### Features

- Discrepancy classification
- Recurring discrepancy detection
- Duplicate pattern detection
- Company-level analysis
- Industry-level analysis
- Geographic analysis
- Rate variance analysis
- Fee pattern analysis
- Historical comparisons
- Frequency analysis
- Aggregated statistics
- Pattern confidence indicators

Analytics should distinguish between documented facts, reported observations, and system-generated analysis.

---

## 10. Public Transparency Module

Provides the public-facing transparency layer.

### Features

- Public discrepancy records
- Aggregated billing statistics
- Company-level summaries
- Industry summaries
- State-level summaries
- Geographic visualization
- Historical trends
- Public evidence summaries
- Methodology documentation
- Verification indicators
- Data provenance indicators

Public views must exclude protected personal information.

---

## 11. Search & Discovery Module

Provides searchable access to public TruthInBilling data.

### Features

- Company search
- Industry search
- State search
- Issue-type search
- Billing category search
- Date filtering
- Pricing filtering
- Discrepancy filtering
- Verified-record filtering
- Evidence availability filtering
- Advanced search
- Structured query support

---

## 12. Public API Module

Provides programmatic access to eligible public data.

### Features

- REST API
- Structured data endpoints
- Search endpoints
- Aggregation endpoints
- Company endpoints
- Industry endpoints
- Geographic endpoints
- Regulatory reference endpoints
- Dataset exports
- API documentation
- Rate limiting
- Access controls
- Public-data-only responses

Private contributor and protected document information must never be exposed through public API endpoints.

---

## 13. Audit & Integrity Module

Maintains system-level accountability.

### Features

- Audit logs
- Record versioning
- Cryptographic hashes
- Tamper-evident records
- Administrative action logging
- Data modification history
- Verification history
- Evidence history
- Access logging
- Integrity verification

---

## 14. Governance Module

Provides transparent rules for managing the platform and its data.

### Features

- Submission review workflows
- Evidence review
- Dispute handling
- Record correction procedures
- Data quality controls
- Moderation workflows
- Contributor permissions
- Administrative permissions
- Governance records
- Methodology publication
- Transparency reporting

---

## 15. Data Export & Research Module

Makes eligible public information useful for researchers and watchdog organizations.

### Features

- CSV exports
- JSON exports
- Structured datasets
- Aggregated datasets
- Research downloads
- Historical datasets
- Data dictionaries
- Schema documentation
- Provenance metadata
- Public API access

---

# Optional Plugin Modules

Optional plugins extend TruthInBilling without requiring specialized functionality to become part of the core platform.

Plugins should use documented interfaces and should not require changes to the core data model unless a capability is broadly applicable across industries.

---

## Industry Plugins

Industry-specific plugins may provide specialized billing models and terminology.

Examples include:

- Utility Billing Plugin
- Telecommunications Billing Plugin
- Internet Service Billing Plugin
- Insurance Billing Plugin
- Medical Billing Plugin
- Property Management Billing Plugin
- Subscription Billing Plugin
- Financial Services Billing Plugin
- Transportation Billing Plugin
- Government Services Billing Plugin

---

## Regulatory Plugins

Regulatory plugins can connect TruthInBilling to external regulatory information.

Examples include:

- Federal Regulatory Database Plugin
- State Regulatory Database Plugin
- Utility Tariff Plugin
- Municipal Ordinance Plugin
- Regulatory Filing Plugin
- Government Document Plugin

---

## Verification Plugins

Verification providers can be integrated without making a specific provider part of the core system.

Examples include:

- Identity Verification Plugin
- Document Verification Plugin
- Business Verification Plugin
- Credential Verification Plugin
- External KYC Provider Plugin

---

## Document Processing Plugins

Optional document processing systems can extend document analysis capabilities.

Examples include:

- OCR Plugin
- PDF Analysis Plugin
- Image Analysis Plugin
- Advanced Redaction Plugin
- Document Classification Plugin
- Invoice Parsing Plugin

---

## Analytics Plugins

Additional analytical capabilities can be added independently.

Examples include:

- Machine Learning Pattern Detection Plugin
- Statistical Analysis Plugin
- Anomaly Detection Plugin
- Pricing Trend Plugin
- Geographic Analysis Plugin
- Industry Benchmark Plugin
- Recurring Fee Detection Plugin

---

## Data Source Plugins

External public data sources can be connected through plugins.

Examples include:

- Public Rate Database Plugin
- Government Data Plugin
- Regulatory Data Plugin
- Public Contract Database Plugin
- Corporate Pricing Archive Plugin
- Historical Rate Database Plugin

---

## Storage Plugins

TruthInBilling can support alternative storage implementations through plugins.

Examples include:

- S3-Compatible Storage Plugin
- Local Storage Plugin
- Distributed Storage Plugin
- Federated Storage Plugin
- Archive Storage Plugin

---

## Notification Plugins

Optional notification systems can provide user and administrative notifications.

Examples include:

- Email Notification Plugin
- SMS Notification Plugin
- Webhook Plugin
- Administrative Alert Plugin
- Regulatory Alert Plugin

---

## Visualization Plugins

Additional visualization systems can extend the public transparency layer.

Examples include:

- Advanced Geographic Mapping Plugin
- Statistical Visualization Plugin
- Industry Dashboard Plugin
- Historical Timeline Plugin
- Public Data Explorer Plugin

---

# Modular Architecture

TruthInBilling should maintain a clear separation between:

1. **Core platform services**
2. **Sensitive identity infrastructure**
3. **Private evidence storage**
4. **Public structured data**
5. **Optional plugins**
6. **External integrations**

Plugins should communicate through documented APIs, events, schemas, and service interfaces.

A plugin should not require users to adopt a proprietary platform or vendor-specific infrastructure.

---

# Privacy Architecture

Privacy is a foundational component of TruthInBilling.

The platform is designed around the principle that **verification and transparency do not require public exposure of identity**.

Protected information should remain separated from public billing records.

Public records should contain only the information necessary to understand the documented billing discrepancy and its supporting evidence.

---

# Verification Model

TruthInBilling uses a verification-oriented model rather than an unrestricted anonymous reporting model.

Verification can establish that a submission originates from a verified contributor without publicly identifying that contributor.

Verification status may be represented through structured indicators such as:

- Verified contributor
- Verified document
- Verified source
- Verified rate
- Verified regulatory reference
- Community reviewed
- System analyzed

Verification levels should clearly distinguish what has actually been verified.

---

# Evidence Model

TruthInBilling should distinguish between:

- User-reported information
- Uploaded documentation
- Publicly advertised pricing
- Contractual information
- Regulatory information
- System calculations
- Community review
- Independently verified information

The platform should never represent an unverified allegation as an established fact.

---

# Public Data Model

Public records may include:

- Company
- Industry
- State
- Service category
- Billing period
- Advertised price
- Contract price
- Actual billed price
- Discrepancy amount
- Discrepancy percentage
- Fee category
- Regulatory reference
- Evidence status
- Verification status
- Submission date
- Record identifier

Personally identifiable information and protected contributor information must remain outside the public dataset.

---

# Security Requirements

The implementation should support:

- Encryption at rest
- Encryption in transit
- Strong authentication
- Role-based access controls
- Least-privilege access
- Secure secret management
- Cryptographic hashing
- Audit logging
- Secure document handling
- Vulnerability management
- Dependency monitoring
- Security testing
- Data retention controls
- Secure deletion

Security implementations should be reviewed continuously as the project evolves.

---

# Suggested Technology Stack

The initial architecture is designed to support:

### Frontend

- React
- TypeScript
- Accessible component architecture
- Data visualization tooling

### Backend

- Python
- FastAPI
- REST APIs
- Background processing services

### Database

- PostgreSQL
- Structured relational data
- Geographic extensions where appropriate

### Document Storage

- S3-compatible encrypted object storage
- Secure document lifecycle management

### Security

- Modern encryption standards
- TLS
- Cryptographic hashing
- Role-separated access controls
- Privacy-preserving verification

### Infrastructure

- Docker
- Terraform
- GitLab CI/CD
- Reproducible deployment configuration

Individual implementations may be replaced as long as they maintain the documented interfaces and security requirements.

---

# Open Source Development

TruthInBilling is designed to remain open source and vendor-neutral.

The core platform should not depend on proprietary services for essential functionality when an interoperable alternative can provide the same capability.

Optional third-party services should be implemented as plugins whenever practical.

---

# Data Integrity

TruthInBilling prioritizes accurate and reproducible records.

The system should preserve:

- Original submission metadata
- Evidence relationships
- Verification status
- Record history
- Calculation methodology
- Source information
- Modification history

Changes to public records should be auditable.

---

# Legal and Responsible Use

TruthInBilling is intended to document and analyze billing information.

The platform should not automatically determine that a company has committed fraud, violated a law, or engaged in unlawful conduct.

Records should clearly distinguish documented billing differences from legal conclusions.

Regulatory references should identify the applicable source rather than automatically asserting that a violation occurred.

---

# Future Extensibility

The modular architecture allows TruthInBilling to expand into additional areas without redesigning the core platform.

Potential future capabilities include:

- Consumer billing comparison
- Public rate archives
- Regulatory monitoring
- Industry benchmarking
- Automated discrepancy detection
- Public-interest research tools
- Regulatory reporting tools
- Historical pricing intelligence
- Federated public datasets
- Independent verification networks

---

# Contributing

Contributions are welcome from developers, researchers, security professionals, data specialists, documentation contributors, and other participants interested in billing transparency.

Please review `CONTRIBUTING.md` before submitting changes.

---

## Project

**TruthInBilling**

**Real Bills. Real Patterns. Real Transparency.**

TruthInBilling is designed to turn individual billing records into a secure, verified, structured public resource that can help reveal patterns that would otherwise remain invisible.

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
  - [https://roxanneardary.com/truthinbilling/](https://roxanneardary.com/truthinbilling/)

---

## License & Notice Requirements

TruthInBilling is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- TruthInBilling specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

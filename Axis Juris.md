# Axis Juris
**Law, aligned.**
- HTML Mirror:  [https://roxanneardary.com/axisjuris-specification/](https://roxanneardary.com/axisjuris-specification/)  

---

## Specification Overview

Axis Juris is an open-source, modular AI legal intelligence system specializing in U.S. patent law, patent applications, case law, legal research, jurisdiction-aware analysis, and continuous monitoring of legal developments.

The system is designed as a source-driven legal intelligence platform rather than a general-purpose chatbot. Axis Juris connects statutes, regulations, cases, patents, applications, jurisdictions, legal doctrines, and temporal changes into a structured legal knowledge system that can be queried and analyzed by AI.

The architecture must support expansion from U.S. federal patent law into U.S. state jurisdictions, Canadian provinces and territories, other countries, and additional legal domains without requiring changes to the underlying core architecture.

Axis Juris must prioritize authoritative sources, traceable citations, cross-references, temporal accuracy, jurisdictional applicability, transparency, and human review.

## Core Design Principles

- Modular architecture
- Open-source implementation
- AGPL-3.0+ licensing
- Source-first legal intelligence
- Mandatory source attribution
- Mandatory cross-referencing
- Jurisdiction-aware reasoning
- Temporal legal awareness
- Continuous legal update capability
- Human-in-the-loop review
- Explainable AI analysis
- Auditable data processing
- Extensible jurisdiction support
- Extensible legal-domain support
- Local and self-hosted deployment capability
- Vendor-neutral architecture
- Pluggable AI providers
- Pluggable data sources
- Pluggable notification systems
- Separation of authoritative legal material from AI interpretation

---

## Core AI Reasoning Module

The Core AI Reasoning Module provides the primary intelligence and reasoning capabilities of Axis Juris.

### Features

- Natural-language legal queries
- Legal issue identification
- Legal concept identification
- Context-aware reasoning
- Multi-step legal analysis
- Statutory interpretation assistance
- Regulatory interpretation assistance
- Case law reasoning
- Legal doctrine identification
- Legal argument mapping
- Issue, rule, application, and conclusion analysis
- Distinction between legal authority and AI inference
- Distinction between established law and uncertain interpretation
- Confidence assessment
- Source-quality assessment
- Contradictory-authority detection
- Outdated-law detection
- Temporal reasoning
- Jurisdiction-aware reasoning
- Human-review escalation
- Persistent research context
- User-defined research contexts
- Structured legal research responses

The module must not present AI-generated conclusions as authoritative legal determinations.

## Patent Law Module

The Patent Law Module provides specialized intelligence for U.S. patent law.

### Features

- U.S. patent law analysis
- Title 35 United States Code analysis
- Patent eligibility analysis
- Section 101 analysis
- Novelty analysis
- Section 102 analysis
- Obviousness analysis
- Section 103 analysis
- Anticipation analysis
- Prior-art analysis
- Claim construction analysis
- Claim scope analysis
- Patent infringement analysis
- Direct infringement analysis
- Indirect infringement analysis
- Literal infringement analysis
- Doctrine of equivalents analysis
- Enablement analysis
- Written-description analysis
- Definiteness analysis
- Patent ownership analysis
- Inventorship analysis
- Assignment analysis
- Patent prosecution analysis
- Patent maintenance analysis
- Patent expiration analysis
- Patent term analysis
- Patent enforceability analysis
- Patent validity analysis
- Patent litigation research
- Patent prosecution research
- Patent portfolio analysis

## Patent Application Module

The Patent Application Module assists users in analyzing and developing patent applications.

### Features

- Invention disclosure analysis
- Technical disclosure structuring
- Patent application analysis
- Claim drafting assistance
- Independent claim analysis
- Dependent claim analysis
- Claim hierarchy analysis
- Claim dependency validation
- Claim terminology analysis
- Specification consistency checking
- Abstract analysis
- Background analysis
- Summary analysis
- Detailed description analysis
- Embodiment analysis
- Figure reference validation
- Terminology consistency checking
- Claim-to-specification support mapping
- Written-description risk detection
- Enablement risk detection
- Definiteness risk detection
- Claim scope analysis
- Alternative embodiment identification
- Claim refinement assistance
- Application version comparison
- Amendment analysis
- Prosecution-history-aware analysis

The module must identify potential legal or drafting issues without representing its output as a substitute for professional legal representation.

## Case Law Intelligence Module

The Case Law Intelligence Module provides structured analysis of judicial decisions and precedent.

### Features

- Case law search
- Case identification
- Case summarization
- Holding extraction
- Rule extraction
- Reasoning extraction
- Factual-background extraction
- Procedural-history extraction
- Majority-opinion analysis
- Concurring-opinion analysis
- Dissent analysis
- Precedent identification
- Binding-authority identification
- Persuasive-authority identification
- Case similarity analysis
- Case distinction analysis
- Treatment-of-precedent tracking
- Overruling detection
- Reversal tracking
- Affirmance tracking
- Citation-network analysis
- Judicial-doctrine tracking
- Doctrine evolution analysis
- Legal trend analysis
- Case timeline generation
- Court hierarchy analysis
- Judicial jurisdiction mapping

## Legal Knowledge Graph Module

The Legal Knowledge Graph Module provides the structured representation of legal authorities and their relationships.

### Legal Entities

- Statutes
- Regulations
- Cases
- Courts
- Agencies
- Jurisdictions
- Patents
- Patent applications
- Claims
- Inventors
- Assignees
- Legal doctrines
- Legislative actions
- Regulatory actions
- Legal publications
- Treaties
- Administrative decisions

### Relationships

- Statute-to-case relationships
- Case-to-case relationships
- Regulation-to-statute relationships
- Patent-to-case relationships
- Patent-to-prior-art relationships
- Claim-to-specification relationships
- Claim-to-prior-art relationships
- Amendment relationships
- Repeal relationships
- Overruling relationships
- Reversal relationships
- Affirmation relationships
- Citation relationships
- Jurisdictional relationships
- Temporal relationships
- Authority relationships

### Features

- Legal entity indexing
- Relationship mapping
- Authority hierarchy mapping
- Citation graph construction
- Legal dependency mapping
- Historical relationship preservation
- Temporal relationship tracking
- Cross-reference generation
- Graph-based legal discovery
- Graph-based precedent analysis

## Source & Citation Module

The Source & Citation Module ensures that legal analysis remains traceable to authoritative sources.

### Features

- Mandatory citations for substantive legal claims
- Official-source prioritization
- Statutory citations
- Regulatory citations
- Case citations
- Court-document citations
- Patent-document citations
- Legislative citations
- Administrative-agency citations
- Source provenance
- Source-date tracking
- Effective-date tracking
- Source-version tracking
- Citation validation
- Citation-to-claim mapping
- Cross-reference generation
- Primary-authority identification
- Secondary-authority identification
- Source reliability assessment
- Source conflict detection
- Legal evidence trails
- Traceable AI reasoning references

The system should prefer primary and authoritative sources whenever available.

## Legal Update & Monitoring Module

The Legal Update Module continuously monitors changes that may affect the legal knowledge base.

### Features

- Federal legislation monitoring
- State legislation monitoring
- Regulatory monitoring
- Court decision monitoring
- USPTO update monitoring
- Federal Register monitoring
- Administrative guidance monitoring
- Legal bulletin monitoring
- New-law detection
- Amendment detection
- Repeal detection
- New-precedent detection
- Precedent-status detection
- Effective-date detection
- Delayed-effective-date tracking
- Proposed-rule tracking
- Final-rule tracking
- Emergency-rule tracking
- Legal-version tracking
- Historical-law preservation
- Change-diff analysis
- Source-change tracking
- Update provenance
- Update validation
- Update rollback capability

The update system must distinguish proposed, pending, enacted, effective, expired, repealed, stayed, overturned, and otherwise inactive legal authorities where applicable.

## Jurisdiction Engine Module

The Jurisdiction Engine determines which legal authorities are relevant to a user's circumstances.

### Features

- U.S. federal jurisdiction
- U.S. state jurisdiction
- Court-specific jurisdiction
- Geographic jurisdiction mapping
- Legal authority hierarchy
- Applicable-law determination
- Federal and state interaction analysis
- Jurisdiction conflict detection
- Jurisdiction-specific effective dates
- User-selected jurisdiction profiles
- Location-aware legal context
- Multi-jurisdiction comparison
- Cross-jurisdiction analysis
- Jurisdiction-specific source selection
- Jurisdiction-specific legal alerts

The system must not assume that a user's physical location alone determines every applicable law. Legal applicability must also consider the nature of the issue, governing authority, parties, venue, transaction, publication, and other relevant circumstances.

## State Law Module

The State Law Module provides extensible support for U.S. state-level legal information where relevant to a user's legal context.

### Features

- Fifty-state jurisdiction framework
- State statutory monitoring
- State regulatory monitoring
- State case law integration
- State court hierarchy
- State-specific legal rules
- State-specific terminology
- State-specific effective dates
- State-specific legal alerts
- State law comparison
- Interstate legal comparison
- Interstate conflict analysis
- Historical state-law versions
- State legal-source tracking

For patent-specific analysis, the system must recognize the distinction between federal patent law and state laws that may affect related matters without incorrectly treating state law as a replacement for federal patent law.

## International Jurisdiction Module

The International Jurisdiction Module provides the framework for expanding Axis Juris beyond the United States.

### Features

- Country-specific jurisdiction packs
- Province-specific jurisdiction packs
- Territory-specific jurisdiction packs
- Regional legal frameworks
- International patent law
- Comparative patent law
- Cross-border analysis
- International filing considerations
- International treaty integration
- Regional patent-office integration
- Country-specific source hierarchies
- Country-specific legal terminology
- Country-specific update feeds
- International effective-date tracking
- Multi-country legal comparison

The architecture must allow additional jurisdictions to be added as independent modules without modifying the fundamental reasoning engine.

## Prior Art & Patent Landscape Module

The Prior Art Module analyzes patent documents and related technical material.

### Features

- Prior-art discovery
- Patent-document similarity analysis
- Claim similarity analysis
- Technical concept matching
- Patent-family identification
- Citation-network analysis
- Forward-citation analysis
- Backward-citation analysis
- Patent landscape analysis
- Competitive patent analysis
- Technology-domain clustering
- Similar-patent identification
- Prior-art timelines
- Filing-date comparison
- Priority-date analysis
- Patent-family timeline analysis
- Similarity-based risk assessment
- User-defined prior-art monitoring

The system must distinguish between similarity findings and legal conclusions regarding novelty or validity.

## Legal Risk Analysis Module

The Legal Risk Module evaluates potential legal issues identified by the system.

### Features

- Patent eligibility risk
- Novelty risk
- Obviousness risk
- Claim construction risk
- Infringement risk
- Enablement risk
- Written-description risk
- Definiteness risk
- Ownership risk
- Inventorship risk
- Procedural risk
- Jurisdictional risk
- Publication risk
- Regulatory risk
- Precedent-change risk
- Prior-art risk
- Source uncertainty
- Legal-change risk
- Risk severity classification
- Risk explanation
- Supporting authorities
- Cross-referenced evidence
- Human-review recommendations

Risk scores must be presented as analytical indicators rather than definitive predictions of legal outcomes.

## Publication Conflict Detection Module

The Publication Conflict Detection Module monitors user-submitted publications, applications, documents, and other content for potential conflicts with legal developments.

### Features

- User document analysis
- Patent application monitoring
- Publication monitoring
- Technical-content analysis
- Legal-risk scanning
- Statutory conflict detection
- Regulatory conflict detection
- Case-law conflict detection
- Patent claim conflict detection
- Jurisdiction-specific conflict detection
- New-law impact analysis
- Existing-law conflict analysis
- New-precedent impact analysis
- Potentially affected passage identification
- Legal-risk classification
- Supporting-source identification
- Cross-reference generation
- Change-impact explanations
- Human-review recommendations

The system must identify potential conflicts rather than represent an automated determination as legally conclusive.

## Alert & Notification Module

The Alert & Notification Module provides proactive notifications when relevant legal developments are detected.

### Features

- Real-time alerts
- Scheduled alerts
- User-configurable alerts
- New statute alerts
- Amendment alerts
- Repeal alerts
- New case alerts
- Precedent-change alerts
- Regulatory alerts
- USPTO alerts
- Jurisdiction-specific alerts
- Publication conflict alerts
- Prior-art alerts
- Legal-risk alerts
- Effective-date reminders
- Deadline reminders
- Watchlist notifications
- Portfolio notifications
- Alert severity levels
- Alert acknowledgment
- Alert dismissal
- Alert escalation
- Alert history
- Duplicate-alert suppression
- Email notifications
- Web notifications
- Webhook notifications
- API-based notifications

## Publication & Portfolio Monitoring Module

The Publication & Portfolio Monitoring Module provides continuous monitoring of user-defined patent and publication assets.

### Features

- Patent portfolio tracking
- Application tracking
- Publication tracking
- Claim-version tracking
- Legal-status tracking
- Jurisdiction tracking
- Document version history
- Continuous risk monitoring
- Portfolio-wide legal scanning
- Technology-area monitoring
- Competitor monitoring
- Legal-change impact reports
- Portfolio risk dashboards
- User-defined monitoring rules
- Asset-specific alerts

## Legal Research Workspace Module

The Legal Research Workspace provides an environment for organizing legal research and analysis.

### Features

- Research projects
- Saved research
- Case collections
- Statute collections
- Patent collections
- Source collections
- Research notes
- Source bookmarks
- Legal issue tagging
- Jurisdiction tagging
- Custom watchlists
- Research timelines
- Cross-reference views
- Saved AI analyses
- Versioned research results
- Research history
- Exportable research reports

## Document Intelligence Module

The Document Intelligence Module processes legal and patent-related documents.

### Features

- PDF analysis
- Patent document parsing
- Court opinion parsing
- Statute parsing
- Regulation parsing
- Legislative document parsing
- Structured text extraction
- Citation extraction
- Legal entity extraction
- Legal terminology extraction
- Document comparison
- Version comparison
- Change highlighting
- Section-level analysis
- Claim-level analysis
- Source identification
- Metadata extraction

## Legal Timeline Module

The Legal Timeline Module provides temporal views of legal authorities and developments.

### Features

- Statute history timelines
- Case development timelines
- Patent prosecution timelines
- Patent family timelines
- Legal doctrine timelines
- Amendment timelines
- Effective-date timelines
- Precedent evolution timelines
- Jurisdictional change timelines
- Legal change timelines
- Before-and-after legal comparisons
- Historical authority reconstruction

## Cross-Reference Module

The Cross-Reference Module connects related legal authorities and user materials.

### Features

- Automatic statute cross-references
- Case-to-case references
- Statute-to-case references
- Patent-to-case references
- Claim-to-specification references
- Claim-to-prior-art references
- Regulation-to-statute references
- Jurisdiction-to-authority references
- Related-doctrine discovery
- Citation-chain traversal
- Authority dependency mapping
- Cross-jurisdiction references
- Historical cross-references

## Legal Transparency Module

The Legal Transparency Module makes the basis for AI-generated analysis visible to the user.

### Features

- Source-first responses
- Citation-required responses
- Authority classification
- Source confidence
- Reasoning transparency
- Evidence trails
- Legal uncertainty indicators
- Conflicting-authority indicators
- Outdated-source indicators
- Temporal context
- Jurisdictional context
- AI inference labeling
- Human-review recommendations
- Reproducible research context
- Audit records

## Data Governance Module

The Data Governance Module manages the integrity and provenance of legal information.

### Features

- Source provenance
- Data versioning
- Legal-version preservation
- Update audit logs
- Data integrity validation
- Source-change tracking
- Structured metadata
- Jurisdiction metadata
- Effective-date metadata
- Authority metadata
- Confidence metadata
- Data-quality monitoring
- Update rollback
- Reproducible ingestion
- Historical data preservation

## Security & Privacy Module

The Security & Privacy Module protects user information and legal research materials.

### Features

- Local-first deployment
- Self-hosted deployment
- User-controlled data
- Encryption support
- Authentication integration
- Role-based access control
- Workspace permissions
- Audit logging
- Secure API access
- Secrets management
- Data-retention controls
- Document access controls
- Configurable external-service access
- Optional isolated AI inference
- Configurable data-processing policies

## API Module

The API Module provides programmatic access to Axis Juris capabilities.

### Features

- REST API
- Authentication support
- Legal research endpoints
- Case endpoints
- Statute endpoints
- Patent endpoints
- Jurisdiction endpoints
- Alert endpoints
- Document-analysis endpoints
- Knowledge-graph endpoints
- Search endpoints
- Legal-update endpoints
- Monitoring endpoints
- Webhook support
- External application integration
- Automation support

## Administration Module

The Administration Module provides system-level configuration and management.

### Features

- Module configuration
- Jurisdiction management
- Source management
- Connector management
- AI-provider management
- Notification-provider management
- User management
- Permission management
- Monitoring configuration
- Logging configuration
- Diagnostic tools
- Health checks
- Ingestion monitoring
- Update monitoring
- Error reporting
- Audit-log management
- Data-quality monitoring

---

# Optional Plugin Modules

Optional plugin modules must extend Axis Juris without requiring modifications to the core reasoning architecture.

## Copyright Law Plugin

- Copyright statute analysis
- Copyright case law
- Copyright registration analysis
- Copyright ownership analysis
- Copyright infringement analysis
- Fair-use analysis
- Publication monitoring
- Copyright-law updates
- Jurisdiction-specific copyright analysis

## Trademark Law Plugin

- Trademark statute analysis
- Trademark case law
- Trademark registration analysis
- Trademark classification
- Trademark similarity analysis
- Trademark infringement analysis
- Trademark enforcement monitoring
- Trademark-law updates

## Trade Secret Law Plugin

- Trade-secret statute analysis
- Trade-secret case law
- Confidentiality analysis
- Misappropriation analysis
- Trade-secret protection analysis
- Jurisdiction-specific trade-secret rules
- Legal-change monitoring

## Licensing Law Plugin

- Intellectual-property licensing analysis
- License-term analysis
- License conflict detection
- Ownership and authorization analysis
- License compliance monitoring
- Jurisdiction-specific licensing rules

## Contract Law Plugin

- Contract analysis
- Clause identification
- Contract-risk detection
- Contract comparison
- Governing-law analysis
- Jurisdiction-specific contract rules
- Contract-law updates

## Regulatory Compliance Plugin

- Regulatory requirement mapping
- Compliance monitoring
- Regulatory change detection
- Effective-date tracking
- Jurisdiction-specific requirements
- Compliance alerts
- Regulatory conflict detection

## International IP Plugin

- International patent law
- International copyright law
- International trademark law
- Treaty analysis
- Regional IP systems
- Cross-border IP analysis
- International filing considerations
- International legal updates

## Legal Research Export Plugin

- Research report generation
- Citation reports
- Legal authority reports
- Patent landscape reports
- Risk reports
- Timeline reports
- Knowledge graph exports
- Structured data exports

## Notification Provider Plugins

- Email notification provider
- SMS notification provider
- Webhook provider
- Collaboration-platform provider
- Calendar provider
- Custom notification provider

## AI Provider Plugins

- Cloud LLM providers
- Local LLM providers
- Self-hosted inference
- Specialized legal language models
- Embedding providers
- Reranking providers
- Custom reasoning providers

## Data Source Plugins

- Legislative databases
- Court databases
- Patent databases
- Regulatory databases
- Government repositories
- International legal repositories
- User-managed legal sources
- Organization-specific legal databases

## Future Legal Domain Plugins

The plugin architecture may support additional legal domains without modifying the core system, including:

- Employment law
- Privacy law
- Data protection law
- Technology law
- Securities law
- Environmental law
- Tax law
- Real estate law
- Healthcare regulation
- Consumer protection law
- International commercial law

# Legal Update Requirements

Axis Juris must maintain a distinction between legal information and legal interpretation.

Every legal update should contain, where available:

- Source
- Authority
- Jurisdiction
- Publication date
- Effective date
- Status
- Relevant legal domain
- Affected provisions
- Previous version
- Current version
- Change description
- Related cases
- Related regulations
- Related statutes
- Source provenance

The update engine must preserve historical versions so that the system can determine what law applied at a particular point in time.

# Jurisdiction Applicability Requirements

The system must not automatically assume that every law associated with a user's geographic location applies to every legal issue.

Applicability analysis should consider:

- User-selected jurisdiction
- Relevant geographic location
- Subject matter
- Legal issue
- Governing law
- Court
- Venue
- Parties
- Transaction
- Publication
- Filing location
- Patent jurisdiction
- Effective date
- Legal authority hierarchy

The system must identify when additional facts are necessary to determine applicability.

# Source Requirements

Legal responses should prioritize authoritative sources, including:

- Statutory sources
- Official legislative sources
- Official court opinions
- Official USPTO sources
- Official government publications
- Official regulatory sources
- Official international legal sources

Secondary sources may supplement analysis but should not silently replace primary authority.

# Conflict Detection Requirements

When a monitored document may be affected by a legal development, Axis Juris should provide:

- The affected document
- The affected section or claim
- The relevant legal authority
- The nature of the potential conflict
- Jurisdiction
- Effective date
- Supporting sources
- Related precedent
- Confidence level
- Risk classification
- Explanation of the potential impact
- Recommendation for human review

The system must clearly distinguish a detected potential conflict from a confirmed legal violation.

# Human Review Requirements

Axis Juris must provide mechanisms for human review when:

- Authorities conflict
- Sources are incomplete
- Legal status is uncertain
- A law has recently changed
- A case has uncertain precedential status
- Jurisdiction is unclear
- The system lacks sufficient facts
- A legal conclusion would require professional judgment
- A filing or legal proceeding may be materially affected

# AI Legal Boundary

Axis Juris is a legal intelligence and research system. It is not a law firm and does not establish an attorney-client relationship.

AI-generated output must be identified as analysis, research assistance, risk assessment, or related informational output rather than guaranteed legal advice or a definitive legal determination.

Users should be directed toward qualified legal professionals when professional legal advice, representation, filing decisions, litigation strategy, or other legally consequential judgment is required.

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
  - [https://roxanneardary.com/axisjuris/](https://roxanneardary.com/axisjuris/)

---

## License & Notice Requirements

Axis Juris is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Axis Juris specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any updates that add contributors or modify attribution must also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the project's `notice.md` file.

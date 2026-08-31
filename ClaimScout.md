# ClaimScout
**The Scout for Your Intellectual Property**
- HTML Mirror: [https://roxanneardary.com/claimscout-specification/](https://roxanneardary.com/claimscout-specification/)

---

## Specification

ClaimScout is an open-source, modular AI system for monitoring, identifying, documenting, and analyzing potential unauthorized use of copyrighted works across public code repositories, websites, social platforms, and other publicly accessible sources.

The system is designed to help copyright owners establish provenance, identify potential infringement, understand applicable licenses and notices, preserve evidence, identify distribution hubs, and prepare evidence-based reports for human review and potential DMCA action.

ClaimScout must prioritize accuracy, traceability, transparency, responsible evidence handling, license awareness, and human approval before any legal notice or enforcement action is initiated.

## Core Principles

ClaimScout must be designed around the following principles:

- Open source architecture
- Modular design
- Local-first operation where practical
- Human-in-the-loop review
- Evidence preservation
- Source and provenance tracking
- License-aware analysis
- Transparent confidence scoring
- Reproducible findings
- Respect for applicable laws and platform terms
- No unauthorized access to private systems or restricted content
- No automatic submission of legal notices without explicit human authorization
- Clear separation between factual findings and legal conclusions

---

## Core System

The core system provides the foundational capabilities required for monitoring, analysis, evidence collection, provenance tracking, reporting, and case management.

### Configuration Core

The Configuration Core manages system-wide settings and user-defined monitoring profiles.

It must support:

- Copyrighted work registration
- Keyword and phrase configuration
- File and directory monitoring
- Content fingerprint registration
- Media fingerprint registration
- Repository and platform selection
- Search frequency configuration
- Monitoring priority configuration
- Confidence thresholds
- Evidence retention settings
- Notification preferences
- Report configuration
- User roles and permissions
- Local and remote storage configuration

### Copyright Work Registry

The Copyright Work Registry maintains authoritative records for works that the user wants ClaimScout to monitor.

Each work may include:

- Work title
- Work description
- Author or rights holder
- Creation date
- Publication date
- First known publication location
- Original repository or website
- Source URL
- File names
- Content hashes
- Text fingerprints
- Media fingerprints
- Keywords
- Distinctive phrases
- Associated domains
- Associated accounts
- License information
- Notice information
- Registration information where applicable
- Supporting provenance records

The registry must support multiple versions of the same work and maintain historical relationships between versions.

### Repository Discovery Core

The Repository Discovery Core searches publicly accessible repositories and code hosting services for potential matches.

It must support:

- Keyword searches
- Exact phrase searches
- Filename searches
- Repository name searches
- Owner searches
- Content searches
- License searches
- URL searches
- Metadata searches
- Search result deduplication
- Repository indexing
- Repository ownership identification
- Repository activity tracking
- Repository update tracking
- Public commit history analysis

The system should identify potential distribution hubs where the same work appears across multiple repositories, forks, mirrors, organizations, or accounts.

### Web and Social Discovery Core

The Web and Social Discovery Core monitors publicly accessible websites and supported social platforms for potential reuse.

It must support:

- Keyword searches
- Exact phrase searches
- URL searches
- Content similarity searches
- Public post discovery
- Public profile identification
- Publication date and time collection
- Source URL collection
- Author or account identification
- Cross-platform matching
- Link relationship analysis
- Public content change tracking

Platform integrations must operate through authorized APIs or otherwise permitted public access methods.

### Content Matching Core

The Content Matching Core determines whether discovered material may correspond to a monitored work.

It must support:

- Exact matching
- Partial matching
- Fuzzy matching
- Semantic similarity
- Phrase similarity
- Structural similarity
- Code similarity
- Variable and identifier normalization
- Formatting normalization
- Whitespace normalization
- Paraphrase detection
- Reordered-content detection
- Modified-content detection
- Duplicate detection
- Near-duplicate detection

Every match must include an explainable basis for the similarity determination.

### Media Fingerprinting Core

The Media Fingerprinting Core analyzes visual, audio, and video material.

It must support:

- Cryptographic hashes
- Perceptual hashes
- Image similarity
- Cropping detection
- Resizing detection
- Compression detection
- Minor modification detection
- Audio fingerprinting
- Video fingerprinting
- Frame similarity
- Thumbnail matching
- Metadata comparison

The system must distinguish between an exact match, probable derivative match, visually similar material, and an inconclusive result.

### Code Analysis Core

The Code Analysis Core specializes in software repositories.

It must support:

- Source code comparison
- Normalized code comparison
- Abstract syntax analysis where available
- Identifier normalization
- Comment comparison
- Documentation comparison
- Function similarity
- File similarity
- Directory similarity
- Commit history analysis
- Earliest known appearance detection
- Fork relationship analysis
- Mirror detection
- Version comparison
- Dependency identification

The system should identify potentially copied portions without automatically determining legal infringement.

### Provenance and Ownership Core

The Provenance and Ownership Core builds a chronological record surrounding a copyrighted work.

It must collect and correlate:

- Creation records
- Publication records
- Repository creation dates
- Commit timestamps
- Release dates
- Website publication dates
- Social media publication dates
- Archived versions
- Original URLs
- Author identities or account names
- Public ownership statements
- License declarations
- Notice files
- Copyright statements
- Attribution records
- Registration information supplied by the user

The system must preserve source references for every provenance claim.

### Evidence Collection Core

The Evidence Collection Core preserves information necessary for later human review.

It must support:

- Timestamped evidence records
- Source URLs
- Repository metadata
- File paths
- Content hashes
- Relevant content excerpts
- Screenshots where permitted
- Public page snapshots where permitted
- Commit references
- Social media post references
- Publication timestamps
- Platform metadata
- License files
- NOTICE files
- Evidence acquisition timestamps
- Evidence integrity hashes

Evidence must be stored with provenance metadata so that users can determine when, where, and how each record was collected.

### Evidence Integrity Core

The Evidence Integrity Core protects collected evidence from unnoticed alteration.

It must support:

- Cryptographic hashing
- Evidence manifests
- Acquisition timestamps
- Immutable or append-only records where available
- Chain-of-custody records
- Evidence versioning
- Source verification
- Integrity validation
- Duplicate evidence detection

ClaimScout must never alter original evidence while generating analytical interpretations.

### License and Notice Core

The License and Notice Core analyzes the legal and attribution information associated with discovered material.

It must detect:

- LICENSE files
- COPYING files
- NOTICE files
- NOTICE.md files
- Copyright headers
- Attribution statements
- Repository license metadata
- Platform license declarations
- Embedded licensing terms

It must identify relevant conditions such as:

- Attribution requirements
- Redistribution requirements
- Modification requirements
- Copyleft requirements
- Source availability requirements
- Notice preservation requirements
- Additional permissions
- Restrictions
- Disclaimers

The system must distinguish between license compliance issues and potential copyright infringement.

### License Compliance Recommendation Core

The License Compliance Recommendation Core evaluates whether a discovered use may have an available licensing pathway.

Possible findings should include:

- License appears compatible
- Attribution appears incomplete
- Required notice appears missing
- License conditions require review
- License information is ambiguous
- License could not be identified
- Potential infringement requires human review

The system must not treat the absence of a license as automatic proof of infringement.

### Cross-Platform Correlation Core

The Cross-Platform Correlation Core connects related findings across repositories, websites, and social platforms.

It must identify:

- Shared content
- Shared URLs
- Shared authors
- Shared organizations
- Shared repository owners
- Common publication patterns
- Common filenames
- Common fingerprints
- Common phrases
- Repository forks
- Mirrors
- Distribution networks
- Repeated appearances

The system should create a relationship graph showing how potentially related instances are connected.

### Distribution Hub Analysis Core

The Distribution Hub Analysis Core identifies locations where potentially unauthorized copies are concentrated.

A hub may be identified based on:

- Number of matching works
- Number of repositories
- Number of mirrors
- Number of forks
- Number of associated accounts
- Cross-platform presence
- Frequency of reuse
- Historical activity
- Content similarity
- Relationship between discovered locations

Reports must identify the repository or platform, repository name, owner or account, relevant URLs, matched work, evidence, timestamps, and confidence level.

### Case Building Core

The Case Building Core organizes findings into individual cases.

Each case should contain:

- Case identifier
- Copyrighted work
- Rights holder
- Potentially matching material
- Repository or platform
- Owner or account
- URLs
- Dates and times
- Evidence
- Provenance records
- License information
- NOTICE information
- Similarity analysis
- Distribution relationships
- Confidence score
- Missing evidence
- Human review status
- Recommended next step

Cases must remain editable by authorized users.

### Case Strength Assessment Core

The Case Strength Assessment Core evaluates evidence completeness and consistency.

It may consider:

- Strength of the content match
- Quality of provenance evidence
- Reliability of timestamps
- Availability of original work records
- Availability of source history
- License information
- Attribution information
- Evidence integrity
- Number of independent corroborating sources
- Relationship between original and discovered material

The system must clearly label its assessment as an analytical recommendation rather than a legal determination.

### DMCA Recommendation Core

The DMCA Recommendation Core prepares potential takedown documentation for human review.

It must:

- Identify the relevant work
- Identify potentially infringing material
- Provide source URLs
- Provide evidence references
- Identify the hosting platform
- Identify repository or account ownership information
- Summarize provenance
- Summarize relevant licensing information
- Identify missing information
- Generate a draft notice
- Provide platform-specific submission guidance
- Record review status

ClaimScout must not automatically submit a DMCA notice without explicit authorization from the rights holder or authorized representative.

### Report Generation Core

The Report Generation Core produces structured reports for investigation, record keeping, legal review, and potential takedown preparation.

Reports should support:

- HTML
- Markdown
- PDF
- CSV
- JSON

Reports may include:

- Executive summary
- Monitored work information
- Findings
- Repository information
- Owner information
- Platform information
- URLs
- Match analysis
- Evidence
- Timeline
- License analysis
- NOTICE analysis
- Distribution hub analysis
- Related findings
- Confidence scores
- Case strength assessment
- Recommended actions
- Human review notes

### Timeline Core

The Timeline Core constructs chronological histories for monitored works and discovered uses.

It must correlate:

- Creation dates
- Publication dates
- Commit dates
- Release dates
- Social media dates
- Website publication dates
- Repository changes
- Evidence acquisition dates

Timeline entries must preserve their original source and confidence.

### Alerting Core

The Alerting Core notifies users about significant monitoring events.

Alerts may include:

- New potential match
- High-confidence match
- New repository appearance
- New social media appearance
- New distribution hub
- Repository change
- License change
- NOTICE change
- New related account
- Repeat appearance
- Evidence integrity issue
- Case status change

### Dashboard Core

The Dashboard Core provides a user interface for monitoring and reviewing ClaimScout activity.

It should provide:

- Active monitoring profiles
- Recent findings
- High-confidence matches
- Open cases
- Evidence status
- Repository activity
- Distribution hubs
- License findings
- Timeline views
- Cross-platform relationships
- Alerts
- Reports
- Review queues

### Search and Query Core

The Search and Query Core provides unified access to collected information.

It must support:

- Full-text search
- Keyword search
- Boolean search
- Repository filtering
- Owner filtering
- Platform filtering
- Date filtering
- License filtering
- Confidence filtering
- Case filtering
- Evidence filtering
- Work filtering

### Audit and Accountability Core

The Audit and Accountability Core records important ClaimScout operations.

It should record:

- User actions
- Configuration changes
- Evidence collection events
- Analysis events
- Report generation
- Case changes
- Review decisions
- Export events
- Notice generation
- Authorization events

Audit records must support investigation and reproducibility.

### Privacy and Security Core

The Privacy and Security Core protects collected information.

It must support:

- Access controls
- Authentication
- Authorization
- Encryption where appropriate
- Secure credential storage
- Data retention controls
- Evidence access controls
- Audit logging
- Sensitive data minimization
- Secure deletion
- Local-first storage options

ClaimScout must not collect private credentials, bypass authentication, or access private repositories without authorization.

### Human Review Core

The Human Review Core ensures that consequential decisions remain subject to human oversight.

Users must be able to:

- Confirm findings
- Reject findings
- Mark findings as inconclusive
- Add evidence
- Correct metadata
- Add provenance
- Review licenses
- Review NOTICE files
- Edit reports
- Approve DMCA drafts
- Record decisions
- Add case notes

AI-generated conclusions must remain distinguishable from verified factual records.

---

## Optional Plugin Modules

ClaimScout must support an extensible plugin system so additional capabilities can be added without modifying the core architecture.

### Repository Plugins

Optional repository plugins may provide integrations for:

- GitHub
- GitLab
- Codeberg
- Bitbucket
- Other compatible public code hosting services

Each plugin should provide repository discovery, metadata retrieval, content search, commit history, and licensing information where supported.

### Social Platform Plugins

Optional plugins may support publicly accessible content from:

- Reddit
- LinkedIn
- X
- Instagram
- Other compatible platforms

Plugins must use authorized interfaces and comply with applicable platform requirements.

### Web Archive Plugins

Optional archive plugins may integrate with permitted archival services to retrieve historical versions of publicly accessible pages.

### Media Analysis Plugins

Optional plugins may provide advanced:

- Image analysis
- Audio fingerprinting
- Video fingerprinting
- OCR
- Visual similarity
- Speech-to-text
- Media metadata analysis

### Advanced AI Plugins

Optional AI plugins may provide:

- Additional embedding models
- Local language models
- Specialized code models
- Multilingual analysis
- Advanced semantic matching
- Document classification
- Entity resolution
- Relationship extraction

Users should be able to select local models where practical to reduce vendor dependency.

### Legal Reference Plugins

Optional legal reference plugins may provide:

- Platform takedown procedures
- DMCA form guidance
- Copyright office references
- Jurisdiction-specific reference material
- Legal terminology
- Notice templates

Legal reference plugins must present information as reference material and must not represent AI output as legal advice.

### Legal Service Plugins

Optional integrations may connect ClaimScout with authorized legal service providers or internal legal workflows.

All legal service integrations must require explicit user authorization before transmitting case information or initiating external actions.

### Notification Plugins

Optional notification plugins may support:

- Email
- Webhooks
- Messaging services
- Desktop notifications
- Mobile notifications
- Team collaboration platforms

### Collaboration Plugins

Optional collaboration plugins may provide:

- Team case review
- Assignment workflows
- Comments
- Evidence annotations
- Approval workflows
- Shared investigations
- Role-based review

### Storage Plugins

Optional storage plugins may support:

- Local databases
- PostgreSQL
- SQLite
- Object storage
- Encrypted evidence stores
- Compatible archival systems

### Export Plugins

Optional plugins may support additional output formats and integrations for:

- Legal case management
- Document management
- Spreadsheet systems
- Evidence management systems
- Reporting platforms

---

## Matching and Confidence Framework

ClaimScout must use transparent confidence classifications.

Recommended classifications include:

- **Exact Match**
- **Strong Match**
- **Probable Match**
- **Possible Match**
- **Weak Match**
- **Inconclusive**
- **False Positive**
- **License-Compliant Use**
- **Requires Human Review**

Confidence scores must be accompanied by an explanation of the evidence supporting the classification.

## Evidence Standards

Every significant finding should maintain a clear distinction between:

- Source material
- Collected metadata
- Derived analysis
- AI interpretation
- Human verification
- Legal recommendation

ClaimScout must never present an AI inference as an established fact without identifying the underlying evidence.

## Responsible Monitoring

ClaimScout is intended for lawful monitoring of publicly accessible information and authorized data sources.

The system must not be designed to:

- Bypass authentication
- Access private repositories without permission
- Circumvent security controls
- Obtain private credentials
- Evade platform restrictions
- Conduct unauthorized intrusion
- Harass individuals
- Automatically submit unsupported legal claims

Users remain responsible for ensuring that their monitoring activities comply with applicable laws, regulations, contracts, licenses, and platform terms.

## Data Retention

Users must be able to configure retention policies for:

- Search results
- Evidence
- Screenshots
- Snapshots
- Metadata
- Audit records
- Case records
- Reports

Retention controls should support automatic expiration, manual deletion, archival, and preservation of selected evidence.

## Reproducibility

ClaimScout should make investigations reproducible by recording:

- Search parameters
- Monitoring configuration
- Collection timestamps
- Source URLs
- Source metadata
- Matching methods
- Model information
- Confidence calculations
- Evidence hashes
- Human decisions
- Report generation timestamps

## Extensibility

All major ClaimScout capabilities should use modular interfaces so that new repositories, platforms, models, storage systems, analysis engines, notification systems, and reporting formats can be added without requiring changes to unrelated core components.

Plugins should be independently configurable, enableable, disableable, and replaceable.

## Operational Workflow

ClaimScout should operate through the following general process:

1. Register copyrighted works.
2. Configure keywords, fingerprints, repositories, platforms, and monitoring rules.
3. Discover publicly accessible content.
4. Collect permitted metadata and evidence.
5. Normalize and fingerprint discovered material.
6. Compare discovered content against registered works.
7. Analyze repository history and publication history.
8. Detect related appearances across platforms.
9. Identify repositories, owners, accounts, and distribution hubs.
10. Detect and analyze licenses and NOTICE files.
11. Evaluate potential license compliance.
12. Build provenance timelines.
13. Preserve supporting evidence.
14. Create or update a case.
15. Calculate confidence and evidence strength.
16. Present findings for human review.
17. Generate a report.
18. Generate a draft DMCA notice when appropriate.
19. Require explicit human approval before external legal action.
20. Record the final decision and maintain the investigation history.

## Reporting Requirements

A standard infringement investigation report should include:

- Case title
- Case identifier
- Rights holder
- Monitored work
- Original source
- Original publication information
- Potentially matching source
- Repository name
- Repository owner
- Platform
- Relevant file path
- Relevant URL
- Publication date and time
- Commit information
- Match type
- Similarity explanation
- Evidence references
- License information
- NOTICE information
- Compliance analysis
- Related sources
- Distribution hubs
- Timeline
- Confidence assessment
- Missing information
- Human review status
- Recommended next step  

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
  - [https://roxanneardary.com/claimscout/](https://roxanneardary.com/claimscout/)

---

## License & Notice Requirements

ClaimScout is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- ClaimScout specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

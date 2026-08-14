# TrustLens

### Prepared Listings, Happy Buyers
- HTML Mirror: [https://roxanneardary.com/trustlens-specification/](https://roxanneardary.com/trustlens-specification/)

TrustLens is part of the **OpenProperty** ecosystem. [https://roxanneardary.com/openproperty/](https://roxanneardary.com/openproperty/)

## Specification

TrustLens is an open-source property transparency platform designed to help sellers and property owners prepare complete, accurate, and disclosure-ready property listings before bringing a property to market.

TrustLens combines AI-assisted analysis, location-aware legal guidance, document processing, compliance verification, inspection preparation, and buyer question anticipation into a modular property preparation system.

## Purpose

TrustLens is designed to reduce transaction delays, disputes, renegotiations, and failed negotiations caused by missing, incomplete, inaccurate, or late-discovered property information.

The system shall help property owners:

- Prepare complete property disclosure packages
- Identify documentation buyers are likely to request
- Verify permits and renovation records
- Understand jurisdiction-specific disclosure and compliance requirements
- Identify documentation gaps
- Prepare proactive inspection records
- Anticipate buyer due diligence questions
- Request records from appropriate government authorities
- Organize property documentation
- Generate a shareable property transparency report
- Present properties with greater transparency and preparedness

## Design Principles

TrustLens shall follow these principles:

- Transparency by default
- Seller preparation before listing
- Location-aware guidance
- Evidence-based property documentation
- Modular architecture
- Human review of AI-generated recommendations
- Privacy-preserving document handling
- Local-first AI support where practical
- Optional external service integrations
- Open-source interoperability
- Vendor-neutral architecture
- Official-source prioritization for government and compliance records

## Core Modules

### Property Profile Module

The Property Profile Module shall maintain the foundational information required to evaluate a property.

Capabilities shall include:

- Property address
- Property location
- Property type
- Construction information
- Ownership information
- Improvement history
- Renovation history
- Relevant jurisdiction information
- HOA or community information
- Property preparation status

The module shall provide normalized property information to other TrustLens modules.

### Disclosure Preparation Module

The Disclosure Preparation Module shall guide sellers through the creation of property disclosure packages.

Capabilities shall include:

- Identification of applicable disclosure categories
- Disclosure preparation workflows
- Common defect identification
- Known-condition documentation
- Maintenance history collection
- Renovation documentation collection
- Environmental disclosure preparation
- Disclosure completeness evaluation
- Identification of potentially missing disclosures
- Disclosure preparation status tracking

The module shall distinguish between information that has been provided, information that remains incomplete, and information requiring further verification.

### Jurisdiction and Legal Guidance Module

The Jurisdiction and Legal Guidance Module shall provide location-aware guidance based on the property's applicable jurisdiction.

Capabilities shall include:

- State disclosure requirement evaluation
- County requirement evaluation
- Township requirement evaluation
- Municipal requirement evaluation
- Zoning requirement evaluation
- HOA requirement identification
- Jurisdiction determination
- Compliance checklist generation
- Location-specific preparation recommendations

The module shall identify applicable requirements without presenting AI-generated guidance as a substitute for professional legal advice.

### Permit and Renovation Verification Module

The Permit and Renovation Verification Module shall evaluate property improvements and identify documentation that may be required to establish compliance.

Capabilities shall include:

- Addition verification
- Sunroom verification
- Finished basement verification
- Electrical upgrade verification
- Plumbing modification verification
- Deck verification
- Structural modification verification
- Permit history evaluation
- Required permit identification
- Inspection record identification
- Renovation documentation evaluation
- Contractor documentation tracking
- Potential compliance gaps

The module shall allow verified records and seller-provided documentation to be evaluated together.

### Inspection Preparation Module

The Inspection Preparation Module shall help sellers identify inspections that may improve property readiness before listing.

Capabilities shall include recommendations for:

- Structural inspections
- Electrical inspections
- Plumbing inspections
- HVAC inspections
- Roof inspections
- Pest inspections
- Other property-specific inspections

The module shall identify recommended inspection documentation and track whether relevant reports have been obtained.

### Buyer Question Anticipation Module

The Buyer Question Anticipation Module shall use property information and available documentation to identify questions buyers may raise during due diligence.

Capabilities shall include:

- Permit history questions
- Repair history questions
- Renovation questions
- Contractor documentation questions
- Utility questions
- HOA questions
- Township compliance questions
- Property condition questions
- Maintenance history questions
- Documentation gap identification

The module shall generate preparation recommendations so sellers can address likely questions before they become transaction issues.

### Government Records and Compliance Request Module

The Government Records and Compliance Request Module shall guide sellers in obtaining records from appropriate official authorities.

Capabilities shall include guidance for requesting:

- Certificate of occupancy records
- Permit history reports
- Zoning confirmations
- Property tax records
- Environmental notices
- Municipal compliance records
- Other jurisdiction-specific property records

The module shall prioritize official government sources when available.

### Document Management Module

The Document Management Module shall provide secure handling and organization of property documentation.

Supported document categories shall include:

- Disclosure forms
- Permits
- Contractor invoices
- Inspection reports
- HOA documents
- Zoning confirmations
- Government records
- Maintenance records
- Renovation records
- Other property-related documentation

Capabilities shall include:

- Document upload
- Document storage
- Document categorization
- Document classification
- Document metadata
- Document status tracking
- Document completeness analysis
- Missing-document identification
- Potential concern identification

### Document Analysis Module

The Document Analysis Module shall analyze uploaded property records using OCR, structured extraction, and AI-assisted analysis.

Capabilities shall include:

- OCR document scanning
- Text extraction
- Structured data extraction
- Automated document classification
- Document type identification
- Key information extraction
- Cross-document comparison
- Missing information detection
- Potential inconsistency identification
- Potential buyer concern identification

The module shall preserve human review as part of the verification process.

### Compliance Verification Module

The Compliance Verification Module shall evaluate available property information against applicable requirements.

Capabilities shall include:

- Permit compliance evaluation
- Disclosure completeness evaluation
- Inspection documentation evaluation
- Zoning information evaluation
- Municipal compliance evaluation
- HOA requirement evaluation
- Documentation gap detection
- Compliance status tracking
- Verification evidence tracking

The module shall distinguish between verified information, seller-provided information, inferred information, and information requiring additional confirmation.

### Property Readiness Scoring Module

The Property Readiness Scoring Module shall evaluate the overall preparation state of a property.

The scoring system may consider:

- Disclosure completeness
- Permit verification
- Inspection documentation
- Renovation records
- Compliance confirmations
- Document completeness
- Identified buyer concerns
- Outstanding preparation tasks

The module shall provide explainable readiness results rather than relying solely on an opaque numerical score.

### Transparency Passport Module

The Transparency Passport Module shall generate a shareable report summarizing property preparation and transparency status.

The Transparency Passport may include:

- Property identification
- Disclosure completeness
- Permit verification
- Inspection documentation
- Renovation records
- Compliance confirmations
- Outstanding documentation
- Preparation status
- Property readiness assessment

The module shall support controlled sharing so property owners can determine what information is made available to prospective buyers and other authorized parties.

### AI Assistance Module

The AI Assistance Module shall provide AI capabilities across TrustLens core workflows.

Supported AI functions shall include:

- Disclosure guidance
- Compliance evaluation
- Document analysis
- Document classification
- Buyer question prediction
- Property readiness scoring
- Missing information identification
- Preparation recommendations

The AI layer shall support:

- Local large language models
- Optional external AI APIs
- Configurable AI providers
- Human review of generated recommendations

AI-generated information shall be distinguishable from verified records and authoritative source information.

### Security and Privacy Module

The Security and Privacy Module shall protect property documentation and user information.

Capabilities shall include:

- Secure authentication
- Encrypted document storage
- Encrypted communication
- Controlled document sharing
- Access controls
- Document permission management
- Secure handling of sensitive property records
- Protection of user data

### Data and Persistence Module

The Data and Persistence Module shall provide structured storage for TrustLens data.

The reference implementation shall support PostgreSQL.

The module shall manage:

- Property records
- User records
- Jurisdiction information
- Disclosure requirements
- Documents
- Document metadata
- Permits
- Inspections
- Renovations
- Compliance findings
- Buyer questions
- Preparation tasks
- Transparency Passport records
- Readiness assessments

## Optional Plugin Modules

TrustLens shall support optional plugins that extend the core platform without requiring every installation to include every integration.

### State Disclosure Law Plugins

Optional plugins may provide jurisdiction-specific disclosure requirements for individual states.

Capabilities may include:

- State disclosure rules
- State-specific disclosure forms
- Disclosure requirement updates
- State-specific preparation workflows

### Permit Database Integration Plugins

Optional plugins may connect TrustLens to municipal, county, or state permit databases.

Capabilities may include:

- Permit searches
- Permit history retrieval
- Permit verification
- Inspection record retrieval
- Automated record matching

### Government Records Plugins

Optional plugins may integrate with government data systems providing:

- Property tax records
- Zoning records
- Certificate of occupancy records
- Environmental records
- Municipal compliance records

### HOA Document Plugins

Optional plugins may support HOA documentation workflows.

Capabilities may include:

- HOA document collection
- Rules and restrictions tracking
- Assessment information
- Community disclosure requirements
- HOA document completeness evaluation

### Inspection Provider Plugins

Optional plugins may integrate with inspection providers and inspection data systems.

Capabilities may include:

- Inspection scheduling
- Inspector directory integration
- Inspection report retrieval
- Inspection status tracking
- Inspection recommendation matching

### Contractor and Renovation Plugins

Optional plugins may support contractor and renovation documentation.

Capabilities may include:

- Contractor record management
- Invoice verification
- Renovation timeline creation
- Contractor documentation matching
- Renovation permit matching

### Property Data Plugins

Optional plugins may connect TrustLens with property data providers.

Capabilities may include:

- Property data retrieval
- Property characteristic enrichment
- Historical property information
- Public record enrichment

### Mapping and Geolocation Plugins

Optional plugins may provide:

- Address geocoding
- Jurisdiction identification
- County identification
- Township identification
- Municipal boundary identification
- Location-based compliance routing

### AI Provider Plugins

Optional AI provider plugins may connect TrustLens to additional AI systems.

Capabilities may include:

- External large language models
- Local model adapters
- Specialized document analysis models
- Embedding providers
- Classification models

AI provider plugins shall remain optional so installations can operate without dependency on a specific commercial AI provider.

### OCR Provider Plugins

Optional OCR plugins may provide alternative document recognition engines.

Capabilities may include:

- Image-to-text conversion
- PDF text extraction
- Handwritten document recognition where supported
- Structured form recognition

### Storage Provider Plugins

Optional storage plugins may support alternative document storage systems.

Capabilities may include:

- Local storage
- Self-hosted object storage
- Compatible cloud storage
- Encrypted archival storage

### Notification Plugins

Optional notification plugins may provide:

- Email notifications
- Preparation reminders
- Missing-document alerts
- Compliance task notifications
- Inspection reminders

### Sharing and Access Plugins

Optional plugins may extend controlled sharing capabilities.

Capabilities may include:

- Buyer access portals
- Agent access
- Inspector access
- Attorney access
- Transaction participant access
- Expiring document access
- Permission-based document sharing

## Application Architecture

TrustLens shall use a modular architecture that separates core property transparency functions from optional integrations.

The reference technology stack shall support:

- Python
- FastAPI
- React
- Next.js
- TailwindCSS
- PostgreSQL

Core functionality shall remain usable without optional plugins wherever practical.

Plugins shall interact with TrustLens through defined interfaces and shall not require modifications to unrelated core modules.

## Data Provenance

TrustLens shall distinguish the origin and verification state of information.

Information may be classified as:

- Seller provided
- Uploaded document evidence
- Government sourced
- Third-party sourced
- AI inferred
- Pending verification
- Verified
- Conflicting
- Incomplete

The system shall preserve provenance information where practical so users can determine how a recommendation or property fact was established.

## Human Review

TrustLens shall maintain human oversight for consequential property information.

Users shall be able to:

- Review AI-generated recommendations
- Correct extracted information
- Confirm or reject findings
- Mark information as verified
- Identify information requiring professional review
- Resolve conflicting records
- Control information included in shared reports

AI assistance shall support property preparation rather than replace legal, inspection, appraisal, engineering, or other professional judgment.

## Transparency Workflow

The core workflow shall support the following general process:

- Create a property profile
- Determine the applicable jurisdiction
- Identify disclosure requirements
- Identify potential documentation requirements
- Upload existing property records
- Analyze documents
- Identify missing information
- Review permits and renovations
- Identify recommended inspections
- Request government records where necessary
- Anticipate buyer questions
- Resolve preparation gaps
- Evaluate property readiness
- Review the completed transparency record
- Generate a Transparency Passport
- Share approved information with authorized parties

## Property Readiness States

TrustLens may use preparation states such as:

- Not Started
- In Progress
- Documentation Requested
- Awaiting Verification
- Needs Attention
- Partially Prepared
- Verified
- Listing Ready

Readiness states shall be explainable through the underlying documentation and outstanding tasks.

## API and Integration Requirements

The application programming interface shall support modular access to core TrustLens functions.

API capabilities may include:

- Property management
- Document management
- Disclosure workflows
- Jurisdiction evaluation
- Permit verification
- Inspection preparation
- Compliance evaluation
- Buyer question generation
- Readiness evaluation
- Transparency Passport generation
- Plugin management
- Authentication and authorization

API responses should preserve relevant provenance and verification information.

## OpenProperty Ecosystem

TrustLens is part of the OpenProperty ecosystem.

The ecosystem may include complementary applications such as:

- HouseLens for buyer and renter property intelligence  [https://roxanneardary.com/houselens/](https://roxanneardary.com/houselens/)
- TrustLens for seller preparation and listing transparency

TrustLens shall be designed to operate independently while remaining capable of interoperability with other OpenProperty applications.

## Vision

TrustLens aims to make property listings more complete, documented, understandable, and transparent from the beginning of the transaction process.

The platform combines AI assistance, jurisdiction-aware guidance, property documentation, compliance preparation, and controlled information sharing to help sellers prepare responsibly and help buyers make better-informed decisions.

**Prepared Listings, Happy Buyers.**

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
  - [https://roxanneardary.com/trustlens/](https://roxanneardary.com/trustlens/)

---

# License & Notice Requirements

TrustLens is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- TrustLens specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

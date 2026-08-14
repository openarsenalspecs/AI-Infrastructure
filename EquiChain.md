# EquiChain

**EquiChain — Code-Driven Equity, Mission-Driven Growth**

## Specification

EquiChain is an open source equity and dividend management platform for businesses that want to privately sell stock to long-term investors without becoming publicly traded.

The system is designed around transparent ownership, responsible dividend programs, accurate financial records, regulatory awareness, auditable transactions, and mission-aligned investment. EquiChain provides the infrastructure for businesses to design, administer, document, and report private equity programs while keeping applicable SEC requirements and other regulatory obligations at the forefront.

EquiChain does not operate as a stock exchange or public securities marketplace. It is designed to help private businesses establish structured relationships with investors who intend to participate in the long-term development and longevity of the business.

## Design Principles

- Open source and vendor-neutral architecture
- Modular and extensible design
- Private-market equity management
- Long-term investor alignment
- Transparent financial reporting
- Accurate and auditable records
- Regulatory awareness and compliance support
- Human approval for material financial and legal actions
- Secure handling of investor and corporate information
- Explainable financial calculations
- Traceable ownership and transaction history
- Portable data and open interfaces
- Separation of public and confidential information
- No automated assumption that a transaction is legally compliant without appropriate review

## Core Modules

### Equity Management

The Equity Management module manages the complete lifecycle of privately issued equity.

Features include:

- Company equity configuration
- Authorized and issued equity tracking
- Common and preferred share classes
- Share class rights and restrictions
- Ownership percentages
- Share issuance
- Share transfers
- Share redemptions
- Share cancellations
- Outstanding share calculations
- Capitalization tables
- Historical ownership records
- Ownership change auditing
- Equity transaction validation

All equity transactions must create a traceable record connecting the transaction to the affected ownership records.

### Investor Management

The Investor Management module maintains investor records and relationships.

Features include:

- Investor profiles
- Investment history
- Ownership records
- Share class assignments
- Investor eligibility information
- Required verification records
- Investor agreements
- Investor disclosures
- Distribution history
- Voting rights
- Investor communications
- Document access controls

Sensitive investor information must remain separated from information designated for public disclosure.

### Dividend Management

The Dividend Management module provides the core framework for designing and administering dividend programs.

Features include:

- Dividend policy creation
- Fixed dividend models
- Profit-based dividend models
- Performance-based dividend models
- Tiered dividend models
- Share-class-specific distributions
- Preferred distribution rules
- Dividend eligibility rules
- Dividend declaration
- Dividend accrual
- Dividend calculation
- Dividend approval
- Dividend payment records
- Outstanding dividend tracking
- Historical dividend records

Dividend calculations must be reproducible from the underlying financial and ownership records.

### Profit Allocation

The Profit Allocation module manages how available business profits are allocated.

Features include:

- Dividend allocation
- Business reserve allocation
- Reinvestment allocation
- Debt and obligation allocations
- Retained earnings
- Mission-related allocations
- Configurable allocation policies
- Allocation scenario modeling
- Allocation approvals
- Historical allocation records

Every allocation must identify its source financial period, applicable policy, calculation, approval status, and resulting allocation.

### Financial Records

The Financial Records module maintains the financial information required for accurate equity and dividend administration.

Features include:

- Revenue records
- Expense records
- Profit and loss information
- Balance sheet information
- Cash position tracking
- Retained earnings
- Reserve tracking
- Financial periods
- Financial adjustments
- Financial source references
- Accounting data imports
- Financial validation
- Historical financial records

Financial records must preserve the relationship between reported figures and their underlying source information.

### Transparency and Reporting

The Transparency and Reporting module generates accurate reports for investors, administrators, auditors, and public disclosure where appropriate.

Features include:

- Investor reports
- Ownership reports
- Dividend reports
- Financial reports
- Distribution summaries
- Governance reports
- Compliance reports
- Transaction reports
- Capitalization reports
- Historical reports
- Public transparency reports
- Exportable reports
- Report versioning

Public reporting must only expose information explicitly designated for public disclosure.

### Public Disclosure

The Public Disclosure module provides controlled publication of approved business and financial information.

Features include:

- Public financial summaries
- Public ownership information where permitted
- Dividend declarations
- Distribution summaries
- Corporate information
- Approved governance information
- Filing records
- Disclosure histories
- Publication timestamps
- Historical publication versions

The system must prevent confidential investor information from being unintentionally included in public disclosures.

### Compliance Management

The Compliance Management module provides regulatory workflow support and validation.

Features include:

- Configurable regulatory requirements
- Offering compliance workflows
- Investor eligibility checks
- Disclosure requirements
- Filing requirements
- Compliance deadlines
- Compliance status tracking
- Regulatory event tracking
- Compliance warnings
- Incomplete record detection
- Transaction validation
- Compliance audit records

Compliance functionality must be designed to support applicable SEC requirements and other relevant regulations. The system must distinguish software validation from legal advice and must allow qualified professionals to review material compliance decisions.

### SEC Filing Management

The SEC Filing Management module organizes filing preparation and filing records.

Features include:

- Filing requirement tracking
- Filing data collection
- Filing-ready document generation
- Form D support
- Filing deadline tracking
- Filing status tracking
- Filing history
- Amendment tracking
- Supporting document management
- Filing-to-transaction relationships
- Filing audit records

Filing functionality must be configurable so that regulatory requirements can be updated without rewriting the core equity system.

### Audit Trail

The Audit Trail module provides persistent records of material system activity.

Features include:

- Equity transaction history
- Ownership changes
- Dividend calculations
- Dividend approvals
- Financial changes
- Governance decisions
- Compliance events
- Filing events
- Configuration changes
- User actions
- Approval records
- Timestamps
- Previous and resulting states

Material records must be traceable from the current state back through their historical changes.

### Governance

The Governance module manages shareholder and corporate decision processes.

Features include:

- Governance policies
- Shareholder voting rights
- Voting eligibility
- Proposals
- Voting events
- Vote records
- Approval thresholds
- Resolutions
- Governance decisions
- Governance history
- Decision-to-equity relationships

Governance actions affecting equity, dividends, or other material corporate matters must be linked to the resulting system changes.

### Document Management

The Document Management module manages documents associated with equity and corporate operations.

Features include:

- Shareholder agreements
- Offering documents
- Investor disclosures
- Dividend policies
- Governance resolutions
- Financial reports
- Regulatory filings
- Compliance records
- Corporate policies
- Document versioning
- Approval history
- Document-to-record relationships
- Controlled access

Documents must maintain their historical versions and relationships to the transactions or decisions they support.

### Scenario Modeling

The Scenario Modeling module allows businesses to evaluate potential financial and equity outcomes before implementing changes.

Features include:

- Dividend scenario modeling
- Profit scenarios
- Revenue scenarios
- Growth scenarios
- Reserve scenarios
- Reinvestment scenarios
- Share issuance scenarios
- Ownership scenarios
- Distribution comparisons
- Long-term projection models

Scenario results must remain clearly separated from official financial and ownership records until formally approved.

### Compliance Validation Engine

The Compliance Validation Engine evaluates configured transactions and workflows against applicable rules.

Features include:

- Rule-based validation
- Transaction validation
- Investor eligibility validation
- Dividend rule validation
- Disclosure validation
- Filing requirement validation
- Required-field validation
- Deadline validation
- Exception reporting
- Explainable validation results
- Review status
- Human approval workflows

Validation results must identify the rule applied, the records evaluated, the result, and any required human review.

### Security and Privacy

The Security and Privacy module protects confidential business and investor information.

Features include:

- Authentication
- Authorization
- Role-based access control
- Permission management
- Data separation
- Access logging
- Security event logging
- Secure document access
- Data protection
- Backup support
- Recovery support
- Administrative controls

Public, investor, administrative, financial, and confidential records must be independently controllable through permissions.

### Human Approval

The Human Approval module ensures that material financial, equity, governance, and compliance decisions remain subject to authorized review.

Features include:

- Approval workflows
- Multi-step approvals
- Authorized approvers
- Approval thresholds
- Rejection workflows
- Revision workflows
- Approval history
- Decision timestamps
- Required review status
- Audit integration

Automation must not independently finalize material actions where human authorization is required.

### Workflow Automation

The Workflow Automation module manages recurring operational processes.

Features include:

- Filing reminders
- Dividend reminders
- Reporting schedules
- Approval notifications
- Compliance notifications
- Document workflows
- Investor notifications
- Recurring reporting
- Scheduled calculations
- Administrative workflows

Automated workflows must preserve audit records and respect configured approval requirements.

### API

The API module provides controlled programmatic access to EquiChain.

Features include:

- REST interfaces
- Event-driven interfaces
- Authentication
- Authorization
- Equity endpoints
- Investor endpoints
- Dividend endpoints
- Financial endpoints
- Governance endpoints
- Compliance endpoints
- Reporting endpoints
- Audit endpoints
- Webhook support
- API activity logging

API access must respect the same security, privacy, validation, and audit requirements as the primary application.

### Data Import and Export

The Data Import and Export module supports data portability.

Features include:

- Investor data import
- Equity data import
- Financial data import
- Transaction import
- Historical data migration
- Structured exports
- Report exports
- Filing exports
- Audit exports
- Backup exports
- Data validation
- Migration integrity checks

Imported data must be validated before becoming authoritative system records.

### Testing and Verification

The Testing and Verification module establishes requirements for financial and operational correctness.

Features include:

- Equity calculation testing
- Ownership testing
- Dividend calculation testing
- Financial calculation testing
- Compliance workflow testing
- Filing generation testing
- Governance testing
- Reporting accuracy testing
- Security testing
- Integration testing
- Regression testing
- Scenario testing

Critical financial calculations must have reproducible tests and documented expected results.

### Change Management

The Change Management module tracks changes to policies, rules, configurations, and other material system behavior.

Features include:

- Dividend policy versioning
- Equity rule versioning
- Governance rule versioning
- Compliance rule versioning
- Configuration history
- Approval requirements
- Effective dates
- Previous versions
- Change attribution
- Change audit records

Material rule changes must not silently alter historical calculations or previously finalized records.

## Optional Plugin Modules

EquiChain supports optional plugins that extend the core system without changing foundational functionality.

### Accounting Integration Plugins

Optional accounting plugins may connect EquiChain with external accounting systems.

Capabilities may include:

- Financial data synchronization
- Profit and loss imports
- Balance sheet imports
- Transaction synchronization
- Reconciliation
- Accounting source references

### Regulatory Plugins

Regulatory plugins may provide jurisdiction-specific requirements.

Capabilities may include:

- Federal regulatory rules
- State securities requirements
- Filing requirements
- Disclosure requirements
- Deadline calendars
- Jurisdiction-specific validation

### Filing Plugins

Filing plugins may support additional regulatory filing formats.

Capabilities may include:

- Additional SEC forms
- State filings
- Regulatory document generation
- Filing validation
- Filing submission preparation

### Dividend Model Plugins

Dividend plugins may introduce additional distribution methodologies.

Capabilities may include:

- Custom formulas
- Industry-specific models
- Performance-based models
- Revenue-based models
- Multi-tier distribution models
- Custom preferred distribution rules

### Investor Verification Plugins

Investor verification plugins may connect to external verification services.

Capabilities may include:

- Identity verification
- Investor eligibility verification
- Accredited investor verification
- Required document verification
- Verification status synchronization

### Financial Analysis Plugins

Financial analysis plugins may extend scenario modeling and business analysis.

Capabilities may include:

- Financial forecasting
- Cash flow analysis
- Dividend sustainability analysis
- Reserve analysis
- Growth modeling
- Sensitivity analysis

### Public Transparency Plugins

Public transparency plugins may extend approved disclosure capabilities.

Capabilities may include:

- Public dashboards
- Financial transparency portals
- Investor statistics
- Dividend histories
- Public filing libraries
- Corporate transparency reports

### Notification Plugins

Notification plugins may connect EquiChain to external communication systems.

Capabilities may include:

- Email notifications
- Application notifications
- Investor alerts
- Compliance alerts
- Filing reminders
- Dividend notifications

### Analytics Plugins

Analytics plugins may provide additional analysis without altering authoritative records.

Capabilities may include:

- Investor analytics
- Ownership analysis
- Dividend analytics
- Financial trends
- Scenario comparisons
- Operational metrics

### Governance Plugins

Governance plugins may extend voting and corporate decision functionality.

Capabilities may include:

- Advanced voting models
- Proxy workflows
- Electronic resolutions
- Voting analytics
- Governance dashboards

### Localization Plugins

Localization plugins may adapt EquiChain for additional jurisdictions and languages.

Capabilities may include:

- Language support
- Currency support
- Date and number formats
- Jurisdiction-specific terminology
- Local reporting requirements

## Data Integrity Requirements

EquiChain must maintain authoritative records for:

- Equity
- Ownership
- Investors
- Transactions
- Dividends
- Financial information
- Governance
- Compliance
- Filings
- Disclosures
- Approvals
- Documents
- Audit events

Records must preserve their relationships and historical state.

No calculation that materially affects ownership, dividends, financial reporting, or compliance should depend on an undocumented assumption.

## Transparency Requirements

EquiChain must make material financial and equity calculations understandable and traceable.

The system should identify:

- Source records
- Calculation rules
- Applicable policies
- Calculation periods
- Adjustments
- Approvals
- Final results

Public transparency must balance accurate disclosure with the protection of confidential investor and business information.

## Regulatory Requirements

EquiChain is intended to support private securities administration while keeping applicable securities regulations at the forefront.

The system must:

- Support configurable regulatory requirements.
- Track applicable compliance obligations.
- Preserve records required for regulatory review.
- Generate filing-ready information.
- Track filing deadlines.
- Maintain filing histories.
- Support appropriate investor eligibility workflows.
- Provide compliance warnings.
- Preserve an audit trail.
- Require human review where appropriate.
- Avoid representing automated validation as legal advice.

Businesses remain responsible for determining which securities laws and regulations apply to their activities and for obtaining qualified legal, accounting, and compliance advice when necessary.

## Mission-Aligned Investment

EquiChain is designed for businesses that want investors who are interested in the long-term success and mission of the company rather than short-term public-market trading.

The platform may support:

- Long-term ownership policies
- Mission statements
- Investor communications
- Mission-related disclosures
- Dividend policies
- Reinvestment policies
- Governance participation
- Long-term financial planning

The system does not guarantee investor behavior or investment outcomes.

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
  - [https://roxanneardary.com/equichain/](https://roxanneardary.com/equichain/)

---

## License & Notice Requirements

**EquiChain** is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- **EquiChain** specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

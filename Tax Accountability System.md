# Tax Accountability System
**Recover Public Funds. Return Public Value.**
- HTML Mirror:  [https://roxanneardary.com/tax-accountability-system-specification/](https://roxanneardary.com/tax-accountability-system-specification/)  

---

## Specification

Tax Accountability System is a modular specification for transparent, government-controlled property tax recovery, statutory redemption, foreclosure, tax forfeiture, public property disposition, financial accountability, and equal township-wide homestead rebates.

The specification is designed to ensure that delinquent property taxes remain a government-administered public obligation rather than becoming an investment product for private tax-lien investors. The system provides a transparent process beginning with tax delinquency and continuing through redemption, foreclosure, government forfeiture, property sale, expense accounting, excess-proceeds calculation, and equal public distribution.

The system is designed for government entities, municipalities, townships, counties, and other jurisdictions seeking an accountable framework for administering delinquent property taxes and forfeited properties.

## Core Principles

- Government-controlled tax recovery
- No sale of delinquent tax liens to private investors
- Public accountability
- Public transparency
- Modular architecture
- Mandatory due process
- 60-day delinquency threshold
- 24-month statutory redemption period
- Government-controlled foreclosure and forfeiture
- Complete property-level financial accounting
- Transparent property sales
- Transparent property expenses
- Transparent excess-proceeds accounting
- Equal township-wide public benefit
- Primary-home equality
- Human oversight of automated systems
- Auditable government action
- Privacy-conscious public records
- Open and machine-readable public information

---

## Core Modules

### Tax Delinquency Module

The Tax Delinquency Module manages property tax obligations and determines when a property enters formal delinquency.

Features include:

- Tax obligation registration
- Tax billing records
- Tax due-date tracking
- Payment status tracking
- 60-day grace-period tracking
- Formal delinquency date calculation
- Formal delinquency status creation after more than 60 days past due
- Property-level delinquency tracking
- First delinquency tracking
- Second delinquency tracking
- Third delinquency tracking
- Historical delinquency records
- Delinquency resolution tracking
- Payment recording
- Partial-payment recording
- Full-payment recording
- Redemption recording
- Delinquency cancellation
- Foreclosure eligibility calculation

### Delinquency Notice Module

The Delinquency Notice Module manages required notifications when a property enters formal delinquency and throughout the redemption and foreclosure process.

Features include:

- Automated delinquency notices
- Formal delinquency notices
- Redemption-period notices
- Periodic delinquency notices
- Final redemption notices
- Foreclosure notices
- Forfeiture notices
- Notice generation
- Notice delivery tracking
- Notice publication
- Notice delivery confirmation
- Failed-delivery tracking
- Notice history
- Notice timestamping
- Public notice verification
- Required notice sequencing
- Notice compliance validation

### Public Delinquency Registry Module

The Public Delinquency Registry Module maintains a publicly accessible record of properties that have entered formal delinquency.

The registry must be freely viewable by the public and must not require an account for basic public access.

Features include:

- Public online delinquency registry
- Free public access
- Property address search
- Parcel number search
- Tax account search
- Jurisdiction search
- Delinquency status search
- Original tax due date
- Formal delinquency date
- Redemption commencement date
- Redemption expiration date
- Remaining redemption period
- Delinquent tax balance
- Authorized fees
- Notice history
- Redemption status
- Foreclosure eligibility status
- Foreclosure status
- Forfeiture status
- Government ownership status
- Property disposition status
- Public property timeline
- Historical status records
- Downloadable public records
- Machine-readable records
- Public API
- Registry update timestamps
- Registry audit history

### Statutory Redemption Module

The Statutory Redemption Module establishes and administers the mandatory redemption period.

The redemption period begins when a property remains unpaid for more than 60 days after the applicable tax payment due date.

The statutory redemption period must be 24 months.

Features include:

- Mandatory 24-month statutory redemption period
- Redemption period beginning after the 60-day delinquency threshold
- Redemption commencement tracking
- Redemption expiration tracking
- Remaining-time calculation
- Owner redemption payments
- Partial-payment tracking
- Full redemption processing
- Redemption confirmation
- Redemption receipts
- Redemption status publication
- Automatic redemption deadline calculation
- Automatic foreclosure eligibility calculation
- Prevention of premature foreclosure
- Redemption audit trail

Foreclosure must not begin before the statutory redemption period has expired and all required notice and due-process requirements have been satisfied.

### Interest Management Module

The Interest Management Module establishes the rules governing interest on delinquent property taxes.

The system must not impose interest during the first or second delinquency.

Interest may become permissible when the same property reaches a third separate delinquency, subject to applicable law and the rules established by the jurisdiction implementing the specification.

Features include:

- No interest on first delinquency
- No interest on second delinquency
- Third-delinquency detection
- Separate delinquency occurrence tracking
- Third-delinquency interest activation
- Prospective interest calculation
- Interest-rate tracking
- Interest accrual tracking
- Interest accounting
- Interest payment tracking
- Interest disclosure
- No retroactive interest on first delinquency
- No retroactive interest on second delinquency
- Interest audit trail
- Interest earned on retained proceeds tracking

### Notice & Due Process Module

The Notice & Due Process Module verifies that all legally required procedures have been completed before foreclosure or forfeiture.

Features include:

- Statutory notice management
- Due-process verification
- Notice sequencing
- Notice deadline tracking
- Administrative review
- Owner response tracking
- Appeal tracking
- Hearing management
- Evidence management
- Dispute resolution
- Foreclosure holds
- Forfeiture holds
- Procedural compliance verification
- Due-process audit trail

### Payment & Redemption Module

The Payment & Redemption Module manages payments made to resolve delinquent property taxes and redeem properties.

Features include:

- Electronic payment support
- Government payment processing
- Payment receipt generation
- Payment allocation
- Payment history
- Partial-payment tracking
- Full-payment tracking
- Payment reconciliation
- Returned-payment tracking
- Payment correction
- Redemption balance calculation
- Redemption status
- Payment audit trail

### Foreclosure Eligibility Module

The Foreclosure Eligibility Module determines whether a property has satisfied every prerequisite for foreclosure.

Features include:

- 24-month redemption verification
- Delinquency verification
- Notice-completion verification
- Due-process verification
- Payment-status verification
- Appeal-status verification
- Property-status verification
- Foreclosure eligibility calculation
- Eligibility timestamp
- Foreclosure hold detection
- Automated eligibility audit
- Human authorization requirement
- Public foreclosure eligibility status

### Government Foreclosure Module

The Government Foreclosure Module administers foreclosure proceedings after all eligibility requirements have been satisfied.

Features include:

- Foreclosure case creation
- Foreclosure case management
- Foreclosure filing tracking
- Court proceeding tracking
- Judgment tracking
- Foreclosure completion
- Government title acquisition
- Title transfer recording
- Foreclosure status publication
- Foreclosure documentation
- Foreclosure audit trail

### Tax Forfeiture Module

The Tax Forfeiture Module manages government acquisition and administration of properties following successful foreclosure.

Features include:

- Government acquisition of forfeited property
- Tax-forfeiture designation
- Forfeiture status tracking
- Government property inventory
- Government ownership records
- Title tracking
- Property condition assessment
- Property maintenance tracking
- Property preservation
- Property security
- Property disposition authorization
- Public forfeiture records
- Forfeiture audit trail

### Primary Residence & Citizenship Module

The Primary Residence & Citizenship Module manages eligibility requirements for residential properties disposed of under the specification.

Residential forfeited properties designated for residential disposition may only be sold as primary residences to verified U.S. citizens, subject to applicable federal and state law.

Features include:

- Primary-residence definition
- Primary-residence verification
- Buyer identity verification
- U.S. citizenship verification
- Citizenship verification before closing
- Primary-residence certification
- Buyer occupancy certification
- Ownership verification
- Closing eligibility determination
- Primary-residence compliance monitoring
- Fraud prevention
- Duplicate ownership detection
- Verification audit trail
- Privacy-protected verification records
- Government-only access to sensitive verification information
- Public non-sensitive verification status
- Post-sale occupancy verification

Sensitive citizenship and identity documentation must not be exposed through the public registry.

### Property Disposition Module

The Property Disposition Module governs the disposition of government-owned forfeited residential properties.

Residential properties subject to the primary-residence disposition requirements must be sold only for use as primary residences to verified U.S. citizens, subject to applicable law.

Features include:

- Primary-residence-only residential sales
- Primary-residence buyer requirement
- Verified U.S. citizen purchaser requirement
- Buyer identity verification
- Citizenship verification
- Primary-residence declaration
- Occupancy commitment
- Pre-closing eligibility verification
- Closing eligibility enforcement
- Investor purchase prohibition
- Rental-only purchase prohibition
- Vacation-home purchase prohibition
- Second-home purchase prohibition
- Speculative acquisition prohibition
- Short-term rental restriction
- Post-sale occupancy monitoring
- Primary-residence compliance monitoring
- Disposition eligibility enforcement
- Government transfer restrictions
- Public disposition records

### Property Sale Transparency Module

The Property Sale Transparency Module requires complete public disclosure of the financial terms and material records associated with the sale of a forfeited property.

Features include:

- Public property sale listing
- Public sale date
- Public sale method
- Public sale terms
- Public final home sale price
- Public winning bid
- Public bid history
- Public number of bids
- Public buyer classification
- Public transfer price
- Pre-sale valuation
- Appraisal records
- Property condition records
- Sale documentation
- Closing documentation
- Transfer documentation
- Post-sale accounting
- Sale audit trail

### Property Expense Transparency Module

The Property Expense Transparency Module requires every expense charged against a forfeited property or deducted from its sale proceeds to be documented and publicly disclosed.

Features include:

- Complete property expense tracking
- Itemized expense disclosure
- Legal expense disclosure
- Foreclosure expense disclosure
- Court-cost disclosure
- Recording-fee disclosure
- Title expense disclosure
- Property maintenance disclosure
- Property preservation disclosure
- Inspection expense disclosure
- Utility expense disclosure
- Insurance expense disclosure
- Repair expense disclosure
- Cleaning expense disclosure
- Landscaping expense disclosure
- Security expense disclosure
- Property management expense disclosure
- Auction expense disclosure
- Marketing expense disclosure
- Commission disclosure
- Transfer expense disclosure
- Closing expense disclosure
- Government administrative expense disclosure
- Other authorized expense disclosure

No undocumented, unclassified, or undisclosed expense may be deducted from property-sale proceeds.

### Expense Documentation Module

The Expense Documentation Module establishes the documentation requirements for every property expense.

Features include:

- Expense category
- Expense amount
- Expense date
- Vendor identification
- Government department identification
- Service description
- Property association
- Authorization record
- Payment date
- Payment method
- Invoice documentation
- Contract documentation
- Supporting documentation
- Legal-recoverability designation
- Public expense record
- Expense audit trail
- Expense reconciliation
- No undocumented deductions
- No unclassified expenses
- No undisclosed expenses

### Property Financial Ledger Module

The Property Financial Ledger Module maintains a complete financial record for each property.

Features include:

- Property-level financial ledger
- Tax liability ledger
- Payment ledger
- Fee ledger
- Interest ledger
- Expense ledger
- Sale proceeds ledger
- Excess proceeds ledger
- Rebate allocation ledger
- Transaction timestamps
- Transaction identifiers
- Source documentation
- Automated reconciliation
- Ledger audit trail
- Public financial summary
- Authorized detailed public records

### Excess Proceeds Module

The Excess Proceeds Module determines the amount remaining after a forfeited property is sold and all legally authorized obligations and documented expenses have been satisfied.

Eligible excess proceeds may include:

- Surplus property-sale proceeds
- Interest earned on retained excess proceeds
- Other legally distributable earnings associated with the proceeds

The module must provide a complete accounting showing:

- Gross property sale proceeds
- Delinquent tax recovery
- Authorized costs
- Documented property expenses
- Interest earned
- Net distributable excess proceeds

Features include:

- Gross property sale proceeds calculation
- Delinquent-tax recovery calculation
- Authorized-cost calculation
- Property-expense calculation
- Interest-earned calculation
- Net proceeds calculation
- Excess-proceeds determination
- Township-wide excess-proceeds pool
- Public excess-proceeds accounting
- Property-level reconciliation
- Sale-to-rebate traceability
- Complete proceeds audit trail
- No undisclosed deductions
- No diversion of eligible excess proceeds

### Homestead Rebate Module

The Homestead Rebate Module distributes eligible excess proceeds equally among all primary homes within the township.

Primary-home ownership is the sole eligibility criterion.

There are no additional qualification requirements based on:

- Property size
- Lot size
- Property value
- Assessed value
- Market value
- Household size
- Household income
- Age
- Disability status
- Tax liability
- Amount of taxes previously paid
- Mortgage status
- Length of ownership
- Neighborhood
- Any other socioeconomic or property characteristic

Features include:

- Township-wide rebate pool
- Primary-home ownership registry
- Primary-home identification
- Equal-share calculation
- One equal share per primary home
- Equal rebate amount
- Automated rebate calculation
- Rebate payment processing
- Rebate payment tracking
- Distribution reconciliation
- Public aggregate rebate reporting
- Rebate audit trail

### Equal Distribution Rules Module

The Equal Distribution Rules Module enforces equal treatment of all primary homes.

The distribution formula is:

Total Distributable Excess Proceeds divided by Total Primary Homes equals Equal Primary Home Rebate

Features include:

- Equal distribution
- One equal share per primary home
- Primary-home ownership as the sole rebate eligibility criterion
- No property-size-based allocation
- No lot-size-based allocation
- No assessed-value-based allocation
- No market-value-based allocation
- No household-size-based allocation
- No income-based allocation
- No age-based allocation
- No disability-based allocation
- No neighborhood-based allocation
- No tax-payment-based allocation
- No mortgage-based allocation
- No length-of-ownership-based allocation
- No socioeconomic allocation
- No discretionary allocation
- No preferential allocation
- No variable rebate formula

### AI Excess-Proceeds Engine Module

The AI Excess-Proceeds Engine supports administrative verification and mathematical distribution of the township-wide rebate pool.

The AI must operate under government-defined rules and must not create independent eligibility standards.

Features include:

- Automated primary-home count
- Primary-home ownership verification
- Equal-share calculation
- One-share-per-primary-home enforcement
- Duplicate detection
- Data validation
- Distribution reconciliation
- Mathematical verification
- Automated error detection
- Reproducible calculations
- Calculation audit trail
- Distribution simulation
- Exception reporting
- Human review controls
- Rule-based AI constraints

### AI Governance Module

The AI Governance Module establishes controls over all AI-assisted functions.

Features include:

- Government-defined rules
- Deterministic allocation requirements
- Human oversight
- AI activity logging
- Calculation explainability
- Reproducible outputs
- Audit records
- Error detection
- Exception reporting
- No autonomous policy creation
- No autonomous eligibility expansion
- No autonomous eligibility restriction
- No income-based decision-making
- No property-value-based decision-making
- No property-size-based decision-making
- No variable rebate calculations
- Equal-treatment enforcement

### Financial Transparency Module

The Financial Transparency Module provides public visibility into the complete financial lifecycle of each forfeited property.

Features include:

- Public gross sale price
- Public itemized expenses
- Public recovered tax amount
- Public authorized costs
- Public interest amounts
- Public interest earnings
- Public excess-proceeds amount
- Public rebate-pool amount
- Public equal-rebate amount
- Public distribution totals
- Vendor payment disclosure
- Government expense disclosure
- Transaction timestamps
- Supporting documentation
- Public financial reconciliation
- Property-level financial reporting
- Township-wide financial reporting
- No undisclosed deductions

### Public Transparency Module

The Public Transparency Module provides public access to records and information generated by the system.

Features include:

- Public delinquency records
- Public redemption records
- Public foreclosure records
- Public forfeiture records
- Public government property inventory
- Public sale records
- Public sale prices
- Public bid information
- Public property expenses
- Public proceeds calculations
- Public interest calculations
- Public excess-proceeds calculations
- Public rebate calculations
- Public aggregate rebate distributions
- Public audit records
- Public transaction histories
- Open data exports
- Machine-readable datasets
- Public API
- Transparency dashboard

### Audit & Records Module

The Audit & Records Module maintains a complete historical record of system activity.

Features include:

- Complete property history
- Complete delinquency history
- Complete payment history
- Complete notice history
- Complete redemption history
- Complete foreclosure history
- Complete forfeiture history
- Complete expense history
- Complete sale history
- Complete proceeds history
- Complete rebate history
- Complete AI calculation history
- Immutable or tamper-evident records
- Records retention
- Public verification tools
- Administrative audit tools
- Historical version tracking

### Reporting Module

The Reporting Module generates standardized government and public accountability reports.

Features include:

- Delinquency reports
- Redemption reports
- Foreclosure reports
- Forfeiture reports
- Property inventory reports
- Property disposition reports
- Property sale reports
- Property expense reports
- Interest reports
- Excess-proceeds reports
- Homestead rebate reports
- Township financial reports
- Public transparency reports
- AI calculation reports
- Audit reports
- Annual accountability reports

### Public Data & API Module

The Public Data & API Module provides structured access to public system information.

Features include:

- Public data portal
- Open data exports
- Machine-readable records
- Property-level data access
- Delinquency data access
- Sale data access
- Expense data access
- Proceeds data access
- Rebate data access
- Statistical data access
- Public read-only API
- API documentation
- Data versioning
- Data integrity verification

### Security & Privacy Module

The Security & Privacy Module protects administrative records and sensitive personal information while maintaining public transparency.

Features include:

- Role-based access control
- Government administrative authentication
- Sensitive-record protection
- Identity-data protection
- Citizenship-record protection
- Encryption
- Secure document storage
- Audit logging
- Data integrity controls
- Fraud detection
- Unauthorized-change detection
- Public/private data separation
- Privacy-preserving public records
- Sensitive information access controls

---

## Optional Plugin Modules

The modular architecture may support optional plugins that extend functionality without altering the core accountability requirements.

### Payment Plan Plugin

- Structured payment plans
- Payment-plan eligibility
- Payment schedules
- Payment compliance tracking
- Payment-plan status
- Automatic delinquency updates

### Hardship Assistance Plugin

- Hardship application management
- Government assistance programs
- Temporary foreclosure holds
- Assistance status tracking
- Resolution tracking

### Appeals Plugin

- Administrative appeals
- Appeal filing
- Evidence submission
- Hearing scheduling
- Decision tracking
- Appeal audit records

### Tax Exemption Integration Plugin

- Tax exemption data integration
- Homestead exemption integration
- Exemption status verification
- Government tax-record synchronization

### GIS & Mapping Plugin

- Property mapping
- Delinquency mapping
- Foreclosure mapping
- Forfeiture mapping
- Government property mapping
- Public transparency maps

### Property Rehabilitation Plugin

- Property rehabilitation planning
- Repair management
- Contractor tracking
- Rehabilitation expenses
- Property condition improvements
- Rehabilitation audit records

### Land Bank Integration Plugin

- Land bank transfers
- Land bank inventory synchronization
- Property disposition tracking
- Community development integration

### Public Housing Integration Plugin

- Public housing transfers
- Affordable housing disposition
- Housing development integration
- Public housing inventory

### Automated Notification Plugin

- Email notifications
- SMS notifications
- Public alerts
- Deadline reminders
- Status-change notifications

### Intergovernmental Data Exchange Plugin

- County integration
- Township integration
- Municipal integration
- State integration
- Tax-record synchronization
- Property-record synchronization

### Document Management Plugin

- Electronic document storage
- Document indexing
- Document versioning
- Document retrieval
- Public document publishing
- Records retention integration

### Electronic Payment Plugin

- Online tax payments
- Electronic redemption payments
- Payment receipts
- Payment reconciliation
- Secure payment processing

### Analytics & Forecasting Plugin

- Delinquency analytics
- Redemption forecasting
- Foreclosure forecasting
- Forfeiture forecasting
- Revenue forecasting
- Excess-proceeds forecasting
- Township rebate forecasting

### Open Data Plugin

- Open datasets
- Bulk data exports
- Data catalogs
- Dataset versioning
- Public data feeds
- Open-data documentation

### Mobile Access Plugin

- Mobile public registry
- Mobile delinquency search
- Mobile property status
- Mobile notifications
- Mobile public reporting

### Multilingual Public Access Plugin

- Multilingual registry
- Multilingual notices
- Multilingual public records
- Language selection
- Accessible government information

### Community Development Plugin

- Community property disposition
- Community development projects
- Public-use property transfers
- Neighborhood redevelopment tracking

### Housing Preservation Plugin

- Primary-home preservation
- Residential rehabilitation
- Owner occupancy monitoring
- Housing preservation programs
- Community housing initiatives

### External Records Integration Plugin

- Government records integration
- Property records integration
- Ownership records integration
- Public records synchronization
- External data validation

---

## System Requirements

Implementations conforming to this specification should:

- Preserve the modular architecture
- Implement all required core modules
- Preserve the 60-day formal delinquency threshold
- Preserve the 24-month statutory redemption period
- Prevent premature foreclosure
- Maintain a publicly viewable delinquency registry
- Maintain complete financial records
- Publicly disclose property sale prices
- Publicly disclose itemized property expenses
- Prevent undocumented deductions
- Maintain transparent excess-proceeds calculations
- Distribute eligible excess proceeds equally among primary homes
- Preserve the equal-distribution requirements
- Maintain auditable records
- Apply AI only within defined governance controls
- Protect sensitive personal information
- Preserve applicable due-process requirements
- Maintain AGPL-3.0+ compliance

## Compliance & Extensibility

The specification is designed to be jurisdiction-aware and extensible. Implementations may incorporate additional statutory requirements, government procedures, reporting requirements, or public programs provided that those additions do not undermine the core transparency, accountability, redemption, financial disclosure, equal-distribution, and auditability requirements of the specification.

Optional plugins may extend the capabilities of an implementation without requiring changes to the core modules. Plugins must not be used to circumvent required public records, the statutory redemption period, financial transparency, equal distribution of eligible excess proceeds, or required due-process protections.

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
  - [https://roxanneardary.com/tax-accountability-system/](https://roxanneardary.com/tax-accountability-system/)  

---

## License & Notice Requirements

Tax Accountability System is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Tax Accountability System specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

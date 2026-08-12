# CampGrid

## Know Your Campground From the Ground Up.

CampGrid is an **AGPL-3.0+ open source campground management specification** for campgrounds, RV parks, seasonal communities, recreational properties, resorts, and mixed-ownership campground communities.

CampGrid provides a modular framework for managing the physical, operational, financial, maintenance, rental, ownership, community, accounting, and tax dimensions of a campground within a unified system.

The specification is designed around a simple principle:

> **Every site, asset, service, expense, owner, rental, and financial transaction should be connected and accountable.**

CampGrid is designed to operate locally, support self-hosted implementations, remain vendor-neutral, provide complete data portability, and allow operators to deploy only the modules required for their campground.

## Core Design Principles

CampGrid is built around the following principles:

- **Modular design**
- **Open source implementation**
- **Local-first operation**
- **Vendor neutrality**
- **Data portability**
- **Complete financial visibility**
- **Transparent shared expenses**
- **Accurate cost attribution**
- **Private ownership support**
- **Comprehensive maintenance management**
- **Full asset lifecycle management**
- **Configurable taxation**
- **Auditable accounting**
- **Human-controlled financial decisions**
- **Interoperability**
- **Extensible plugin architecture**
- **Operational optimization**
- **Community transparency**

## Core Modules

### Campground Management

The Campground Management module establishes the physical and organizational model of the campground.

Features include:

- Campground properties
- Multiple property support
- Buildings
- Structures
- RV sites
- Tent sites
- Seasonal sites
- Monthly sites
- Annual sites
- Full-hookup sites
- Partial-hookup sites
- Primitive sites
- Cabins
- Cottages
- Park models
- Rental units
- Storage spaces
- Parking areas
- Common areas
- Recreational facilities
- Infrastructure
- Site classifications
- Site attributes
- Site availability
- Site occupancy
- Geographic campground mapping
- Physical asset identification
- Site-specific pricing
- Site-specific expenses
- Site-specific revenue

### Site and Space Management

The Site and Space Management module manages the individual spaces that make up the campground.

Features include:

- Digital site maps
- Site boundaries
- Site dimensions
- Site types
- Utility connections
- Utility availability
- Site amenities
- Site restrictions
- Vehicle restrictions
- RV restrictions
- Pet policies
- Occupancy limits
- Accessibility information
- Site pricing
- Site expenses
- Site maintenance history
- Site revenue
- Site profitability

### Reservation Management

The Reservation Management module manages transient, seasonal, recurring, and long-term reservations.

Features include:

- Online reservations
- Staff-created reservations
- Walk-in reservations
- Telephone reservations
- Group reservations
- Multi-site reservations
- Recurring reservations
- Seasonal reservations
- Monthly reservations
- Annual reservations
- Reservation calendars
- Availability management
- Check-in management
- Check-out management
- Early check-in
- Late check-out
- Reservation extensions
- Site transfers
- Deposits
- Security deposits
- Cancellation fees
- No-show fees
- Refunds
- Credits
- Discounts
- Promotions
- Rate overrides
- Reservation history
- Guest history

### Rental Management

The Rental Management module manages campground-owned or campground-operated rental assets.

Supported rental assets include:

- RVs
- Cabins
- Cottages
- Park models
- Lodging units
- Equipment
- Recreational equipment
- Storage units
- Other campground-managed rental assets

Features include:

- Rental inventory
- Rental calendars
- Rental pricing
- Rental deposits
- Rental revenue
- Rental expenses
- Rental maintenance
- Rental cleaning
- Rental utilities
- Rental supplies
- Rental insurance
- Rental depreciation
- Rental occupancy
- Rental profitability
- Rental forecasting

Each rental asset should maintain an independent financial profile allowing management to determine its actual cost and profitability.

### Private Ownership Management

The Private Ownership Management module supports communities where individuals own RVs, park models, cabins, cottages, or other structures located within a campground.

Features include:

- Owner records
- Ownership history
- Ownership dates
- Unit ownership
- Site ownership relationships
- Community agreements
- Owner obligations
- Owner charges
- Owner payments
- Owner balances
- Owner statements
- Owner maintenance requests
- Owner-specific expenses
- Shared community expenses
- Special assessments
- Utility charges
- Trash charges
- Pool charges
- Landscaping charges
- Road maintenance charges
- Community service charges

The system must distinguish between campground-owned assets and privately owned assets.

### Community Management

The Community Management module supports campgrounds that function as shared communities.

Features include:

- Community member management
- Residents
- Seasonal occupants
- Long-term occupants
- Visitors
- Vehicles
- Pets
- Community rules
- Community policies
- Community notices
- Community fees
- Community services
- Community assessments
- Special assessments
- Shared infrastructure
- Community facilities
- Community financial records

### Maintenance Management

The Maintenance Management module provides complete maintenance management for campground property, infrastructure, facilities, equipment, rental assets, and privately owned units where campground services are provided.

Features include:

- Preventive maintenance
- Corrective maintenance
- Emergency maintenance
- Scheduled maintenance
- Recurring maintenance
- Maintenance requests
- Work orders
- Inspections
- Maintenance checklists
- Asset maintenance histories
- Maintenance priorities
- Maintenance status
- Maintenance costs
- Maintenance budgets
- Maintenance forecasting
- Maintenance documentation
- Maintenance photographs
- Warranty tracking
- Service contract tracking

### Work Order Management

The Work Order Management module tracks the complete lifecycle of maintenance work.

Features include:

- Employee work orders
- Owner work orders
- Guest maintenance requests
- Preventive work orders
- Emergency work orders
- Vendor work orders
- Asset-specific work orders
- Site-specific work orders
- Labor tracking
- Parts tracking
- Equipment tracking
- Vendor costs
- Internal labor costs
- External labor costs
- Work order approvals
- Work order documentation
- Chargeable work identification
- Work order cost attribution

### Private Owner Maintenance

The Private Owner Maintenance module determines responsibility and billing when campground personnel or vendors perform services for privately owned units.

The system should distinguish among:

- Campground responsibility
- Owner responsibility
- Shared responsibility
- Warranty responsibility
- Vendor responsibility

Features include:

- Owner maintenance requests
- Responsibility determination
- Owner approvals
- Labor allocation
- Material allocation
- Equipment allocation
- Administrative cost allocation
- Vendor charges
- Owner charge generation
- Owner maintenance statements

### Asset Management

The Asset Management module tracks the complete lifecycle of campground assets.

Supported assets include:

- Land
- Buildings
- Roads
- Bridges
- Pools
- Bathhouses
- Restrooms
- Clubhouses
- Utility infrastructure
- Electrical systems
- Water systems
- Sewer systems
- Septic systems
- Landscaping infrastructure
- Recreation facilities
- Vehicles
- Maintenance equipment
- Rental equipment
- Furniture
- Fixtures
- Technology infrastructure

Asset records should support:

- Acquisition date
- Acquisition cost
- Installation cost
- Improvements
- Current value
- Useful life
- Depreciation
- Maintenance history
- Repair history
- Replacement schedule
- Warranty
- Insurance
- Operating cost
- Capital cost
- Disposal history

### Community Services

The Community Services module manages services that benefit multiple campground sites, residents, owners, guests, or facilities.

Supported services include:

- Trash removal
- Recycling
- Pool maintenance
- Landscaping
- Road maintenance
- Snow removal
- Security
- Pest control
- Water services
- Sewer services
- Septic services
- Common electricity
- Common lighting
- Internet
- Cable
- Recreation facilities
- Laundry facilities
- Bathhouses
- Clubhouses
- Community buildings

The module records the actual cost of providing each shared service and connects those costs to the applicable beneficiaries.

### Shared Expense Allocation

The Shared Expense Allocation module distributes common campground expenses according to configurable allocation rules.

Supported allocation methods include:

- Equal allocation
- Per-site allocation
- Per-unit allocation
- Per-occupant allocation
- Occupancy-based allocation
- Usage-based allocation
- Meter-based allocation
- Revenue-based allocation
- Ownership-based allocation
- Square-footage allocation
- Fixed-fee allocation
- Tiered allocation
- Percentage allocation
- Hybrid allocation
- Custom allocation formulas

The system should allow multiple allocation methods to coexist.

For example, a community service may use:

- A fixed base fee
- An occupancy component
- A usage component

The allocation engine must retain the formula used to calculate each charge.

### Shared Expense Transparency

Every shared expense should be traceable from its original source to the individual charges generated from it.

A shared expense record should support:

- Vendor
- Contract
- Invoice
- Service period
- Total cost
- Applicable properties
- Applicable sites
- Applicable units
- Applicable owners
- Applicable rental units
- Allocation methodology
- Allocation formula
- Individual allocations
- Supporting documentation
- Approval history
- Accounting entries

The system should allow a user to answer:

> **Why was I charged this amount?**

The answer should include the underlying expense, allocation method, calculation, and supporting documentation.

### Utilities Management

The Utilities Management module tracks utility infrastructure, consumption, costs, and reimbursement.

Supported utilities include:

- Electricity
- Water
- Sewer
- Propane
- Natural gas
- Internet
- Cable
- Wastewater
- Other campground utilities

Features include:

- Master meters
- Submeters
- Individual meters
- Smart meters
- Meter readings
- Actual consumption
- Estimated consumption
- Utility rates
- Utility taxes
- Utility fees
- Utility reimbursement
- Shared utility allocation
- Utility forecasting
- Utility cost analysis
- Consumption analysis
- Utility anomaly detection
- Leak detection
- Unmetered loss analysis

### Accounting

The Accounting module provides a complete campground accounting framework.

Features include:

- General ledger
- Chart of accounts
- Accounts payable
- Accounts receivable
- Cash management
- Bank reconciliation
- Journal entries
- Accrual accounting
- Cash accounting
- Revenue recognition
- Expense recognition
- Deferred revenue
- Deposits
- Refunds
- Credits
- Adjustments
- Owner balances
- Vendor balances
- Asset accounting
- Liability accounting
- Equity accounting
- Inter-account transfers

Operational transactions should be capable of generating corresponding accounting entries.

### Revenue Management

The Revenue Management module tracks all campground revenue sources.

Supported revenue includes:

- Campsite revenue
- Reservation revenue
- Seasonal revenue
- Monthly revenue
- Annual revenue
- Cabin revenue
- RV rental revenue
- Equipment rental revenue
- Storage revenue
- Laundry revenue
- Recreation revenue
- Event revenue
- Internet revenue
- Utility reimbursement
- Maintenance charges
- Community fees
- Administrative fees
- Cancellation fees
- Late fees
- Other campground revenue

### Expense Management

The Expense Management module tracks the complete cost of campground operations.

Supported expenses include:

- Operating expenses
- Maintenance expenses
- Labor
- Utilities
- Insurance
- Property taxes
- Vendor expenses
- Supplies
- Cleaning
- Landscaping
- Pool maintenance
- Trash removal
- Security
- Repairs
- Equipment
- Fuel
- Administrative expenses
- Technology
- Marketing
- Professional services
- Capital expenditures

Expenses must support attribution to the campground, property, facility, site, unit, rental, owner, department, service, project, or other applicable cost center.

### Owner Accounting

The Owner Accounting module provides individual financial records for private owners.

Owner records should support:

- Community fees
- Site fees
- Utility charges
- Maintenance charges
- Shared service charges
- Special assessments
- Administrative fees
- Payments
- Credits
- Refunds
- Current balances
- Past-due balances
- Payment history
- Supporting documentation

Owners should be able to receive statements showing how shared expenses were calculated.

### Invoice Management

The Invoice Management module supports financial document processing.

Features include:

- Vendor invoices
- Owner invoices
- Customer invoices
- Recurring invoices
- Invoice approvals
- Purchase order matching
- Invoice classification
- Expense classification
- Duplicate invoice detection
- Invoice allocation
- Payment tracking
- Credit tracking
- Invoice history

### Vendor Management

The Vendor Management module manages vendors and service providers.

Features include:

- Vendor profiles
- Vendor contacts
- Vendor contracts
- Service agreements
- Insurance documentation
- Licenses
- W-9 information
- Payment terms
- Vendor pricing
- Vendor history
- Vendor performance
- Contract expiration
- Vendor spending analysis

### Procurement

The Procurement module manages purchases from request through payment.

Features include:

- Purchase requests
- Purchase approvals
- Purchase orders
- Vendor quotes
- Competitive pricing
- Recurring purchases
- Emergency purchases
- Capital purchases
- Inventory purchases
- Receipt tracking
- Invoice matching
- Procurement history

### Inventory Management

The Inventory Management module tracks campground supplies, maintenance materials, and consumables.

Supported inventory includes:

- Maintenance parts
- Plumbing supplies
- Electrical supplies
- Cleaning supplies
- Pool chemicals
- Landscaping supplies
- Office supplies
- Replacement equipment
- Consumables

Features include:

- Inventory counts
- Inventory valuation
- Minimum stock levels
- Reorder points
- Vendor pricing
- Inventory usage
- Inventory allocation
- Inventory shrinkage detection

### Labor Management

The Labor Management module tracks the complete cost of campground labor.

Features include:

- Employee records
- Departments
- Scheduling
- Time tracking
- Work order labor
- Project labor
- Facility labor
- Site labor
- Maintenance labor
- Administrative labor
- Overtime
- Employer costs
- Benefits
- Contractor labor
- Temporary labor

Labor costs should support allocation to the service, asset, site, owner, rental, project, department, or facility that generated the cost.

### Capital Planning

The Capital Planning module manages major campground investments and infrastructure projects.

Features include:

- Capital projects
- Project budgets
- Project expenses
- Labor
- Materials
- Contractors
- Permits
- Funding
- Project timelines
- Asset creation
- Capitalization
- Depreciation
- Project completion
- Project cost tracking

### Asset Replacement Planning

The Asset Replacement Planning module forecasts future infrastructure and asset requirements.

Features include:

- Asset lifecycle analysis
- Remaining useful life
- Replacement forecasting
- Replacement cost estimates
- Reserve planning
- Capital funding requirements
- Infrastructure risk
- Deferred maintenance analysis

### Budgeting

The Budgeting module supports financial planning across the campground.

Budgets can be created for:

- Campground operations
- Departments
- Facilities
- Sites
- Rentals
- Maintenance
- Utilities
- Labor
- Capital projects
- Services

Features include:

- Annual budgets
- Monthly budgets
- Seasonal budgets
- Department budgets
- Facility budgets
- Site budgets
- Rental budgets
- Maintenance budgets
- Utility budgets
- Labor budgets
- Capital budgets
- Project budgets
- Budget variance analysis

### Financial Forecasting

The Financial Forecasting module provides forward-looking financial analysis.

Features include:

- Revenue forecasting
- Expense forecasting
- Cash-flow forecasting
- Occupancy forecasting
- Maintenance forecasting
- Utility forecasting
- Labor forecasting
- Capital expenditure forecasting
- Vendor cost forecasting
- Scenario modeling
- Budget forecasting

### Financial Optimization

The Financial Optimization module analyzes campground operations for opportunities to improve financial performance.

Features include:

- Expense reduction analysis
- Vendor cost analysis
- Service cost analysis
- Facility profitability
- Rental profitability
- Site profitability
- Utility optimization
- Labor optimization
- Inventory optimization
- Maintenance optimization
- Revenue optimization
- Shared-cost optimization
- Underutilization detection
- Cost anomaly detection

### Shared Expense Optimization

The Shared Expense Optimization module compares allocation methods to identify an appropriate distribution of common expenses.

The system may compare:

- Equal allocation
- Per-site allocation
- Per-unit allocation
- Occupancy allocation
- Usage allocation
- Revenue allocation
- Ownership allocation
- Hybrid allocation

Optimization should consider:

- Actual usage
- Cost causation
- Contractual obligations
- Community agreements
- Historical patterns
- Regulatory requirements
- Administrative complexity
- Transparency
- Predictability

### Tax Management

The Tax Management module provides configurable tax calculation and reporting infrastructure.

Supported tax categories may include:

- Federal tax data
- State tax data
- Local tax data
- Sales tax
- Lodging tax
- Occupancy tax
- Tourism tax
- Property tax
- Payroll tax
- Tax-exempt transactions
- Taxable revenue
- Taxable expenses
- Tax liabilities
- Tax collections

The tax engine should be configurable by jurisdiction rather than permanently tied to a single jurisdiction.

### Tax Reporting

The Tax Reporting module provides structured tax reporting data.

Features include:

- Tax summaries
- Tax liability reports
- Filing reports
- Transaction-level tax records
- Supporting schedules
- Tax exports
- Audit documentation
- Historical tax records
- Tax-period controls
- Tax adjustment tracking

CampGrid provides tax management infrastructure and reporting capabilities but does not replace qualified tax, legal, or accounting professionals where professional review is required.

### Reporting and Analytics

The Reporting and Analytics module provides operational, financial, ownership, maintenance, and community reporting.

Management reports include:

- Daily operations
- Occupancy
- Revenue
- Expenses
- Profitability
- Cash flow
- Maintenance
- Utilities
- Labor
- Inventory
- Vendor spending
- Capital projects

Owner reports include:

- Owner statements
- Site charges
- Maintenance charges
- Utility charges
- Community charges
- Shared expense allocations
- Special assessments
- Payment history
- Outstanding balances
- Supporting expense documentation

Accounting reports include:

- General ledger
- Trial balance
- Profit and loss
- Balance sheet
- Cash flow
- Accounts payable
- Accounts receivable
- Aging reports
- Revenue reports
- Expense reports
- Asset reports

Operational analytics include:

- Revenue per site
- Revenue per occupied night
- Cost per site
- Maintenance cost per asset
- Utility cost per site
- Labor cost per service
- Rental profitability
- Facility profitability
- Vendor cost trends
- Occupancy trends
- Expense trends
- Community service costs

### Audit and Financial Provenance

The Audit and Financial Provenance module maintains a complete history of financial and operational changes.

Records should include:

- User identification
- Timestamp
- Original value
- Revised value
- Change reason
- Approval history
- Source document
- Allocation calculation
- Accounting entries
- Payment history
- Tax history

Financial records should not be silently overwritten or removed.

### Document Management

The Document Management module associates documents with campground records.

Supported documents include:

- Rental agreements
- Owner agreements
- Site agreements
- Community rules
- Vendor contracts
- Insurance certificates
- Permits
- Licenses
- Inspection reports
- Maintenance records
- Invoices
- Receipts
- Tax documentation
- Financial records

Documents should be associable with:

**Person → Site → Unit → Asset → Contract → Expense → Payment**

### Security and Permissions

The Security and Permissions module provides configurable access control.

Supported roles include:

- Owners
- Operators
- General managers
- Property managers
- Accountants
- Reservation staff
- Maintenance staff
- Employees
- Vendors
- Private owners
- Residents
- Auditors

Permissions should be configurable at multiple levels:

**System → Property → Facility → Site → Unit → Financial Record**

Security features include:

- Authentication
- Role-based authorization
- Permission management
- Audit logging
- Data encryption
- Secure backups
- Session management
- API authentication
- Sensitive financial data protection

### API and Integration

The API and Integration module provides vendor-neutral interfaces for external systems.

Potential integrations include:

- Payment processors
- Banking systems
- Accounting systems
- Tax systems
- Reservation systems
- Payroll systems
- Smart meters
- Gate systems
- Access-control systems
- IoT devices
- Property-management systems
- Mapping systems
- Email
- SMS

CampGrid should not require a specific vendor to implement the specification.

### Local-First Operation

CampGrid is designed to support local-first campground management.

Capabilities include:

- Self-hosted deployment
- Local databases
- Local network operation
- Offline operation
- Local backups
- Disaster recovery
- Optional cloud synchronization
- Multi-property synchronization
- Data ownership
- Open data export

### Data Portability

CampGrid implementations should provide mechanisms to export operational and financial data.

Exportable information includes:

- Sites
- Units
- Owners
- Guests
- Reservations
- Assets
- Maintenance
- Work orders
- Vendors
- Invoices
- Payments
- Accounting records
- Tax records
- Expense allocations
- Audit records
- Documents

CampGrid is designed to prevent vendor lock-in and preserve campground control over its data.

### Multi-Property Management

The Multi-Property Management module supports operators managing multiple campground properties.

Features include:

- Multiple campgrounds
- Regional management
- Corporate management
- Consolidated accounting
- Property-level accounting
- Property-level reporting
- Shared vendors
- Central procurement
- Inter-property transfers
- Cross-property benchmarking
- Consolidated budgeting

## Optional Plugin Modules

CampGrid's core modules provide the foundational campground management specification. Optional plugins extend the system for specialized operations without requiring those capabilities in every implementation.

### Online Booking Plugin

Provides advanced public-facing booking capabilities.

Features may include:

- Public booking websites
- Online availability
- Online payments
- Guest accounts
- Reservation modifications
- Automated confirmations
- Automated reminders
- Cancellation workflows
- Promotional codes
- Dynamic pricing

### Point of Sale Plugin

Supports campground retail and service transactions.

Potential uses include:

- Camp stores
- Restaurants
- Snack bars
- Laundry
- Recreation
- Equipment rentals
- Firewood
- Propane
- Merchandise
- Guest services

### Smart Meter Plugin

Connects utility meters to CampGrid.

Features may include:

- Automated meter readings
- Real-time consumption
- Utility alerts
- Usage thresholds
- Anomaly detection
- Automated owner billing
- Automated utility allocation

### Gate and Access Control Plugin

Supports campground access systems.

Features may include:

- Gate access
- Digital credentials
- Vehicle access
- Guest access
- Owner access
- Staff access
- Temporary access
- Access logs
- Automated expiration

### Security Systems Plugin

Integrates campground security infrastructure.

Potential integrations include:

- Cameras
- Security sensors
- Emergency systems
- Access systems
- Perimeter monitoring
- Incident records

### Payroll Plugin

Provides deeper payroll integration.

Features may include:

- Payroll processing
- Time records
- Overtime
- Employer taxes
- Benefits
- Labor allocation
- Payroll reporting

### Advanced Tax Filing Plugin

Extends the core tax engine with jurisdiction-specific filing integrations.

Features may include:

- Electronic filing
- Filing calendars
- Automated filing preparation
- Jurisdiction-specific reports
- Tax payment tracking
- Filing confirmations

### AI Optimization Plugin

Provides advanced AI-assisted analysis.

Features may include:

- Predictive maintenance
- Revenue forecasting
- Occupancy forecasting
- Expense forecasting
- Vendor optimization
- Utility optimization
- Staffing analysis
- Inventory forecasting
- Shared expense optimization
- Financial anomaly detection
- Scenario modeling

AI-generated recommendations should remain subject to configurable human approval.

### Utility Management Plugin

Provides advanced utility infrastructure management.

Potential capabilities include:

- Utility networks
- Utility meters
- Water systems
- Sewer systems
- Electrical systems
- Pump systems
- Solar systems
- Energy storage
- Automated consumption monitoring

### Fleet Management Plugin

Manages campground vehicles and mobile equipment.

Features may include:

- Vehicle records
- Maintenance
- Fuel
- Mileage
- Insurance
- Registration
- Driver assignments
- Replacement planning
- Operating cost analysis

### Marina Management Plugin

Extends CampGrid to campground properties with marina operations.

Features may include:

- Boat slips
- Dock management
- Boat storage
- Slip reservations
- Utility allocation
- Maintenance
- Owner management
- Marina fees

### Horse Facility Plugin

Supports campgrounds that include equestrian facilities.

Potential capabilities include:

- Stalls
- Paddocks
- Boarding
- Feed
- Maintenance
- Facility reservations
- Owner accounts
- Animal records
- Service charges

### Event Management Plugin

Supports campground events and activities.

Features may include:

- Event scheduling
- Facility reservations
- Event registration
- Event fees
- Staff
- Supplies
- Vendors
- Revenue
- Expenses
- Event profitability

### Laundry Management Plugin

Supports campground laundry operations.

Features may include:

- Machines
- Machine availability
- Maintenance
- Usage
- Revenue
- Utilities
- Supplies
- Cost analysis

### Camp Store Plugin

Supports campground retail operations.

Features may include:

- Products
- Inventory
- Vendors
- Purchasing
- Point of sale
- Pricing
- Taxes
- Sales
- Profitability

### Restaurant and Food Service Plugin

Supports campground food service operations.

Potential capabilities include:

- Menus
- Recipes
- Ingredients
- Inventory
- Vendors
- Point of sale
- Labor
- Food costs
- Taxes
- Revenue
- Profitability

### Golf Cart Rental Plugin

Supports campground golf cart operations.

Features may include:

- Golf cart inventory
- Reservations
- Rental agreements
- Deposits
- Maintenance
- Charging
- Damage records
- Revenue
- Expenses
- Profitability

### Equipment Rental Plugin

Supports rental of campground equipment.

Potential assets include:

- Bicycles
- Kayaks
- Canoes
- Paddleboards
- Trailers
- Recreation equipment
- Tools
- Other rental equipment

### Long-Term Housing Plugin

Extends CampGrid for campground communities containing longer-term residential arrangements.

Features may include:

- Long-term occupancy
- Housing units
- Resident records
- Recurring charges
- Utilities
- Maintenance
- Community services
- Owner accounting

### Property Owner Portal Plugin

Provides private owners with direct access to their campground records.

Features may include:

- Owner statements
- Payments
- Maintenance requests
- Expense allocations
- Community charges
- Documents
- Notices
- Service history
- Unit information

### Resident Portal Plugin

Provides residents and long-term occupants with access to campground services.

Features may include:

- Account management
- Payments
- Reservations
- Maintenance requests
- Community notices
- Service requests
- Documents
- Community information

## Economic Model

CampGrid is designed around the principle that campground operations should be economically traceable from the physical resource to the financial record.

A campground service may follow this chain:

**Asset → Service → Maintenance → Expense → Allocation → Charge → Payment → Accounting → Tax Reporting**

A privately owned unit may follow:

**Owner → Unit → Site → Utilities → Community Services → Maintenance → Charges → Payment → Owner Statement → Accounting**

A rental unit may follow:

**Rental Unit → Reservation → Revenue → Tax → Cleaning → Utilities → Maintenance → Supplies → Depreciation → Profitability**

This interconnected model allows operators to understand the true cost and financial performance of every part of the campground.

## Financial Transparency Principle

CampGrid should make it possible to determine:

> **What does every part of the campground cost, who benefits from it, who is responsible for it, and how should that cost be accounted for?**

Shared expenses should never become unexplained charges.

Every charge should be traceable to its source, allocation method, and accounting record.

## Optimization Principle

CampGrid should not merely record campground activity.

It should provide the information necessary to improve campground operations.

The system should support analysis of:

- Cost
- Revenue
- Profitability
- Occupancy
- Maintenance
- Utilities
- Labor
- Inventory
- Vendors
- Capital requirements
- Shared expenses
- Community services
- Asset lifecycle
- Future financial requirements

The objective is to help campground operators understand the campground as a complete economic and physical system.

## Modularity Principle

Each core module should have defined interfaces and responsibilities so that implementations can:

- Deploy modules independently where appropriate
- Extend modules
- Replace implementations
- Integrate external systems
- Add plugins
- Remove optional capabilities
- Synchronize selected data
- Maintain interoperability

Core functionality should not depend on optional plugins unless explicitly defined by an implementation.

## Human Governance Principle

CampGrid may use automation and artificial intelligence to analyze campground operations, but financial and operational authority should remain configurable and subject to human governance.

Implementations should support approval workflows for:

- Financial adjustments
- Expense allocations
- Vendor changes
- Tax classifications
- Accounting changes
- Budget changes
- Capital expenditures
- Owner charges
- Community assessments
- AI-generated recommendations

## Implementation Neutrality

CampGrid is a specification rather than a requirement to use a particular software stack, database, cloud provider, payment processor, accounting platform, reservation provider, or hardware vendor.

Implementations may use different technologies while remaining compatible with the CampGrid specification.

## Open Source and Data Independence

CampGrid is designed to encourage an ecosystem of interoperable campground management implementations.

The specification prioritizes:

- Open source software
- Self-hosting
- Local-first infrastructure
- Vendor neutrality
- Open interfaces
- Data portability
- Transparent financial records
- Extensible modules
- Community-driven development

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
  - [https://roxanneardary.com/campgrid/](https://roxanneardary.com/campgrid/)  

---

## License & Notice Requirements

CampGrid is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- CampGrid specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

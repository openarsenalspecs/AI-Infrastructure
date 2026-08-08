# HelixERP

**Self-Hosted. Community-Driven. Enterprise-Ready.**

HelixERP is a fast, modular, self-hosted, open-source Enterprise Resource Planning (ERP) platform designed to provide businesses with complete control over their operations, data, and infrastructure.

HelixERP is designed as an alternative to traditional monolithic ERP platforms. Its modular architecture allows organizations to deploy the functionality they need while maintaining a unified data model, consistent security framework, shared workflows, and seamless communication between modules.

The platform is built for performance, scalability, extensibility, and long-term maintainability, with support for everything from small self-hosted deployments to complex enterprise environments.

---

## Project Goals

HelixERP is designed around several core principles:

- **Self-hosted** — Organizations maintain control over their infrastructure and data.
- **Open source** — The platform is developed transparently under the AGPL-3.0+ license.
- **Modular** — Business capabilities are organized into independently maintainable modules.
- **Fast** — Performance is treated as a core architectural requirement.
- **Scalable** — Deployments can scale vertically or horizontally as requirements grow.
- **Extensible** — Organizations and developers can build plugins without modifying the core platform.
- **Secure** — Granular permissions, auditing, authentication, and data protection are built into the platform.
- **API-first** — Core functionality is accessible through standardized APIs.
- **Interoperable** — HelixERP is designed to integrate with external business systems and services.
- **Human-controlled** — Automation and AI assist users without removing human oversight from important business decisions.

---

# Specification

HelixERP uses a modular ERP architecture consisting of a **Core Platform**, **Core Business Modules**, and **Optional Plugin Modules**.

The Core Platform provides the infrastructure shared by the entire system. Core Business Modules provide the primary ERP functionality required to operate an organization. Optional Plugin Modules extend the platform with additional capabilities, integrations, industry-specific functionality, and specialized services.

Modules communicate through standardized APIs, events, services, and the shared HelixERP data model rather than creating isolated systems.

---

# Core Platform

The Core Platform provides the foundation upon which all HelixERP modules operate.

### Identity & Access

- User accounts
- Organizations and companies
- Roles and permissions
- Module-level permissions
- Record-level permissions
- Field-level permissions
- Authentication
- Two-factor authentication
- Single sign-on support
- Session management
- API authentication
- Service accounts
- Access policies

### Security & Compliance

- Security policies
- Audit logging
- Authentication logging
- Administrative activity tracking
- Data access tracking
- Sensitive-data protection
- Encryption support
- Security event monitoring
- Data retention controls
- Privacy controls
- Compliance-ready architecture

### Configuration

- System settings
- Company settings
- Module configuration
- User preferences
- Localization
- Currency configuration
- Tax configuration
- Numbering sequences
- Custom fields
- Custom metadata
- Feature configuration

### Workflow Engine

- Workflow definitions
- Business rules
- Approval chains
- Conditional logic
- Automated actions
- Scheduled actions
- Event-triggered workflows
- Notifications
- Escalations
- Human approval steps

### Event Bus & Service Layer

- Internal event bus
- Module-to-module events
- Background services
- Service discovery
- Event subscriptions
- Event queues
- Asynchronous processing
- Webhooks
- External event integrations

### Document & File Management

- Document storage
- File attachments
- Document metadata
- Document versioning
- Document permissions
- Document relationships
- Document search
- Document retention policies

### Notifications

- In-app notifications
- Email notifications
- System alerts
- Workflow notifications
- User notifications
- Administrative alerts
- Notification preferences

### API Platform

- REST API
- GraphQL API
- Webhooks
- API authentication
- API permissions
- API versioning
- Integration endpoints
- Import/export services
- Developer documentation

### Search

- Global search
- Module-specific search
- Full-text search
- Advanced filtering
- Saved searches
- Search permissions
- Indexed business records

### Reporting Foundation

- Report engine
- Report permissions
- Report scheduling
- Export services
- Dashboard framework
- Data aggregation
- Saved reports
- Custom report definitions

---

# Core Business Modules

Core modules provide the primary enterprise functionality of HelixERP.

## Finance & Accounting

The Finance & Accounting module provides the financial foundation of the organization.

- General Ledger
- Chart of Accounts
- Accounts Payable
- Accounts Receivable
- Customer invoicing
- Vendor billing
- Payments
- Receipts
- Bank accounts
- Bank reconciliation
- Journal entries
- Recurring transactions
- Expense management
- Financial periods
- Budgeting
- Financial forecasting
- Multi-company accounting
- Consolidated accounting
- Multi-currency accounting
- Tax management
- Financial reporting
- Cash-flow management
- Financial audit trails

---

## Sales & CRM

The Sales & CRM module manages customer relationships and the complete sales lifecycle.

- Leads
- Prospects
- Contacts
- Organizations
- Opportunities
- Sales pipelines
- Sales stages
- Activities
- Tasks
- Calls
- Meetings
- Customer communications
- Quotations
- Sales orders
- Customer history
- Sales forecasting
- Territory management
- Sales teams
- Commission management
- Customer segmentation
- Customer lifecycle management

---

## Procurement

The Procurement module manages purchasing and supplier relationships.

- Vendors
- Vendor records
- Purchase requests
- Purchase requisitions
- Requests for quotation
- Vendor quotations
- Purchase orders
- Purchase approvals
- Purchase receipts
- Vendor invoices
- Vendor performance
- Supplier catalogs
- Procurement workflows
- Purchase analytics
- Spend analysis

---

## Inventory & Warehouse

The Inventory & Warehouse module manages physical products, stock, and warehouse operations.

- Products
- Product variants
- Product categories
- Units of measure
- Warehouses
- Storage locations
- Inventory balances
- Stock movements
- Stock transfers
- Inventory adjustments
- Receiving
- Picking
- Packing
- Shipping
- Batch tracking
- Lot tracking
- Serial number tracking
- Inventory valuation
- Reorder points
- Replenishment
- Inventory forecasting
- Warehouse operations
- Stock auditing

---

## Supply Chain

The Supply Chain module connects procurement, inventory, sales, and fulfillment.

- Supply planning
- Demand planning
- Replenishment planning
- Supplier management
- Lead-time tracking
- Purchase planning
- Inventory forecasting
- Supply-chain analytics
- Fulfillment planning
- Order allocation
- Shipment planning
- Supply-chain alerts

---

## Human Resources

The Human Resources module manages employee information and organizational processes.

- Employee records
- Departments
- Positions
- Organizational structure
- Employee onboarding
- Employee offboarding
- Leave management
- Attendance
- Time tracking
- Employee documents
- Performance management
- Skills tracking
- Training records
- Benefits management
- HR workflows
- Employee self-service

---

## Payroll

The Payroll module manages payroll processing and payroll-related records.

- Payroll profiles
- Pay schedules
- Earnings
- Deductions
- Benefits
- Taxes
- Payroll calculations
- Payroll periods
- Payroll approvals
- Payroll reporting
- Payroll history
- Employee payroll records

Payroll functionality can be configured for different jurisdictions through extensible tax and payroll rules.

---

## Projects & Services

The Projects & Services module manages projects, tasks, resources, and service delivery.

- Projects
- Tasks
- Subtasks
- Milestones
- Dependencies
- Gantt planning
- Kanban workflows
- Project teams
- Time tracking
- Resource allocation
- Project budgets
- Project costs
- Project profitability
- Client projects
- Service engagements
- Project billing
- Project reporting

---

## Manufacturing

The Manufacturing module manages production operations.

- Bill of materials
- Manufacturing orders
- Work orders
- Work centers
- Production planning
- Production scheduling
- Material requirements
- Production consumption
- Finished goods
- Production costs
- Quality checkpoints
- Manufacturing workflows
- Production analytics
- Capacity planning

---

## Order Management

The Order Management module provides a unified lifecycle for customer orders.

- Quotes
- Sales orders
- Order approvals
- Order fulfillment
- Order allocation
- Backorders
- Returns
- Refunds
- Order status tracking
- Order history
- Customer order portals
- Order analytics

---

## E-Commerce

The E-Commerce module provides native commerce capabilities and integration with external storefronts.

- Product catalogs
- Online orders
- Shopping carts
- Customer accounts
- Pricing
- Promotions
- Discounts
- Inventory synchronization
- Order synchronization
- Payment integration
- Shipping integration
- Store management
- Commerce analytics

---

## Assets & Maintenance

The Assets & Maintenance module manages organizational assets and maintenance operations.

- Asset registry
- Asset ownership
- Asset locations
- Asset depreciation
- Asset lifecycle tracking
- Maintenance schedules
- Preventive maintenance
- Maintenance requests
- Maintenance work orders
- Maintenance history
- Asset costs
- Asset reporting

---

## Service Management

The Service Management module manages customer and internal service operations.

- Service requests
- Tickets
- Case management
- Service queues
- Service-level agreements
- Escalations
- Service assignments
- Customer service history
- Knowledge resources
- Service analytics

---

## Reporting & Business Intelligence

The Reporting & Business Intelligence module provides organization-wide analysis.

- Financial dashboards
- Sales dashboards
- Inventory dashboards
- HR dashboards
- Project dashboards
- Operations dashboards
- Custom dashboards
- Custom reports
- KPI tracking
- Trend analysis
- Drill-down reporting
- Scheduled reports
- Data exports
- Cross-module analytics
- Executive dashboards

---

## AI & Intelligent Automation

The AI module provides optional intelligent capabilities while maintaining human oversight.

- Financial insights
- Cash-flow forecasting
- Demand forecasting
- Inventory forecasting
- Sales forecasting
- Expense categorization
- Anomaly detection
- Workflow recommendations
- Resource optimization
- Document extraction
- Natural-language search
- Natural-language reporting
- Business intelligence assistance
- Predictive maintenance
- Operational recommendations

AI-generated recommendations should remain reviewable and configurable by authorized users.

---

# Optional Plugin Modules

HelixERP supports an extensible plugin architecture for functionality that is useful to specific organizations but should not be required by every installation.

Plugins can add functionality without requiring modifications to the HelixERP Core Platform.

### Communications Plugin

- Email management
- Email campaigns
- SMS
- Messaging integrations
- Notification providers
- Communication templates

### Marketing Plugin

- Marketing campaigns
- Lead campaigns
- Customer segmentation
- Marketing automation
- Campaign analytics
- Landing-page integration

### Help Desk Plugin

- Advanced ticketing
- Customer support portals
- Knowledge bases
- SLA management
- Support analytics
- Automated support workflows

### Advanced BI Plugin

- Advanced data visualization
- Data warehousing
- OLAP-style analysis
- Advanced forecasting
- Custom analytical models
- Executive intelligence dashboards

### Payment Gateway Plugins

Support for external payment providers through independently maintained integrations.

- Payment processing
- Payment reconciliation
- Refund processing
- Recurring payments
- Payment webhooks

### E-Commerce Connector Plugins

Connect HelixERP with external commerce platforms.

- Store synchronization
- Product synchronization
- Inventory synchronization
- Customer synchronization
- Order synchronization
- Fulfillment synchronization

### Banking Connector Plugins

- Bank feeds
- Transaction synchronization
- Automated reconciliation
- Payment initiation
- Banking alerts

### Shipping & Logistics Plugins

- Carrier integrations
- Shipping rates
- Label generation
- Shipment tracking
- Delivery notifications
- Logistics analytics

### Document Intelligence Plugin

- OCR
- Invoice extraction
- Receipt extraction
- Document classification
- Contract extraction
- Automated data entry

### Advanced AI Plugin

- Local AI models
- External AI providers
- AI agents
- AI workflow assistants
- Advanced forecasting
- Custom business models
- Natural-language business operations

### Industry Plugin Framework

Organizations and developers can create specialized plugins for industries such as:

- Construction
- Healthcare
- Hospitality
- Manufacturing
- Distribution
- Professional services
- Real estate
- Nonprofits
- Education
- Retail

---

# Plugin Architecture

Plugins should integrate with HelixERP through documented extension points rather than modifying core functionality.

Plugins may provide:

- New modules
- New database entities
- New workflows
- New API endpoints
- New dashboard components
- New reports
- New integrations
- New automation rules
- New user interfaces
- New event handlers

Plugins should be independently installable, configurable, updateable, and removable wherever practical.

---

# Performance Architecture

Performance is a fundamental design requirement of HelixERP.

The platform is designed to support:

- Asynchronous background processing
- Job queues
- Intelligent caching
- Database indexing
- Query optimization
- Database partitioning
- Lazy loading
- Frontend code splitting
- API response optimization
- Event-driven processing
- Horizontal scaling
- Service isolation
- Background report generation
- Large-volume imports and exports

Heavy operations should not unnecessarily block interactive user workflows.

---

# Security Architecture

Security is built into the platform rather than added as an afterthought.

HelixERP supports:

- Role-based access control
- Record-level permissions
- Field-level permissions
- Two-factor authentication
- Single sign-on
- API authentication
- Audit trails
- Security event logging
- Encryption support
- Secure session management
- Data access controls
- Administrative activity tracking
- Backup and recovery strategies
- Configurable data retention

---

# Multi-Company & Multi-Organization Support

HelixERP is designed to support organizations operating multiple companies, subsidiaries, divisions, or business units.

Capabilities include:

- Multiple companies
- Company-specific settings
- Company-specific users
- Company-specific accounting
- Intercompany transactions
- Consolidated reporting
- Shared or isolated catalogs
- Cross-company permissions
- Company-specific workflows

---

# Localization

HelixERP is designed for international deployments.

Localization capabilities include:

- Multiple languages
- Multiple currencies
- Regional date formats
- Regional number formats
- Time zones
- Tax rules
- Localization plugins
- Regional accounting requirements
- Localized documents

---

# Data Import & Export

HelixERP provides tools for moving business data into and out of the platform.

Supported capabilities include:

- CSV imports
- CSV exports
- Spreadsheet-compatible exports
- API imports
- API exports
- Bulk operations
- Data validation
- Import previews
- Import error reporting
- Scheduled exports

---

# Deployment

HelixERP is designed primarily for self-hosted deployment.

Supported deployment models can include:

- Single-server installations
- Docker deployments
- Containerized deployments
- Private infrastructure
- Virtual machines
- On-premises servers
- Cloud-hosted infrastructure controlled by the organization
- High-availability deployments
- Horizontally scaled deployments

The architecture should allow smaller organizations to run HelixERP with a relatively simple deployment while providing a path toward larger distributed installations.

---

# Developer Experience

HelixERP is designed to make development and customization accessible.

The project provides:

- Documented APIs
- Modular source structure
- Extension points
- Plugin architecture
- Database migration system
- Testing framework
- Developer documentation
- API documentation
- Module documentation
- Contribution guidelines
- Development workflow documentation

---

# Community Development

HelixERP is designed as a community-driven project.

Contributors can participate through:

- Core development
- Module development
- Plugin development
- Bug fixes
- Security improvements
- Performance improvements
- Documentation
- Testing
- Translations
- Integrations
- UI/UX improvements

Community-developed functionality should favor reusable modules and plugins over modifications that unnecessarily increase core complexity.

---

# Vision

HelixERP aims to provide an open alternative to proprietary enterprise software by combining the breadth expected from a modern ERP platform with a faster, more modular, transparent, and self-hosted architecture.

**HelixERP — Self-Hosted. Community-Driven. Enterprise-Ready.**

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
  - [https://roxanneardary.com/helixerp/](https://roxanneardary.com/helixerp/)

---

## License & Notice Requirements

HelixERP is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- HelixERP specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

# FoodMesh

**Building a shared network for resilient food systems.**

FoodMesh is an open-source, modular logistics specification designed to connect small farmers, independent trucking operators, distributors, and communities through a shared transportation network.

The specification provides the foundation for decentralized agricultural logistics by enabling transparent load tracking, multi-farm shipment coordination, GPS verification, weight tracking, smart routing, and private transaction records.

FoodMesh helps create a more resilient food supply network by allowing regional producers to efficiently move products to markets without requiring dependence on centralized logistics platforms.

---

# Overview

Modern agricultural transportation systems are optimized for large-scale producers, leaving many small farms without affordable access to regional and national markets. FoodMesh introduces a distributed logistics model where multiple farms can contribute partial loads, independent carriers can optimize routes, and buyers can receive verified delivery information.

The system is designed around private transactions between participants while maintaining transparent records of shipment movement, ownership, and delivery verification.

FoodMesh provides:

- Farm-to-market transportation coordination
- Multi-source shipment consolidation
- Load documentation and verification
- Truck-aware routing
- GPS-based transportation tracking
- Digital weight verification
- Mileage and fleet tracking
- Private transaction management
- Open API interoperability

---

# Design Goals

FoodMesh is designed with the following principles:

- **Open Infrastructure**  
  Provide a reusable specification that organizations and communities can build upon.

- **Modular Architecture**  
  Allow individual components to be deployed independently or combined into a complete logistics platform.

- **Private Transactions**  
  Enable direct business relationships between farmers, carriers, distributors, and buyers.

- **Transparent Verification**  
  Provide trustworthy shipment records without requiring centralized control.

- **Interoperability**  
  Support integration with existing farm, transportation, inventory, and payment systems.

- **Community Resilience**  
  Strengthen regional food networks by improving access to transportation.

---

# Core Modules

## Participant Identity Module

Manages participants within the FoodMesh network.

Features:

- Farmer profiles
- Carrier profiles
- Driver accounts
- Buyer profiles
- Equipment records
- Permissions management
- Digital identity verification
- Organization management

---

## Load Management Module

Creates and manages agricultural shipment records.

Features:

- Product descriptions
- Load creation
- Farm origin records
- Quantity tracking
- Packaging details
- Shipment ownership records
- Load status updates
- Digital shipment documentation

---

## Multi-Farm Consolidation Module

Enables multiple farms to share transportation capacity.

Features:

- Partial load management
- Multi-stop pickup planning
- Capacity calculations
- Load grouping
- Individual producer tracking
- Route coordination

---

## Load Documentation Module

Provides digital proof of shipment condition.

Features:

- Pickup photographs
- Delivery photographs
- Timestamp records
- Location metadata
- Product condition reports
- Digital signatures

---

## Weight Verification Module

Tracks shipment weight throughout transportation.

Features:

- Farm scale integration
- Portable scale support
- Vehicle scale integration
- Pickup weight recording
- Delivery weight recording
- Weight discrepancy reporting
- Loss calculations

---

## GPS Tracking Module

Provides real-time shipment visibility.

Features:

- Pickup location recording
- Delivery location recording
- Live vehicle tracking
- Route history
- Estimated arrival times
- Location verification

---

## Truck Routing Module

Provides transportation routing optimized for commercial vehicles.

Features:

- Truck size restrictions
- Height clearance warnings
- Weight restrictions
- Bridge limitations
- Trailer length compatibility
- Delivery location suitability checks
- Commercial vehicle routing

---

## Fuel Optimization Module

Provides fuel-efficient route planning.

Features:

- Fuel-saving routes
- Idle reduction tracking
- Fuel consumption analysis
- Cost calculations
- Vehicle efficiency reporting

---

## Toll Optimization Module

Provides independent toll management options.

Features:

- Lowest toll routes
- Toll avoidance routes
- Cost comparisons
- Route preference selection

---

## Mileage & Fleet Module

Tracks vehicle operations.

Features:

- Mileage tracking
- Fuel records
- Maintenance schedules
- Inspection records
- Vehicle history
- Fleet reporting

---

## Delivery Verification Module

Completes shipment transactions.

Features:

- Delivery confirmation
- Receiver signatures
- Final photographs
- Final weight verification
- Shipment completion records

---

## Blockchain Verification Module

Provides optional cryptographic verification.

Features:

- Bitcoin timestamp verification
- OpenTimestamps support
- Proof-of-record verification
- Tamper-resistant shipment records
- Lightning Network payment integration

Private shipment information remains controlled by participants while verification records can prove that events occurred.

---

# Optional Plugin Modules

FoodMesh supports optional extensions that can be added based on deployment requirements.

---

## AI Route Intelligence Plugin

Provides intelligent transportation optimization.

Features:

- Predictive routing
- Traffic analysis
- Weather-aware routing
- Delivery prediction
- Fuel optimization recommendations

---

## AI Load Matching Plugin

Matches available transportation capacity with available shipments.

Features:

- Farm shipment matching
- Truck capacity matching
- Regional demand analysis
- Route efficiency recommendations

---

## Predictive Maintenance Plugin

Uses vehicle data to predict maintenance needs.

Features:

- Mechanical trend analysis
- Service reminders
- Failure prediction
- Maintenance scheduling

---

## Marketplace Plugin

Creates private agricultural logistics marketplaces.

Features:

- Shipment listings
- Carrier availability
- Private bidding
- Contract management
- Transaction history

---

## Payment & Settlement Plugin

Supports private financial transactions.

Features:

- Digital invoices
- Payment tracking
- Settlement records
- Lightning Network payments
- Accounting integration

---

## Cold Chain Monitoring Plugin

Supports temperature-sensitive transportation.

Features:

- Temperature sensors
- Refrigeration monitoring
- Alert systems
- Storage condition records

---

## Analytics Plugin

Provides network intelligence.

Features:

- Transportation statistics
- Regional supply analysis
- Route performance
- Cost analysis
- Network optimization

---

# API Architecture

FoodMesh is designed for interoperability.

Supported integrations may include:

- Farm management platforms
- Inventory systems
- Transportation software
- Warehouse systems
- Payment platforms
- Sensor networks
- Mapping services

APIs allow organizations to build specialized applications while remaining compatible with the specification.

---

# Deployment Models

FoodMesh can support:

## Cooperative Networks

Regional farms and carriers operate a shared logistics system.

## Private Enterprise Networks

Companies deploy their own FoodMesh-compatible infrastructure.

## Community Food Networks

Local communities create transportation systems connecting producers and consumers.

## Commercial Logistics Platforms

Transportation companies build services using the open specification.

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
  - [https://roxanneardary.com/foodmesh/](https://roxanneardary.com/foodmesh/)  

---

## License & Notice Requirements

FoodMesh is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- FoodMesh specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

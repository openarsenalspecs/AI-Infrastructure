# LocaleMaterials Specification
**Where Geography Meets Material Science.**
- HTML Mirror:  [https://roxanneardary.com/localematerials-specification/](https://roxanneardary.com/localematerials-specification/)  

---

## Purpose

LocaleMaterials is an open-source, modular AI platform for identifying, evaluating, producing, sourcing, and applying regenerative, renewable, reclaimed, and locally available building materials.

The system shall combine geographic intelligence, material science, environmental conditions, local resource availability, supply chains, construction requirements, lifecycle economics, climate resilience, and real-world performance data to generate location-specific building recommendations.

LocaleMaterials shall prioritize materials and construction systems that can be sourced, grown, harvested, processed, manufactured, reclaimed, or reused as close to the project location as reasonably possible.

The system shall prioritize options in the following order:

- On-site resources
- Hyperlocal resources
- Local resources
- Regional resources
- Statewide resources
- National resources
- International resources only when justified

The system shall evaluate environmental performance and economic practicality together rather than treating sustainability as a separate consideration from cost.

---

## Design Principles

LocaleMaterials shall be designed according to the following principles:

- Open-source development
- Modular architecture
- Local-first sourcing
- Regenerative resource use
- Renewable material preference
- Circular material use
- Transparent calculations
- Explainable AI
- Evidence-based recommendations
- Real-world validation
- Lifecycle economics
- Climate resilience
- Human review
- Vendor neutrality
- Interoperability
- Local-first data processing where practical
- No reliance on proprietary supplier ecosystems
- No unsupported sustainability claims

---

## Core Modules

### Geographic and Site Intelligence Module

The Geographic and Site Intelligence Module shall analyze the physical and environmental characteristics of a project location.

Features shall include:

- Address and coordinate analysis
- Parcel and regional analysis where data is available
- Soil composition analysis
- Soil texture analysis
- Soil mineral analysis
- Soil suitability analysis
- Geology analysis
- Topography analysis
- Elevation analysis
- Hydrology analysis
- Watershed analysis
- Drainage analysis
- Groundwater considerations
- Flood-risk analysis
- Climate-zone identification
- Temperature analysis
- Precipitation analysis
- Humidity analysis
- Freeze and thaw analysis
- Wind exposure analysis
- Solar exposure analysis
- Seasonal analysis
- Native ecological resource analysis
- Agricultural resource analysis
- Forestry resource analysis
- Biomass availability analysis
- Local waste-stream analysis

The module shall provide geographic context to all downstream recommendation modules.

### Material Intelligence Module

The Material Intelligence Module shall maintain structured information about building materials and construction systems.

Material records shall support:

- Material composition
- Source type
- Renewable status
- Regenerative potential
- Recycled content
- Reclaimed status
- Resource requirements
- Thermal properties
- Structural properties
- Moisture behavior
- Fire performance
- Acoustic properties
- Durability
- Pest resistance
- Weather resistance
- Repairability
- Reusability
- Recyclability
- End-of-life pathways
- Expected service life
- Maintenance requirements
- Manufacturing requirements
- Processing requirements
- Geographic suitability
- Climate suitability
- Construction applications

The module shall distinguish between natural, renewable, regenerative, recycled, reclaimed, reused, finite, and non-renewable resources.

### AI Material Recommendation Module

The AI Material Recommendation Module shall generate location-specific material and construction-system recommendations.

The module shall evaluate:

- Project location
- Building type
- Project scale
- Climate
- Soil
- Resource availability
- Material availability
- Budget
- Labor requirements
- Equipment requirements
- Construction method
- Construction timeline
- Durability requirements
- Resilience requirements
- Regulatory requirements
- User-defined priorities

The module shall provide:

- Ranked recommendations
- Alternative recommendations
- Hybrid system recommendations
- Material substitutions
- Recommendation explanations
- Confidence levels
- Evidence references
- Known limitations
- Tradeoff analysis

AI-generated recommendations shall not override deterministic constraints or verified requirements.

### LocaleScore Module

The LocaleScore Module shall provide a transparent scoring framework for comparing materials and construction systems.

Scoring factors shall include, where applicable:

- Regeneration rate
- Renewable availability
- Resource abundance
- Embodied energy
- Embodied carbon
- Transportation distance
- Transportation energy
- Water requirements
- Land requirements
- Toxicity
- Worker exposure considerations
- Occupant exposure considerations
- Durability
- Repairability
- Reusability
- Recyclability
- End-of-life impact
- Waste generation
- Local economic benefit
- Supply-chain resilience
- Climate resilience
- Resource dependency

Scoring weights shall be configurable.

The system shall expose the factors, weights, assumptions, and calculations contributing to each score.

### Local-First Sourcing Module

The Local-First Sourcing Module shall identify material sources according to geographic proximity and project requirements.

The module shall search for:

- On-site resources
- Local producers
- Farmers
- Fiber producers
- Timber producers
- Sawmills
- Clay sources
- Aggregate sources
- Lime producers
- Salvage yards
- Reuse centers
- Demolition inventories
- Material exchanges
- Cooperatives
- Independent manufacturers
- Processing facilities

The module shall compare geographic distance, availability, price, transportation requirements, lead time, and supply reliability.

### Grow-It-Yourself Module

The Grow-It-Yourself Module shall identify materials that can potentially be produced from locally grown biological resources.

Features shall include:

- Suitable crops and species
- Geographic suitability
- Soil requirements
- Water requirements
- Growing requirements
- Seasonal requirements
- Time to maturity
- Harvest cycles
- Expected yield
- Acreage requirements
- Harvest methods
- Processing methods
- Drying requirements
- Storage requirements
- Equipment requirements
- Labor requirements
- Estimated production costs
- Regrowth cycles
- Material yield calculations
- Agricultural integration opportunities

The module shall compare growing and processing a material against purchasing and transporting an equivalent material.

### Material Production Module

The Material Production Module shall provide pathways for making or processing locally available materials.

Features shall include:

- Raw material identification
- Ingredient requirements
- Processing requirements
- Equipment requirements
- Labor requirements
- Material ratios where appropriately documented
- Drying requirements
- Curing requirements
- Storage requirements
- Quality-control checkpoints
- Testing requirements
- Production cost estimates
- Expected yields
- Production risks
- Material preparation workflows

The system shall clearly identify processes that require professional expertise, testing, certification, or regulatory approval.

### Lifecycle Cost Module

The Lifecycle Cost Module shall calculate the actual economic cost of material and construction decisions.

Calculations shall include:

- Material purchase cost
- Labor
- Equipment
- Transportation
- Processing
- Installation
- Maintenance
- Repair
- Replacement
- Energy implications
- Disposal
- Salvage value
- Reuse value
- Expected service life
- Cost volatility
- Lifecycle cost

The module shall support comparisons between upfront cost and total lifecycle cost.

### Multi-Objective Optimization Module

The Multi-Objective Optimization Module shall allow users to establish project priorities.

Optimization factors shall include:

- Lowest upfront cost
- Lowest lifecycle cost
- Maximum local sourcing
- Maximum regeneration
- Lowest transportation
- Lowest embodied energy
- Lowest embodied carbon
- Maximum durability
- Maximum resilience
- Fastest construction
- Simplest construction
- Maximum reuse
- Maximum local economic retention
- Minimum waste

The system shall expose tradeoffs rather than hiding conflicting objectives.

### Climate Adaptation Module

The Climate Adaptation Module shall evaluate materials and construction systems against current and projected environmental conditions.

Features shall include:

- Heat resilience
- Flood resilience
- Moisture resilience
- Humidity analysis
- Mold-risk considerations
- Wildfire considerations
- Wind resilience
- Freeze and thaw resilience
- Drought considerations
- Storm resilience
- Long-term climate scenarios
- Short-term resilience analysis
- Long-term resilience analysis

The module shall provide:

- Current optimal recommendations
- Future-resilient recommendations
- Low-cost resilient alternatives
- Resilience tradeoff analysis

### AI Design Co-Pilot Module

The AI Design Co-Pilot Module shall assist with early-stage building and site planning before final material selection.

Features shall include:

- Site-responsive building concepts
- Building-form recommendations
- Orientation recommendations
- Passive solar strategies
- Passive cooling strategies
- Natural ventilation strategies
- Material-minimizing design strategies
- Climate-responsive layouts
- Local construction-method recommendations
- Building-system comparisons
- Preliminary material quantity estimates
- Design alternatives

The module shall provide preliminary planning intelligence and shall not represent conceptual AI outputs as stamped architectural or engineering documents.

### Regional Material Ecosystem Module

The Regional Material Ecosystem Module shall provide geographic intelligence about the material resources and production capacity of a region.

Maps shall support:

- Material abundance
- Material scarcity
- Agricultural resources
- Forestry resources
- Industrial byproducts
- Agricultural waste streams
- Salvage inventories
- Reclaimed materials
- Processing capacity
- Manufacturing capacity
- Supply gaps
- Supply dependencies
- Transportation routes
- Regional production opportunities

The module shall support analysis of regional material self-sufficiency.

### Circular Material Economy Module

The Circular Material Economy Module shall identify opportunities to keep materials and components in productive use.

Features shall include:

- Salvaged-material discovery
- Reclaimed-material matching
- Demolition-material recovery
- Construction-waste matching
- Material reuse planning
- Component reuse
- Surplus-material exchange
- Local material marketplaces
- Regional material loops
- Industrial symbiosis
- Agricultural-to-construction resource matching

### Construction Systems Module

The Construction Systems Module shall organize materials into complete building assemblies.

Supported systems shall include:

- Wall systems
- Roof systems
- Floor systems
- Foundation systems
- Insulation systems
- Exterior finishes
- Interior finishes
- Moisture-management systems
- Drainage systems
- Passive heating systems
- Passive cooling systems
- Natural ventilation systems

Each system shall support:

- Required materials
- Quantities
- Assembly sequence
- Performance characteristics
- Climate suitability
- Cost
- Maintenance requirements
- Expected service life
- Risks
- Alternatives

### Code Compliance Module

The Code Compliance Module shall connect material recommendations with applicable construction requirements.

Features shall include:

- Jurisdiction identification
- Applicable-code identification
- Code requirement mapping
- Material-to-code crosswalks
- Performance requirement identification
- Documentation requirements
- Alternative-material pathways
- Testing requirements
- Engineering requirements
- Compliance gap identification
- Permit documentation assistance

The module shall clearly distinguish informational code analysis from official regulatory approval, professional engineering, architectural services, inspections, and certifications.

### Verified Assembly Module

The Verified Assembly Module shall maintain construction assemblies supported by appropriate documentation.

Records shall support:

- Test data
- Engineering data
- Fire testing
- Moisture testing
- Thermal testing
- Structural testing
- Manufacturer documentation
- Published research
- Building-code references
- Geographic suitability
- Climate suitability
- Installation requirements
- Version history
- Evidence provenance

Verification status shall be clearly displayed.

### Construction Package Module

The Construction Package Module shall transform recommendations into project documentation.

Generated outputs shall include:

- Material schedules
- Bills of materials
- Quantity estimates
- Cost summaries
- Tool lists
- Construction sequences
- Material preparation instructions
- Maintenance plans
- Compliance summaries
- Sourcing reports
- Environmental impact reports
- Lifecycle-cost reports

### Material Substitution Module

The Material Substitution Module shall identify alternatives when recommended materials are unavailable or impractical.

Substitutions shall be evaluated according to:

- Functional equivalence
- Local availability
- Climate suitability
- Performance
- Cost
- Regeneration
- Embodied energy
- Transportation
- Installation requirements
- Durability
- End-of-life characteristics

The system shall explain the consequences and tradeoffs of substitutions.

### Material Testing Module

The Material Testing Module shall provide a framework for recording material and assembly validation.

Supported records shall include:

- Laboratory tests
- Field tests
- Moisture measurements
- Thermal measurements
- Strength measurements
- Durability observations
- Fire testing
- Aging observations
- Installation results
- Quality-control results

Test records shall retain provenance and applicable metadata.

### Failure and Performance Module

The Failure and Performance Module shall maintain real-world information about successful and unsuccessful material applications.

Records shall include:

- Material failures
- Assembly failures
- Climate-related failures
- Moisture failures
- Pest failures
- Fire failures
- Structural failures
- Installation mistakes
- Incorrect material combinations
- Maintenance problems
- Cost overruns
- Unexpected performance

Failures shall be treated as valuable data rather than suppressed or excluded from recommendations.

### Project Benchmarking Module

The Project Benchmarking Module shall allow users to compare completed and proposed projects.

Comparison factors shall include:

- Geography
- Climate
- Building type
- Material system
- Construction method
- Initial cost
- Lifecycle cost
- Performance
- Maintenance
- Longevity
- Environmental impact
- Resilience
- Local economic impact

### Disaster Rebuild Module

The Disaster Rebuild Module shall support rapid material and construction planning following disruptive events.

Supported scenarios shall include:

- Hurricanes
- Floods
- Wildfires
- Earthquakes
- Tornadoes
- Severe storms
- Infrastructure failures

Features shall include:

- Rapid local-resource assessment
- Salvage-resource mapping
- Emergency material sourcing
- Temporary shelter recommendations
- Rapid construction systems
- Local labor identification
- Supply-chain disruption analysis
- Reconstruction planning
- Temporary-to-permanent transition planning
- Regenerative rebuilding strategies

### Regenerative Index Module

The Regenerative Index Module shall evaluate complete buildings, developments, and construction projects.

Evaluation factors shall include:

- Material regeneration
- Ecological impact
- Soil impact
- Water impact
- Local resource utilization
- Local economic retention
- Waste reduction
- Carbon lifecycle
- Transportation
- Durability
- Repairability
- Reuse
- End-of-life recovery
- Resilience

The system shall provide transparent project-level scores and improvement recommendations.

### Finance and Insurance Module

The Finance and Insurance Module shall organize information useful for financial and risk-analysis processes.

Features shall include:

- Lifecycle-cost analysis
- Replacement-cost estimates
- Durability information
- Risk profiles
- Maintenance projections
- Resilience characteristics
- Comparable construction systems
- Supporting documentation

Outputs shall be informational and shall not represent underwriting, lending, appraisal, insurance, legal, architectural, or engineering decisions.

### Explanation and Evidence Module

The Explanation and Evidence Module shall explain the basis of recommendations.

Each significant recommendation shall be capable of displaying:

- Geographic reasoning
- Climate reasoning
- Soil reasoning
- Ecological reasoning
- Material reasoning
- Economic reasoning
- Availability reasoning
- Rejected alternatives
- Tradeoffs
- Risks
- Evidence
- Confidence
- Known limitations

The module shall maintain provenance for datasets, research, test results, supplier information, calculations, models, and recommendations.

### Community Contribution Module

The Community Contribution Module shall allow users to contribute real-world knowledge.

Supported contributions shall include:

- Materials
- Suppliers
- Local prices
- Production methods
- Construction techniques
- Field results
- Failures
- Regional knowledge
- Material availability
- Material yields
- Project outcomes

Contributions shall support attribution, review, validation, versioning, and correction.

### Human Review Module

The Human Review Module shall allow users and qualified professionals to review system outputs.

Features shall include:

- Recommendation approval
- Recommendation rejection
- Assumption modification
- Ranking overrides
- Local knowledge additions
- Data-quality flags
- Evidence review
- Professional review workflows
- Project outcome recording

Human decisions shall remain distinguishable from automated system recommendations.

### Offline Field Module

The Offline Field Module shall support construction and rural environments with limited connectivity.

Features shall include:

- Offline maps
- Offline material information
- Offline project data
- Offline calculations
- Offline documentation
- Local dataset storage
- Synchronization when connectivity is restored

### API and Integration Module

The API and Integration Module shall expose LocaleMaterials capabilities to external systems.

Supported integrations may include:

- Architecture software
- Construction-management systems
- GIS platforms
- Municipal planning systems
- Building-planning tools
- Material marketplaces
- Supply-chain systems
- Research systems
- Environmental databases

The API shall support modular access to data, recommendations, scoring, geographic analysis, and project outputs.

### Regional Planning Module

The Regional Planning Module shall extend LocaleMaterials from individual projects to communities and regions.

Features shall include:

- Regional material inventories
- Construction-resource planning
- Material dependency analysis
- Local manufacturing opportunities
- Waste-stream utilization
- Disaster preparedness
- Housing-resource analysis
- Regional resilience planning
- Material self-sufficiency analysis
- Regional production opportunity identification

### Transparency and Trust Module

The Transparency and Trust Module shall provide visibility into system behavior.

Users shall be able to inspect:

- Recommendation inputs
- Scoring criteria
- Scoring weights
- Data sources
- Calculation methods
- AI retrieval sources
- Confidence levels
- Assumptions
- Known limitations
- Conflicting evidence
- Model versions
- Dataset versions

---

## Optional Plugin Modules

LocaleMaterials shall support optional plugins that extend functionality without requiring changes to the core system.

Potential plugins shall include:

### Geographic Dataset Plugins

- Additional soil datasets
- Additional climate datasets
- Regional ecological datasets
- Hydrology datasets
- Topography datasets
- Forestry datasets
- Agricultural datasets

### Material Database Plugins

- Natural material databases
- Regenerative material databases
- Reclaimed material databases
- Regional material catalogs
- Specialized material-science databases

### Supplier Network Plugins

- Regional supplier networks
- Local producer directories
- Salvage networks
- Cooperative networks
- Material exchange networks
- Manufacturing networks

### Building Code Plugins

- National code datasets
- State code datasets
- Municipal code datasets
- Regional construction standards
- Specialized building standards

### Climate Model Plugins

- Climate projection datasets
- Extreme-weather models
- Regional resilience models
- Hazard datasets

### Agricultural Production Plugins

- Crop databases
- Fiber crop databases
- Biomass yield models
- Regenerative agriculture datasets
- Regional growing calendars

### Forestry Plugins

- Regional forestry datasets
- Species databases
- Growth-cycle data
- Timber resource inventories
- Regenerative forestry information

### Marketplace Plugins

- Supplier marketplaces
- Salvage marketplaces
- Material exchanges
- Cooperative purchasing systems
- Local manufacturing marketplaces

### GIS Plugins

- Additional map providers
- Specialized spatial datasets
- Parcel data
- Infrastructure data
- Regional planning data

### Construction Software Plugins

- Building information modeling integrations
- Estimating systems
- Construction-management systems
- Project-management systems
- Quantity-takeoff systems

### AI Model Plugins

- Local AI models
- Remote AI models
- Specialized material-science models
- Geospatial models
- Construction reasoning models
- Translation models

---

## AI Requirements

The AI system shall operate as a reasoning and interface layer over structured data, deterministic calculations, retrieval systems, and validated knowledge.

The system shall:

- Prefer sourced information over unsupported generation
- Identify uncertainty
- Cite evidence where available
- Distinguish facts from estimates
- Distinguish estimates from recommendations
- Expose assumptions
- Respect deterministic constraints
- Support multiple AI models
- Avoid unnecessary vendor lock-in
- Permit local model deployment where practical
- Preserve provenance throughout the recommendation process

The AI shall not fabricate suppliers, test results, building-code requirements, material properties, certifications, or scientific evidence.

## Data Requirements

Data shall support:

- Geographic provenance
- Source attribution
- Collection date
- Update date
- Geographic coverage
- Data quality
- Confidence level
- Licensing information
- Version information
- Validation status

The system shall distinguish between verified, reported, estimated, modeled, community-contributed, and unverified information.

## Economic Requirements

The system shall prioritize economic practicality alongside environmental performance.

Economic analysis shall account for:

- Acquisition cost
- Production cost
- Processing cost
- Labor
- Transportation
- Equipment
- Maintenance
- Replacement
- Energy
- Disposal
- Salvage
- Reuse
- Service life
- Price volatility
- Availability
- Supply-chain risk

The system shall avoid assuming that the most environmentally favorable option is automatically the most economical option.

## Regenerative Requirements

The system shall distinguish between:

- Renewable
- Regenerative
- Recyclable
- Reusable
- Reclaimed
- Recycled
- Low-impact
- Non-renewable
- Finite
- Extractive

A material shall not be classified as regenerative solely because it is marketed as sustainable.

Regenerative claims shall be supported by documented evidence, defined criteria, or clearly identified assumptions.

## Safety and Professional Review

LocaleMaterials shall identify situations requiring qualified professionals.

These may include:

- Structural engineering
- Electrical work
- Plumbing
- Fire protection
- Hazardous material handling
- Building-code approval
- Architectural services
- Geotechnical analysis
- Structural testing
- Professional certification
- Permit approval
- Insurance underwriting
- Financial underwriting

The platform shall provide decision support and documentation assistance without presenting automated recommendations as professional certification or official approval.

## Modularity Requirements

Modules shall:

- Have defined interfaces
- Minimize unnecessary dependencies
- Be independently testable
- Support independent updates
- Support optional activation
- Support replacement where practical
- Preserve core functionality when optional modules are unavailable
- Maintain documented inputs and outputs

Optional plugins shall not be required for the core recommendation system.

## Local-First Architecture

LocaleMaterials shall support local-first operation wherever technically practical.

The architecture shall support:

- Local data caching
- Local databases
- Offline operation
- Self-hosted deployments
- Regional deployments
- Community-managed instances
- Synchronization
- Federated data possibilities

## Technical Stack

### Backend

- Python
- FastAPI
- Pydantic
- GeoPandas
- Shapely
- Rasterio

### Geospatial and Data

- PostgreSQL
- PostGIS
- DuckDB
- Parquet
- GeoJSON
- Raster datasets
- Vector datasets
- Spatial indexing

### AI

- Retrieval-Augmented Generation
- Embedding-based retrieval
- Deterministic scoring
- Rule-based constraints
- Explainable recommendation logic
- Confidence estimation
- Model-independent AI interfaces
- Local and remote model support

### Frontend

- Progressive Web App
- React or SvelteKit
- Responsive interface
- Map-driven workflows
- Offline-capable functionality

### Infrastructure

- Containerized deployment
- API-first architecture
- Modular services
- Local-first operation
- Self-hosted deployment
- Regional deployments
- Community-hosted instances

### Development

- GitLab
- Automated testing
- Continuous integration
- Continuous deployment
- Version-controlled source code
- Version-controlled datasets
- Version-controlled scoring models
- Modular plugins
- Documented APIs

## Open-Source Requirements

LocaleMaterials shall remain an open-source project licensed under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.

The project shall support:

- Forking
- Self-hosting
- Modification
- Redistribution
- Regional deployments
- Community datasets
- Independent modules
- Plugin development
- Auditable algorithms
- Transparent scoring
- Collaborative development
- Network-deployed open-source versions

## Project Outputs

LocaleMaterials shall be capable of producing:

- Material recommendations
- Material comparisons
- Local sourcing reports
- Grow-it-yourself plans
- Material production pathways
- Lifecycle cost comparisons
- Climate adaptation reports
- Design recommendations
- Regional material maps
- Construction-system recommendations
- Code analysis
- Compliance documentation
- Bills of materials
- Construction packages
- Material substitution reports
- Performance reports
- Failure reports
- Disaster rebuild plans
- Regenerative Index reports
- Finance and insurance support reports
- Regional resource assessments

## Primary Decision Framework

LocaleMaterials shall continuously evaluate the following questions:

- What resources are available at the project location?
- What resources can regenerate in that location?
- What materials can be grown?
- What materials can be produced locally?
- What materials can be reclaimed or reused?
- What materials can be sourced locally?
- What materials must be transported?
- What is the true lifecycle cost?
- What environmental impacts result from each option?
- What construction system best fits the location?
- What will perform under current conditions?
- What will remain resilient under changing conditions?
- What regulatory requirements apply?
- What evidence supports the recommendation?
- What uncertainties remain?
- What alternatives provide better outcomes?

## Long-Term Vision

LocaleMaterials shall provide a general-purpose intelligence layer for place-based construction.

The system shall connect:

**Geography → Resources → Materials → Design → Construction → Economics → Resilience → Regeneration**

The long-term objective is to enable buildings and communities to make better use of the resources available around them while reducing unnecessary extraction, transportation, waste, supply-chain dependency, and lifecycle cost.

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
  - [https://roxanneardary.com/localematerials/](https://roxanneardary.com/localematerials/)  

---

# 🔓 License & Notice Requirements

LocaleMaterials is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- LocaleMaterials specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments. Any updates that add contributors or modify attribution must update `notice.md`.  
- When submitting pull requests, ensure new files maintain attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the project's `notice.md` file.  

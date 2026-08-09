# OptiRank

**Smarter Pages. Better Rankings.**

OptiRank is an open-source SEO and LLM optimization platform designed to analyze and improve existing website content for both traditional search engines and AI-driven discovery systems.

For more than two decades, SEO has focused primarily on helping search engines crawl, understand, and rank websites. As search increasingly shifts toward AI systems that interpret, summarize, retrieve, and personalize information, websites need to optimize not only for indexing and ranking, but also for machine understanding.

OptiRank addresses this transition by providing a modular analysis and optimization system that evaluates website content, identifies weaknesses, and provides actionable recommendations for improving traditional SEO, semantic relevance, structured information, and LLM discoverability.

## Project Goals

OptiRank is designed to:

- Analyze existing website content rather than require content generation.
- Improve traditional search engine optimization.
- Improve semantic clarity and machine understanding.
- Prepare content for AI-powered search and retrieval systems.
- Identify technical barriers to crawling and indexing.
- Evaluate how clearly a page communicates its subject, entities, relationships, and intent.
- Provide actionable recommendations instead of simply reporting scores.
- Support self-hosted, open-source deployments.
- Maintain a modular architecture that can evolve with search and AI technologies.
- Allow optional capabilities to be added without modifying the core platform.

## Modular Design

OptiRank uses a modular architecture in which each major capability operates as an independent module.

The core platform provides the shared infrastructure required to crawl websites, extract content, analyze pages, calculate scores, generate recommendations, store results, and present reports.

Core modules provide the primary OptiRank functionality and are intended to work together as an integrated analysis pipeline.

Optional plugin modules extend OptiRank with additional capabilities without requiring those capabilities to be part of the core installation.

This architecture allows OptiRank to remain lightweight while providing a framework for expanding into new search engines, AI systems, content types, data sources, and optimization methods.

## Core Modules

### 1. Crawler Module

The Crawler Module discovers and retrieves website pages for analysis.

Features include:

- Website discovery and crawling
- Internal link discovery
- Sitemap discovery
- Robots.txt detection
- Canonical URL detection
- Redirect detection
- Crawl depth tracking
- HTTP status analysis
- Duplicate URL detection
- Crawl scheduling
- Configurable crawl limits
- Dynamic page rendering support

The crawler provides the page data used by the other OptiRank modules.

### 2. Content Extraction Module

The Content Extraction Module converts retrieved webpages into structured content that can be analyzed.

Features include:

- HTML parsing
- Main content extraction
- Navigation detection
- Header extraction
- Paragraph extraction
- List extraction
- Table extraction
- Image extraction
- Link extraction
- Metadata extraction
- Structured data extraction
- Content-to-code ratio analysis

### 3. Technical SEO Module

The Technical SEO Module evaluates technical factors that affect crawling, indexing, and search visibility.

Features include:

- Title analysis
- Meta description analysis
- Heading hierarchy analysis
- Canonical URL analysis
- Robots directives analysis
- Robots.txt analysis
- XML sitemap analysis
- HTTP status analysis
- Redirect analysis
- Broken link detection
- Indexability analysis
- Crawlability analysis
- Mobile-related checks
- HTTPS checks
- Page performance signals
- Duplicate URL detection

### 4. Content SEO Module

The Content SEO Module evaluates how effectively existing content communicates its subject and satisfies search intent.

Features include:

- Keyword analysis
- Topic identification
- Topic coverage analysis
- Search intent analysis
- Content depth analysis
- Content freshness analysis
- Thin content detection
- Duplicate content detection
- Readability analysis
- Heading optimization
- Title optimization
- Meta description optimization
- Content structure analysis

### 5. Semantic Analysis Module

The Semantic Analysis Module evaluates the meaning and relationships contained within website content.

Features include:

- Semantic topic extraction
- Entity identification
- Entity relationship analysis
- Topic clustering
- Context analysis
- Related concept detection
- Semantic similarity analysis
- Content-to-topic alignment
- Context completeness analysis
- Knowledge graph-oriented relationships

This module helps determine whether a page clearly establishes what it is about and how its concepts relate to one another.

### 6. Structured Data Module

The Structured Data Module analyzes machine-readable information contained within webpages.

Features include:

- Schema.org detection
- JSON-LD analysis
- Microdata analysis
- RDFa analysis
- Schema validation
- Missing structured data detection
- Entity-to-schema alignment
- Structured data recommendations
- Content and structured data consistency checks

### 7. Internal Linking Module

The Internal Linking Module evaluates how information is connected throughout a website.

Features include:

- Internal link discovery
- Orphan page detection
- Internal link density analysis
- Anchor text analysis
- Contextual link recommendations
- Related page recommendations
- Topic cluster analysis
- Link hierarchy analysis
- Internal authority flow analysis

### 8. LLM Optimization Module

The LLM Optimization Module evaluates content for retrieval, interpretation, summarization, and AI-assisted discovery.

Features include:

- AI readability analysis
- Semantic clarity analysis
- Context completeness analysis
- Question-and-answer structure analysis
- Entity clarity analysis
- Definition detection
- Answer extraction analysis
- Passage-level usefulness analysis
- AI citation readiness analysis
- Retrieval-oriented content recommendations
- Machine interpretation recommendations

The goal is not to optimize content for one specific AI model. Instead, OptiRank evaluates characteristics that can make content easier for AI systems to understand, retrieve, summarize, and associate with relevant questions.

### 9. AI Visibility Module

The AI Visibility Module evaluates how effectively a website communicates information that may be useful to AI-driven search and retrieval systems.

Features include:

- Topic authority analysis
- Entity authority analysis
- Information completeness scoring
- Citation-worthiness analysis
- Answer usefulness scoring
- Content consistency analysis
- Source attribution analysis
- AI discoverability scoring
- Page-level AI visibility scoring
- Site-level AI visibility scoring

### 10. Scoring Module

The Scoring Module combines analysis from the individual core modules into understandable measurements.

Features include:

- Technical SEO Score
- Content SEO Score
- Semantic Score
- Structured Data Score
- Internal Linking Score
- LLM Optimization Score
- AI Visibility Score
- Overall OptiRank Score
- Page-level scoring
- Site-wide scoring
- Category-level scoring
- Score history
- Comparative scoring

Scores are intended to identify areas for improvement rather than serve as direct predictions of search rankings.

### 11. Recommendation Module

The Recommendation Module converts analysis into actionable optimization tasks.

Features include:

- Prioritized recommendations
- Severity classification
- Impact estimates
- Implementation guidance
- Page-specific recommendations
- Site-wide recommendations
- Technical recommendations
- Content recommendations
- Semantic recommendations
- LLM optimization recommendations
- Duplicate recommendation suppression
- Recommendation status tracking

Recommendations should focus on what needs to change, why it matters, and where the change should be made.

### 12. Reporting Module

The Reporting Module provides a unified view of website optimization results.

Features include:

- Site health reports
- Page reports
- SEO reports
- LLM optimization reports
- Technical reports
- Content reports
- Semantic reports
- Structured data reports
- Internal linking reports
- Prioritized issue lists
- Score trends
- Exportable reports

Supported export formats may include:

- JSON
- CSV
- PDF
- HTML

### 13. Dashboard Module

The Dashboard Module provides the user interface for managing websites, crawls, audits, scores, and recommendations.

Features include:

- Website management
- Crawl management
- Audit status
- Site health overview
- Page-level analysis
- Module-specific scores
- Recommendation management
- Historical comparisons
- Search and filtering
- Report generation
- Configuration management

## Optional Plugin Modules

OptiRank supports optional plugins that extend the core platform without increasing the required complexity of the base installation.

### Search Engine Plugins

Optional search engine integrations may provide:

- Search performance data
- Search query analysis
- Ranking data
- Index coverage information
- Search appearance information
- Search-specific recommendations

Potential integrations can be developed for services such as Google Search Console, Bing Webmaster Tools, and other search platforms.

### AI Platform Plugins

Optional AI platform plugins can provide platform-specific analysis and testing.

Potential capabilities include:

- AI search visibility monitoring
- AI response testing
- Citation monitoring
- Mention monitoring
- Retrieval testing
- Platform-specific recommendations

### CMS Plugins

CMS plugins can connect OptiRank directly to content management systems.

Potential integrations include:

- WordPress
- Drupal
- Ghost
- Joomla
- Headless CMS platforms
- Custom CMS systems

CMS plugins may allow users to review recommendations and apply approved changes directly from the OptiRank interface.

### Content Management Plugins

Optional plugins may provide controlled content optimization workflows.

Capabilities may include:

- Title recommendations
- Meta description recommendations
- Heading recommendations
- Internal link recommendations
- Alt text recommendations
- Content restructuring suggestions
- Human approval workflows

OptiRank is intended to provide recommendations for existing content rather than automatically replacing content without user approval.

### Analytics Plugins

Optional analytics integrations can connect website behavior data to OptiRank analysis.

Potential integrations include:

- Traffic analytics
- Engagement analytics
- Conversion analytics
- Search traffic analysis
- Content performance analysis

### Language Plugins

Language plugins can extend analysis to additional languages.

Potential capabilities include:

- Multilingual NLP
- Language-specific readability scoring
- Language-specific semantic analysis
- Multilingual entity extraction
- Translation-aware content analysis

### Knowledge Graph Plugins

Optional knowledge graph integrations can extend semantic analysis.

Potential capabilities include:

- Entity enrichment
- Entity relationship mapping
- Knowledge graph comparison
- External entity verification
- Topic authority analysis

### AI Model Plugins

OptiRank may support optional local or remote AI model providers.

Potential integrations include:

- Local open-weight models
- Self-hosted inference servers
- Embedding models
- Classification models
- Summarization models
- Semantic similarity models

AI model integrations should remain provider-independent so that users are not locked into a single AI vendor.

## Plugin Architecture

Plugins should interact with OptiRank through defined interfaces rather than modifying core modules directly.

A plugin may provide:

- New analysis capabilities
- New data sources
- New integrations
- New scoring methods
- New recommendation types
- New report formats
- New dashboards
- New AI model providers

Plugins should be independently enableable and disableable.

Core functionality must not depend on optional commercial services or proprietary APIs.

## Technology Stack

### Backend

- Python
- FastAPI
- Pydantic
- SQLAlchemy

### Frontend

- React
- TypeScript
- Recharts

### Crawling

- Scrapy
- Playwright
- HTTPX

### HTML and Content Processing

- BeautifulSoup
- lxml
- Readability tooling
- Custom content extraction pipelines

### NLP and Semantic Processing

- spaCy
- Hugging Face Transformers
- Sentence Transformers
- Vector similarity analysis

### LLM Integration

OptiRank uses a provider-independent architecture for LLM functionality.

Supported deployments may use:

- Local open-weight models
- Self-hosted inference
- Compatible model APIs
- Embedding models
- Specialized NLP models

No single proprietary AI provider should be required for core functionality.

### Database

- PostgreSQL for production deployments
- SQLite for lightweight installations and development

### Background Processing

- Redis
- Celery

These components support asynchronous crawling, analysis, indexing, and reporting for larger websites.

### Deployment

- Docker
- Docker Compose
- Linux
- Self-hosted environments

### Development and CI/CD

- GitLab
- GitLab CI/CD
- Python testing frameworks
- TypeScript testing tools
- Automated linting
- Automated security checks

## Analysis Pipeline

OptiRank processes websites through a modular analysis pipeline:

1. Discover the website.
2. Crawl accessible pages.
3. Extract HTML and content.
4. Analyze technical SEO factors.
5. Analyze page content.
6. Extract entities and semantic relationships.
7. Analyze structured data.
8. Evaluate internal linking.
9. Evaluate LLM and AI discoverability characteristics.
10. Calculate module-level scores.
11. Calculate overall site and page scores.
12. Generate prioritized recommendations.
13. Present results through the dashboard.
14. Export reports for implementation and tracking.

Each stage should remain independently testable and replaceable.

## Data Ownership

OptiRank is designed around user-controlled data.

Users should be able to:

- Self-host the application.
- Control website crawl data.
- Control analysis results.
- Select their own AI model providers.
- Use local AI models where practical.
- Export analysis data.
- Remove stored website data.

OptiRank should avoid unnecessary transmission of website content to third-party services.

## Privacy

The core application should not require sending website content to external AI providers.

When optional external integrations are enabled, the application should clearly identify what information is transmitted and to which service.

Local and self-hosted AI processing should be supported wherever practical.

## Extensibility

OptiRank is intended to evolve as search technology changes.

The modular architecture allows new capabilities to be added without redesigning the entire application.

Future modules and plugins may address:

- New search systems
- New AI search platforms
- New LLM architectures
- New structured data standards
- New ranking signals
- New content formats
- New analytics platforms
- New CMS platforms
- New languages
- New semantic models

## Project Philosophy

OptiRank is based on the principle that the future of website visibility will depend on more than traditional ranking signals.

Websites increasingly need to communicate information in ways that can be understood by search engines, retrieval systems, AI models, and ultimately the individualized AI assistants that users increasingly rely upon.

OptiRank therefore focuses on three complementary goals:

- **Rankability:** Can search engines effectively crawl, index, and evaluate the page?
- **Understandability:** Can machines clearly understand what the page means and how its information relates?
- **Retrievability:** Can AI systems identify, extract, and use the page's information when answering relevant questions?

OptiRank is designed to help website owners optimize for all three.

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
  - [https://roxanneardary.com/optirank/](https://roxanneardary.com/optirank/)

---

## License & Notice Requirements

OptiRank is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**. 
- OptiRank specifications are free to use with attribution. A Specification Branding License can be negotiated upon request. 
- The project's `notice.md` file tracks attribution requirements and contributor acknowledgments. Any updates that add contributors or modify attribution must update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the project's `notice.md` file.

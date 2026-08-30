# AllPost
**One post. Every platform.**
- HTML Mirror:  [https://roxanneardary.com/allpost-specification/](https://roxanneardary.com/allpost-specification/)  

---

## Specification

AllPost is an open source, self-hostable social publishing platform designed to allow users to create, adapt, schedule, manage, and publish content across multiple social media platforms from a unified application.

AllPost is designed around modularity, extensibility, privacy, encryption, user ownership, accessibility, and platform independence. Social platform integrations are implemented as independently maintainable adapters, while optional plugins extend the capabilities of the core system without requiring changes to the fundamental application.

AllPost is licensed under the GNU Affero General Public License v3.0 or later (AGPL-3.0+).

## Core Principles

- Open source
- Self-hostable
- Modular by design
- Plugin extensible
- Platform independent
- User owned data
- Privacy by design
- Encryption by default
- Secure authentication
- Human controlled AI
- Transparent system behavior
- Accessible by design
- Data portability
- Vendor independence
- API first architecture
- Mobile and desktop compatible
- Long term maintainability

---

## Core Application Module

The Core Application Module provides the foundational services required by every AllPost deployment.

### Core Responsibilities

- Application lifecycle management
- Configuration management
- User management
- Workspace management
- Content management
- Plugin management
- Permission enforcement
- Event processing
- System configuration
- API coordination
- Security policy enforcement
- Data protection enforcement

The core application must remain independent from individual social media platforms and optional service providers.

## User Module

The User Module manages user accounts and identity within AllPost.

### Features

- User registration
- User authentication
- User profile management
- Account recovery
- Password management
- Session management
- Active device management
- Session revocation
- Security notifications
- User preferences
- Notification preferences
- Privacy preferences
- AI preferences
- Connected-account management

Passwords must never be stored in reversible form.

## Authentication and Identity Module

The Authentication and Identity Module provides secure access to AllPost.

### Features

- Password authentication
- Argon2 password hashing
- Passkeys
- WebAuthn
- TOTP two-factor authentication
- Recovery codes
- Session expiration
- Session revocation
- Device recognition
- Login notifications
- Suspicious-login detection
- Account recovery
- Administrator-controlled authentication policies
- Optional mandatory two-factor authentication

External platform authentication must use secure authorization mechanisms supported by the platform.

## Workspace Module

The Workspace Module provides isolated environments for individuals, teams, organizations, agencies, and clients.

### Features

- Multiple workspaces per user
- Workspace creation
- Workspace invitations
- Workspace membership
- Workspace isolation
- Workspace settings
- Workspace branding
- Workspace-specific integrations
- Workspace-specific content
- Workspace-specific analytics
- Workspace-specific AI settings
- Workspace-specific permissions
- Workspace-specific audit logs
- Workspace-specific retention policies

Users must not gain access to another workspace's private information without explicit authorization.

## Roles and Permissions Module

The Roles and Permissions Module provides role-based access control.

### Default Roles

- Owner
- Administrator
- Editor
- Publisher
- Reviewer
- Analyst
- Viewer

### Features

- Role assignment
- Permission management
- Custom roles
- Platform-specific permissions
- Content-specific permissions
- Integration permissions
- AI permissions
- Analytics permissions
- Audit-log permissions
- Workspace administration permissions
- Permission inheritance controls

Permissions must follow the principle of least privilege.

## Content Module

The Content Module manages the canonical version of every post.

### Features

- Post creation
- Post editing
- Drafts
- Saved posts
- Post duplication
- Post templates
- Content categorization
- Content tagging
- Campaign tagging
- Internal labels
- Content ownership
- Content priority
- Content status
- Content archival
- Content search
- Full-text search
- Semantic search
- Related-content discovery
- Duplicate-content detection
- Content history

The canonical post must remain separate from platform-specific variants.

## Content Versioning Module

The Content Versioning Module maintains a history of changes made to content.

### Features

- Version history
- Platform-specific version history
- Before and after comparison
- Change tracking
- User change attribution
- AI change attribution
- Rollback
- Revision comparison
- Published-version tracking
- Draft-version tracking

AI-generated modifications must be distinguishable from user-created modifications.

## Platform Adaptation Module

The Platform Adaptation Module converts canonical content into platform-specific versions.

### Features

- Character-limit handling
- Formatting adaptation
- Hashtag adaptation
- Mention adaptation
- Link handling
- Media adaptation
- Platform-specific content rules
- Platform-specific validation
- Platform-specific accessibility requirements
- Platform-specific content previews
- Platform-specific recommendations
- Manual editing of generated variants

Users must retain control over every platform-specific version before publication unless they explicitly configure an automated workflow.

## Publishing Module

The Publishing Module coordinates distribution of content to connected platforms.

### Features

- Immediate publishing
- Multi-platform publishing
- Multi-account publishing
- Selective platform publishing
- Platform-specific publishing
- Publication status tracking
- Publication confirmation
- Publication failure reporting
- Retry handling
- Duplicate-publication protection
- Idempotent publishing operations
- Rate-limit awareness
- Platform outage handling

A failed publication on one platform must not unnecessarily prevent successful publication to other selected platforms.

## Scheduling Module

The Scheduling Module manages future publication.

### Features

- Scheduled posts
- Bulk scheduling
- Publishing queues
- Recurring posts
- Time-zone-aware scheduling
- Platform-specific schedules
- Workspace-specific schedules
- User-defined publishing windows
- Optimal-time recommendations
- Queue prioritization
- Retry scheduling
- Rate-limit-aware scheduling
- Failed-publication recovery

## Content Calendar Module

The Content Calendar Module provides visual planning and scheduling.

### Features

- Day view
- Week view
- Month view
- Platform filtering
- Workspace filtering
- Campaign filtering
- Status filtering
- Drag-and-drop scheduling
- Scheduled-post visualization
- Publishing queue visualization
- Content gap identification
- Content frequency monitoring
- Calendar export

## Approval Workflow Module

The Approval Workflow Module provides controlled content review before publication.

### Workflow States

- Draft
- Review
- Revision requested
- Approved
- Scheduled
- Publishing
- Published
- Failed
- Archived

### Features

- Review requests
- Approval requirements
- Multiple reviewers
- Multi-stage approval
- Reviewer comments
- Revision requests
- Publisher authorization
- Platform-specific approval
- Approval history
- Approval audit trail

Workspaces must be able to require approval before content can be published.

## Media Module

The Media Module manages media associated with social content.

### Features

- Central media library
- Image management
- Video management
- Audio management
- Document management
- Media collections
- Media tagging
- Media search
- Media metadata
- Media reuse
- Image resizing
- Video processing
- Thumbnail generation
- Format conversion
- Platform-specific media validation
- Alt-text management
- Copyright metadata
- Licensing metadata

## User Interface Module

The User Interface Module provides the primary AllPost application interface.

### Requirements

- Responsive design
- Desktop support
- Tablet support
- Mobile support
- Progressive Web App support
- Keyboard navigation
- Screen-reader compatibility
- Accessible controls
- Consistent navigation
- Responsive layouts
- Configurable dashboards
- Contextual platform controls

The interface must remain usable across supported device sizes without requiring a separate application architecture.

## UI Design System Module

The UI Design System Module provides reusable interface components and visual standards.

### Components

- Buttons
- Inputs
- Forms
- Cards
- Dialogs
- Menus
- Navigation
- Tables
- Notifications
- Tooltips
- Editors
- Media controls
- Platform previews
- Dashboard components

### Features

- Design tokens
- Component consistency
- Theme support
- Light mode
- Dark mode
- Organization branding
- Custom logos
- Custom typography
- Responsive behavior
- Accessibility standards
- Plugin compatibility

## UI Layout Module

The UI Layout Module provides configurable application layouts.

### Features

- Dashboard layouts
- Drag-and-drop widgets
- Multi-panel composer
- Configurable sidebars
- Configurable navigation
- Workspace-specific layouts
- User-specific layouts
- Responsive layout adaptation
- Layout persistence

## UI Injection Module

The UI Injection Module allows plugins to extend the AllPost interface through controlled extension points.

### Standard UI Slots

- composer.sidebar
- composer.preview
- composer.toolbar
- dashboard.widgets
- post.card.extensions
- settings.integrations
- ai.suggestions.panel

### Requirements

- Slot-based injection
- Controlled component mounting
- No unrestricted DOM manipulation
- No unrestricted global state access
- Prop-based communication
- Permission-scoped capabilities
- Theme-token compliance
- Responsive behavior
- Accessibility compliance
- Deterministic rendering order

Untrusted plugins may be rendered through a sandboxed execution environment.

## Plugin Registry Module

The Plugin Registry Module manages extensions installed into AllPost.

### Features

- Plugin discovery
- Plugin installation
- Plugin removal
- Plugin enablement
- Plugin disabling
- Plugin configuration
- Plugin versioning
- Compatibility checking
- Dependency management
- Permission declarations
- Capability declarations
- Plugin health status
- Plugin lifecycle events

Plugins must explicitly declare the capabilities and permissions they require.

## Plugin Security Module

The Plugin Security Module establishes security boundaries between plugins and the core application.

### Requirements

- Least-privilege permissions
- Capability-based access
- Controlled APIs
- Secret isolation
- Permission validation
- Plugin identity
- Plugin version validation
- Optional sandboxing
- Auditability
- No direct access to encryption keys
- No unrestricted access to user data
- No access to credentials unless explicitly required and securely mediated

Plugins must not receive raw authentication secrets through UI components.

## Audit Module

The Audit Module provides a system-wide append-only record of important actions.

### Logged Events

- User registration
- Login
- Logout
- Two-factor authentication
- Passkey authentication
- Password changes
- Workspace creation
- Workspace membership changes
- Role changes
- Permission changes
- Integration changes
- Post creation
- Post modification
- Post scheduling
- Post approval
- Post publication
- Publication failure
- Post archival
- AI suggestion generation
- AI suggestion acceptance
- AI suggestion rejection
- Plugin installation
- Plugin activation
- Plugin deactivation
- Plugin activity
- Configuration changes

### Audit Record Fields

- Timestamp
- Actor
- Workspace identifier
- Action type
- Resource identifier
- Event identifier
- Structured metadata

Audit records must not contain unnecessary sensitive information.

## Audit Integrity Module

The Audit Integrity Module protects the integrity of audit records.

### Features

- Append-only storage
- Tamper detection
- Optional cryptographic chaining
- Integrity verification
- Timestamp verification
- Export
- JSON export
- CSV export
- Retention controls
- Privacy-preserving logging
- Workspace-specific audit policies

## Encryption and Privacy Module

The Encryption and Privacy Module establishes mandatory protection for personal and sensitive information.

### Mandatory Encryption

Personal and sensitive data must be encrypted at rest.

Protected information includes, where stored:

- Authentication information
- OAuth access tokens
- OAuth refresh tokens
- API keys
- Email addresses
- Identity metadata
- Private workspace information
- Workspace membership information
- Private drafts
- Unpublished content
- AI interaction data
- Sensitive analytics
- Sensitive audit information
- Private media
- Other information capable of identifying a person or reconstructing sensitive behavior

### Encryption Requirements

- Strong authenticated encryption
- AES-256 or an equivalent modern encryption standard
- Application-level encryption and/or appropriately configured storage encryption
- TLS for data in transit
- TLS 1.2 minimum
- TLS 1.3 preferred
- Encrypted internal communications where applicable
- Encryption key separation
- Secure key storage
- Key rotation
- Key lifecycle management
- Secure secret management

Encryption keys must not be stored alongside encrypted data.

## Secret Management Module

The Secret Management Module protects credentials and cryptographic secrets.

### Features

- Secure secret storage
- Encryption-key management
- OAuth credential protection
- API-key protection
- Secret rotation
- Secret revocation
- Environment-secured configuration
- Vault integration
- Self-hosted secret manager support
- Secret access auditing

Secrets must never be intentionally written to application logs.

## AI Module

The AI Module provides optional intelligent assistance for content creation and optimization.

### Features

- AI writing assistance
- Rewrite suggestions
- Grammar correction
- Spelling correction
- Clarity improvement
- Tone recommendations
- Platform-specific recommendations
- Hashtag recommendations
- Tagging recommendations
- Formatting recommendations
- Accessibility recommendations
- Alt-text generation
- Content-length recommendations
- Call-to-action suggestions
- Duplicate-content detection
- Content quality analysis
- Readability analysis
- Brand voice analysis
- Audience-specific recommendations
- Post variation generation

## AI Governance Module

The AI Governance Module provides user control over AI behavior.

### Features

- AI enablement controls
- Workspace-level AI policies
- User-level AI policies
- Post-level AI controls
- Suggest-only mode
- Annotation-only mode
- Controlled automatic editing
- AI change explanations
- Individual suggestion approval
- Suggestion rejection
- AI history controls
- AI retention controls
- AI provider selection
- Local-only AI mode

AI must not silently modify user content.

## Local AI Module

The Local AI Module supports local model execution.

### Supported Integrations

- Ollama
- LM Studio
- Other compatible local inference systems

### Features

- Local model selection
- Local model configuration
- Model capability detection
- Local processing
- Local embeddings
- Local semantic search
- Local content analysis
- Local brand voice analysis
- Local-only privacy mode

## Brand Voice Module

The Brand Voice Module allows workspaces to define content standards.

### Features

- Brand voice profiles
- Tone definitions
- Vocabulary preferences
- Preferred terminology
- Restricted terminology
- Banned phrases
- Preferred hashtags
- Required hashtags
- Preferred calls to action
- Writing rules
- Platform-specific voice rules
- Multiple brand profiles
- Client-specific profiles
- AI adherence checking

## Analytics Module

The Analytics Module provides unified performance information.

### Features

- Cross-platform analytics
- Platform-specific analytics
- Post performance
- Impressions
- Reach
- Engagement
- Likes
- Comments
- Shares
- Reposts
- Saves
- Clicks
- Video views
- Audience growth
- Follower growth
- Engagement rate
- Performance over time
- Campaign performance
- Content performance
- Platform comparison

## Analytics Abstraction Module

The Analytics Abstraction Module normalizes compatible metrics across platforms.

Platform adapters may map native metrics into a common AllPost analytics model while retaining platform-specific metrics that cannot be normalized.

The system must clearly distinguish normalized metrics from platform-specific metrics.

## Notification Module

The Notification Module provides system and workflow notifications.

### Features

- In-app notifications
- Publication notifications
- Failed-publication notifications
- Approval notifications
- Review notifications
- Integration expiration notifications
- Security notifications
- Workspace notifications
- Optional email notifications
- Configurable notification preferences

## Search Module

The Search Module provides centralized discovery across user-authorized content.

### Features

- Global search
- Post search
- Media search
- Workspace search
- Campaign search
- Platform search
- Tag search
- User search
- Full-text search
- Filtered search
- Semantic search
- AI-assisted content discovery

Search must respect workspace and permission boundaries.

## Import and Export Module

The Import and Export Module provides data portability.

### Features

- Content import
- Media import
- Configuration import
- Platform configuration import where supported
- Post export
- Media metadata export
- Analytics export
- Audit-log export
- JSON export
- CSV export
- Portable workspace data
- Backup export
- Migration support

## Backup and Recovery Module

The Backup and Recovery Module protects against data loss.

### Features

- Automated backups
- Scheduled backups
- Encrypted backups
- Database backups
- Workspace backups
- Full-instance backups
- Backup verification
- Restore verification
- Disaster recovery support
- Configuration recovery

## Event System Module

The Event System Module provides internal event-driven communication.

### Standard Events

- user.created
- user.login
- user.logout
- workspace.created
- workspace.member.added
- workspace.member.removed
- post.created
- post.updated
- post.reviewed
- post.approved
- post.scheduled
- post.publishing
- post.published
- post.failed
- post.archived
- ai.suggestion.generated
- ai.suggestion.accepted
- ai.suggestion.rejected
- plugin.installed
- plugin.enabled
- plugin.disabled
- integration.connected
- integration.disconnected

Events must be permission-aware and must not expose protected information to unauthorized subscribers.

## API Module

The API Module provides programmatic access to AllPost.

### Features

- REST API
- Optional GraphQL API
- Authentication API
- User API
- Workspace API
- Content API
- Scheduling API
- Publishing API
- Analytics API
- Plugin API
- UI extension API
- Audit API
- AI API
- Notification API
- Webhook API

### API Requirements

- Authentication
- Authorization
- Permission enforcement
- Rate limiting
- Versioning
- Validation
- Error handling
- Documentation
- Secure defaults

## Webhook Module

The Webhook Module allows AllPost to communicate with external systems.

### Features

- Event-based webhooks
- Configurable webhook endpoints
- Signed webhook requests
- Delivery retries
- Delivery status
- Failure handling
- Webhook authentication
- Webhook event filtering

## Automation Module

The Automation Module allows authorized workflows to respond to system events.

### Features

- Event triggers
- Conditional workflows
- Scheduled workflows
- Webhook triggers
- Post-created actions
- Post-approved actions
- Post-published actions
- Publication-failure actions
- AI suggestion actions
- Analytics-based actions
- Plugin events
- Workflow history

Automation must respect workspace permissions and security policies.

## Offline Module

The Offline Module provides resilient content creation when connectivity is unavailable.

### Features

- Offline draft creation
- Offline draft editing
- Local content queue
- Automatic synchronization
- Synchronization conflict detection
- Conflict resolution
- Network recovery
- Failed synchronization reporting

Offline storage must follow the same privacy and encryption requirements applicable to stored personal data.

## Reliability Module

The Reliability Module provides resilient publication and application behavior.

### Features

- Background job queues
- Automatic retries
- Exponential backoff
- Idempotent operations
- Duplicate-publication protection
- Rate-limit handling
- Failure isolation
- Dead-letter queues
- Recovery workflows
- Platform outage detection
- Integration health monitoring

## Validation Module

The Validation Module verifies content before publication.

### Features

- Character-limit validation
- Media validation
- Platform capability validation
- Unsupported-feature warnings
- Link validation
- Mention validation
- Hashtag validation
- Accessibility validation
- Content-policy warnings
- Duplicate-content warnings
- User-defined validation rules

## Observability Module

The Observability Module provides operational visibility without unnecessarily exposing personal information.

### Features

- Application health monitoring
- Plugin health monitoring
- Integration health monitoring
- Queue monitoring
- Publishing status
- API error monitoring
- Authentication monitoring
- Resource monitoring
- Structured application logs
- Privacy-aware diagnostics

Sensitive information must not be included in diagnostic logs.

## Deployment Module

The Deployment Module supports self-hosted and scalable installations.

### Requirements

- Docker support
- Docker Compose support
- Kubernetes support
- Environment configuration
- Database migrations
- Health checks
- Reverse-proxy compatibility
- TLS configuration
- Secret management
- Backup configuration
- Upgrade procedures
- Local AI deployment
- Self-hosted storage

AllPost must remain usable without requiring a proprietary hosted service.

## Developer Module

The Developer Module provides tools for building and maintaining AllPost extensions.

### Features

- Plugin SDK
- Platform adapter SDK
- UI extension SDK
- API documentation
- TypeScript types
- Example integrations
- Plugin templates
- Test utilities
- Mock platform APIs
- Integration testing
- Compatibility testing
- Plugin validation
- Development tooling
- CI/CD integration

---

## Optional Plugin Modules

Optional functionality must be implemented through plugins when it is not required for the fundamental operation of AllPost.

### Social Platform Plugins

Social platform plugins provide integrations for individual networks.

Each platform plugin may provide:

- Authentication
- Account connection
- Content validation
- Content formatting
- Publishing
- Scheduling capabilities
- Media handling
- Analytics
- Rate-limit rules
- Platform-specific settings
- Platform-specific previews
- UI extensions
- Webhooks
- Platform capability declarations

### AI Provider Plugins

AI provider plugins may provide connections to external AI services.

Examples include:

- Cloud LLM providers
- Local inference providers
- Specialized content models
- Embedding providers
- Image-generation systems
- Speech or transcription systems

Users must explicitly authorize external AI providers.

### Analytics Provider Plugins

Analytics plugins may provide additional analytics systems or specialized measurement capabilities.

### Storage Plugins

Storage plugins may provide alternative media and object-storage backends.

### Workflow Plugins

Workflow plugins may provide additional automation systems and external workflow integrations.

### Notification Plugins

Notification plugins may provide:

- Email
- Messaging
- Push notifications
- External notification services

### Import Plugins

Import plugins may support migration from other publishing systems and content-management applications.

### Export Plugins

Export plugins may support additional portable formats and external destinations.

### Federation Plugins

Federation plugins may provide support for decentralized and federated social protocols.

### Integration Plugins

Integration plugins may connect AllPost to external productivity, publishing, analytics, storage, or business systems.

---

## Social Platform Adapter Contract

Every social platform adapter should provide a standardized capability interface.

### Authentication

- connect()
- authorize()
- refresh()
- disconnect()
- validateConnection()

### Content

- validatePost()
- formatPost()
- previewPost()
- publish()

### Media

- validateMedia()
- uploadMedia()
- formatMedia()

### Platform Rules

- getCharacterLimits()
- getMediaRequirements()
- getRateLimitRules()
- getCapabilities()

### Analytics

- getMetrics()
- normalizeMetrics()

### Optional Extensions

- getUIExtensions()
- getWebhooks()
- getPlatformEvents()

The adapter contract must remain versioned so that platform plugins can evolve independently from the core application.

## Plugin Compatibility

Plugins must declare:

- Plugin identifier
- Plugin version
- AllPost compatibility version
- Required capabilities
- Required permissions
- Dependencies
- Optional dependencies
- Supported platforms
- UI extensions
- API requirements

The core application must validate plugin compatibility before activation.

## Privacy Requirements

AllPost must minimize collection and retention of personal information.

### Requirements

- Collect only necessary information
- Encrypt personal data
- Encrypt sensitive content
- Protect authentication credentials
- Protect platform tokens
- Minimize telemetry
- Avoid unnecessary third-party tracking
- Avoid behavioral advertising
- Provide configurable retention
- Provide data export
- Provide secure deletion where technically applicable
- Respect workspace privacy boundaries

## AI Privacy Requirements

AI functionality must follow additional privacy requirements.

- AI must be optional
- Local AI should be supported
- External AI requires user authorization
- User-provided cloud credentials must be protected
- Sensitive information should be minimized before external processing
- AI history must be configurable
- AI retention must be configurable
- AI providers must not receive information outside the authorized request scope
- AI must not silently retain content through AllPost
- AI-generated changes must remain distinguishable from user changes

## Security Requirements

Security is a core architectural requirement.

### Requirements

- Secure authentication
- Two-factor authentication
- Passkeys
- WebAuthn
- Strong password hashing
- Encryption at rest
- Encryption in transit
- Secure secret management
- Key rotation
- Least-privilege permissions
- Workspace isolation
- Plugin isolation
- Input validation
- Output validation
- Secure API design
- Rate limiting
- Audit logging
- Security event monitoring
- Secure backups
- Dependency security
- Security testing

## Accessibility Requirements

AllPost should follow modern accessibility standards.

### Requirements

- Keyboard accessibility
- Screen-reader compatibility
- Sufficient contrast
- Accessible forms
- Accessible notifications
- Accessible media controls
- Alternative text support
- Focus management
- Semantic HTML
- Responsive interfaces
- Reduced-motion support where appropriate

---

## Technology Stack

### Frontend

- React
- TypeScript
- Vite
- Progressive Web App technologies
- Responsive CSS
- Accessible component architecture

### Backend

The backend may use:

- Node.js
- NestJS
- Go

The final backend implementation should prioritize security, maintainability, performance, modularity, and contributor accessibility.

### API

- REST
- Optional GraphQL
- Webhooks
- Event-driven services

### Database

- PostgreSQL

### Queue and Cache

- Redis

### Object Storage

- S3-compatible storage

### AI

- Ollama
- LM Studio
- Optional external AI providers through plugins

### Authentication

- OAuth 2.0
- PKCE
- WebAuthn
- Passkeys
- TOTP
- Argon2

### Deployment

- Docker
- Docker Compose
- Kubernetes
- GitLab CI/CD

## Testing Requirements

AllPost should maintain automated testing across core functionality.

### Testing Areas

- Unit testing
- Integration testing
- API testing
- Plugin testing
- Platform adapter testing
- UI testing
- Accessibility testing
- Authentication testing
- Encryption testing
- Permission testing
- Workspace isolation testing
- Audit integrity testing
- Scheduling testing
- Publication testing
- Failure recovery testing
- Security testing

Platform adapters should provide mock interfaces for testing without requiring production social-media credentials.

## Documentation Requirements

Documentation should cover:

- Installation
- Configuration
- Self-hosting
- Authentication
- Security
- Encryption
- Workspace management
- User management
- Publishing
- Scheduling
- AI configuration
- Plugin development
- Platform adapter development
- UI extension development
- API usage
- Webhooks
- Deployment
- Backup and recovery
- Troubleshooting
- Contribution requirements

## Open Source Development

AllPost is developed as an open source project.

Contributions may include:

- Core development
- Platform adapters
- Plugins
- UI components
- Accessibility improvements
- AI improvements
- Security improvements
- Documentation
- Testing
- Deployment tooling
- Performance improvements
- Bug fixes

All contributions must comply with the project's licensing and security requirements.

## Design Goals

AllPost is intended to provide:

- One unified publishing experience
- Broad social platform compatibility
- Easy platform expansion
- User-controlled content
- User-controlled credentials
- Encrypted personal data
- Transparent AI assistance
- Secure collaboration
- Extensible interfaces
- Portable data
- Self-hosted operation
- Long-term platform independence

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
  - [https://roxanneardary.com/allpost/](https://roxanneardary.com/allpost/)

---

## 📜 License & Notice Requirements

AllPost is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- AllPost specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

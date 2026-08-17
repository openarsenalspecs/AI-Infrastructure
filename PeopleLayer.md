# PeopleLayer Specification
**Contribute, Verify, Repeat.**
- HTML Mirror:  [https://roxanneardary.com/peoplelayer-specification/](https://roxanneardary.com/peoplelayer-specification/)

---

PeopleLayer is an open-source, modular specification for self-sovereign identity, verifiable credentials, portable reputation, privacy-preserving trust, and cross-platform contribution verification.

The system provides a user-controlled people layer for digital ecosystems. Each participant can maintain a cryptographic identity, receive verifiable credentials, accumulate portable reputation, selectively prove qualifications, and participate in federated trust networks without surrendering identity or reputation to a centralized platform.

## Specification Goals

PeopleLayer is designed to:

- Give individuals direct control over their digital identity and reputation.
- Make meaningful contributions verifiable and portable.
- Separate reputation from centralized platforms.
- Enable privacy-preserving proof of skills, contributions, and trust.
- Prevent unnecessary disclosure of identity and personal information.
- Support pseudonymous and anonymous participation where appropriate.
- Provide interoperable credentials and reputation signals.
- Connect human contributors with trusted AI agents and automated systems.
- Support federated communities without requiring a central authority.
- Provide modular integration points for external applications and services.
- Maintain local-first operation wherever practical.
- Avoid vendor lock-in and proprietary identity dependencies.
- Establish common standards for people-centered trust infrastructure.

---

## Core Modules

### Identity and Wallet Module

The Identity and Wallet Module provides the foundation for user-controlled identity.

Capabilities include:

- Self-sovereign decentralized identifiers.
- Local cryptographic key generation and management.
- User-controlled identity wallets.
- Local-first identity storage.
- DID creation, rotation, recovery, and deactivation.
- Multiple identities and pseudonyms.
- Identity separation for different communities or contexts.
- Cryptographic signing and verification.
- Hardware wallet integration.
- Secure key storage.
- Encrypted wallet backups.
- Recovery mechanisms that do not require a centralized account.
- Identity portability between compatible implementations.
- Optional identity linking when explicitly authorized by the user.
- Support for human identities, organizational identities, and authorized agent identities.

The wallet must not require a centralized cloud account for basic identity ownership.

### Verifiable Credentials Module

The Verifiable Credentials Module provides portable proof of skills, contributions, activities, qualifications, and community recognition.

Capabilities include:

- Credential issuance.
- Credential acceptance.
- Credential storage.
- Credential presentation.
- Cryptographic credential verification.
- Credential expiration.
- Credential suspension.
- Credential revocation.
- Credential renewal.
- Credential versioning.
- Credential provenance.
- Credential issuer verification.
- Credential subject verification.
- Credential schema management.
- Contribution-specific credential types.
- Skill-specific credential types.
- Civic participation credentials.
- Open-source contribution credentials.
- Security contribution credentials.
- Research and knowledge contribution credentials.
- Community service credentials.
- Human stewardship credentials.

Example credentials may include:

- Verified Election Observer: 47 precincts audited.
- Trademark Infringements Flagged: 12.
- CommonGuard Cases Verified: 35.
- ShieldGrid Defense Hours: 120.
- Open-Source Contributions: 84 accepted contributions.

### Portable Reputation Module

The Portable Reputation Module converts verified activity and credentials into portable reputation signals.

Capabilities include:

- User-controlled reputation profiles.
- Contribution-based reputation.
- Credential-based reputation.
- Weighted contribution scoring.
- Reputation levels.
- Reputation categories.
- Domain-specific reputation.
- Reputation freshness.
- Reputation decay.
- Reputation history.
- Reputation provenance.
- Reputation signal aggregation.
- Cross-platform reputation portability.
- Community-specific reputation models.
- Opt-in public reputation profiles.
- Private reputation profiles.
- Pseudonymous reputation profiles.
- Reputation export and import.
- Reputation verification without unnecessary identity disclosure.

Reputation must be explainable and traceable to verifiable evidence rather than functioning as an opaque popularity score.

### Selective Disclosure and Privacy Module

The Selective Disclosure and Privacy Module protects users while allowing them to prove relevant claims.

Capabilities include:

- Selective credential disclosure.
- Selective reputation disclosure.
- Zero-knowledge proofs.
- Anonymous credential presentation.
- Threshold proofs.
- Range proofs.
- Attribute proofs.
- Age or qualification verification without unnecessary personal information.
- Reputation-level verification without revealing complete history.
- Pseudonymous participation.
- Context-specific identifiers.
- Identity compartmentalization.
- Credential minimization.
- Metadata minimization.
- Privacy-preserving verification.

Examples include proving that a participant has reached Contributor Level 5 without revealing their name, location, complete credential history, or individual contributions.

### Anti-Doxxing Module

The Anti-Doxxing Module provides protections against unnecessary exposure of personal identity and sensitive information.

Capabilities include:

- Separation of real-world identity from public reputation.
- Pseudonymous credentials.
- Rotating identifiers.
- Context-specific identities.
- Private contact information.
- Hidden location information.
- Minimal disclosure defaults.
- Protection against credential correlation.
- Protection against reputation correlation.
- Privacy-preserving public profiles.
- User-controlled identity revelation.
- Emergency identity disclosure controls where explicitly authorized.
- Metadata minimization.
- Protection against accidental identity linking.

PeopleLayer must treat identity exposure as a security event rather than a default feature.

### Federated Trust Registry Module

The Federated Trust Registry Module enables independent communities to exchange trust signals without requiring one centralized authority.

Capabilities include:

- Federated trust registries.
- Peer-to-peer trust exchange.
- Community-operated registries.
- Distributed credential discovery.
- Trust issuer discovery.
- Reputation signal exchange.
- Registry synchronization.
- Registry federation.
- Community-specific trust policies.
- Trust issuer allowlists and denylists.
- Credential status synchronization.
- Offline-capable verification.
- Conflict detection between trust sources.
- Multiple independent trust authorities.

No single registry should be required to determine whether a credential or reputation signal is valid.

### Human Steward Module

The Human Steward Module connects people, communities, and trusted stewards.

Capabilities include:

- Steward verification.
- Steward-issued credentials.
- Human contribution validation.
- Community verification.
- Peer attestations.
- Steward reputation.
- Steward delegation.
- Multi-steward verification.
- Steward revocation.
- Dispute escalation.
- Human review of automated decisions.
- Community-specific stewardship policies.

Steward relationships must remain transparent, revocable, and subject to user consent.

### Human-Agent Link Module

The Human-Agent Link Module connects human identities with authorized AI agents.

Capabilities include:

- Agent identity registration.
- Human ownership or stewardship relationships.
- Agent authorization.
- Agent activity attribution.
- Agent contribution credentials.
- Human-earned reputation from authorized agent activity.
- Agent-earned trust from human stewardship.
- Delegated authority.
- Agent permission scopes.
- Agent action logs.
- Human review of consequential agent activity.
- Revocation of agent authority.
- Separation of human reputation from unauthorized agent activity.

The system must distinguish between actions performed directly by a human and actions performed by an agent acting under delegated authority.

### Integration Module

The Integration Module provides standardized interfaces for connecting PeopleLayer to external applications.

Capabilities include:

- REST APIs.
- Event-driven integration.
- Credential issuance hooks.
- Credential verification hooks.
- Reputation verification hooks.
- Contribution event hooks.
- Webhooks.
- CLI integration.
- SDK support.
- Authentication interfaces.
- Authorization interfaces.
- Identity discovery.
- Credential exchange.
- Reputation exchange.
- Automated contribution recording.

Example integrations include:

- Automatically issuing a credential when a CommonGuard case is verified.
- Recording verified ShieldGrid defense hours.
- Recording VoteInsight election observation contributions.
- Issuing credentials for accepted open-source contributions.
- Recording verified community service.
- Connecting external applications to user-controlled reputation.

### Contribution Tracking Module

The Contribution Tracking Module records verifiable activity that can contribute to credentials and reputation.

Capabilities include:

- Contribution records.
- Contribution timestamps.
- Contribution provenance.
- Contribution verification.
- Contribution categories.
- Contribution impact measurements.
- Contribution effort measurements.
- Contribution attestations.
- Contribution aggregation.
- Duplicate detection.
- Fraud detection.
- Contribution disputes.
- Contribution corrections.
- Contribution withdrawal.
- Contribution history export.

Contribution tracking must distinguish between claims, attestations, and independently verifiable evidence.

### Reputation Scoring Module

The Reputation Scoring Module provides configurable methods for calculating reputation.

Capabilities include:

- Weighted scoring.
- Category-specific scoring.
- Community-specific scoring.
- Contribution impact weighting.
- Contribution difficulty weighting.
- Verification strength weighting.
- Recency weighting.
- Reputation decay.
- Reputation recovery.
- Reputation thresholds.
- Reputation levels.
- Confidence scores.
- Evidence strength indicators.
- Transparent scoring rules.
- User-visible scoring explanations.
- Multiple simultaneous reputation models.

PeopleLayer must not require one universal reputation score. Communities should be able to define their own trust models.

### Endorsement Module

The Endorsement Module enables people and trusted entities to attest to contributions.

Capabilities include:

- Peer endorsements.
- Organizational endorsements.
- Steward endorsements.
- Credential-backed endorsements.
- Endorsement expiration.
- Endorsement revocation.
- Endorsement weighting.
- Endorsement provenance.
- Endorsement verification.
- Anti-manipulation controls.

Endorsements should supplement verifiable evidence rather than replace it.

### Governance and Dispute Module

The Governance and Dispute Module provides mechanisms for handling contested credentials, reputation signals, and trust relationships.

Capabilities include:

- Credential disputes.
- Reputation disputes.
- Evidence submission.
- Peer review.
- Steward review.
- Appeal processes.
- Credential suspension.
- Credential revocation.
- Reputation corrections.
- False-claim reporting.
- Fraud investigations.
- Community-specific governance policies.
- Transparent dispute records.
- Privacy-preserving dispute handling.

### Security Module

The Security Module protects identity, credentials, reputation, integrations, and network communications.

Capabilities include:

- Cryptographic key protection.
- Secure local storage.
- Encryption.
- Key rotation.
- Key revocation.
- Credential signature validation.
- Replay protection.
- Authentication.
- Authorization.
- Secure synchronization.
- Secure federation.
- Hardware-backed security.
- Multi-factor authorization.
- Threat detection.
- Suspicious activity detection.
- Audit logging.
- Security event reporting.

Private keys, recovery secrets, and sensitive credentials must never be transmitted or stored in plaintext.

### Recovery and Continuity Module

The Recovery and Continuity Module allows users to recover access without surrendering control to a centralized provider.

Capabilities include:

- Encrypted wallet backups.
- Recovery phrases.
- Hardware-assisted recovery.
- Social recovery.
- Multi-party recovery.
- Recovery guardians.
- Credential restoration.
- Identity rotation after compromise.
- Key compromise response.
- Emergency identity suspension.
- Device migration.
- Secure wallet export.

Recovery mechanisms must minimize opportunities for unauthorized identity takeover.

### Analytics Module

The Analytics Module provides users and participating communities with insight into contributions and trust activity.

Capabilities include:

- Personal contribution analytics.
- Reputation history.
- Credential history.
- Contribution trends.
- Skill development tracking.
- Community participation metrics.
- Trust network analysis.
- Credential usage metrics.
- Reputation freshness indicators.
- Verification statistics.
- Community health indicators.

Analytics must respect the privacy settings and disclosure preferences established by users and communities.

### Accessibility and Localization Module

The Accessibility and Localization Module ensures that PeopleLayer can be used by people with different technical abilities, languages, and accessibility requirements.

Capabilities include:

- Accessible interfaces.
- Keyboard navigation.
- Screen reader compatibility.
- High contrast support.
- Plain-language interfaces.
- Multilingual interfaces.
- Localized credential descriptions.
- Localized reputation terminology.
- Mobile-friendly interfaces.
- Low-bandwidth operation.
- Offline-capable workflows.

### Interoperability Module

The Interoperability Module defines how PeopleLayer implementations communicate with external identity, credential, reputation, and trust systems.

Capabilities include:

- DID interoperability.
- Verifiable credential interoperability.
- Anonymous credential interoperability.
- Zero-knowledge proof interoperability.
- Credential schema interoperability.
- Reputation schema interoperability.
- Identity portability.
- Credential portability.
- Reputation portability.
- Import and export interfaces.
- Protocol versioning.
- Compatibility negotiation.

Implementations should prefer established open standards where appropriate and avoid unnecessary proprietary dependencies.

## Optional Plugin Modules

PeopleLayer supports optional plugins that extend functionality without requiring those capabilities in the core implementation.

### Blockchain Anchoring Plugin

Provides optional blockchain-based anchoring for:

- Credential hashes.
- Registry checkpoints.
- Reputation snapshots.
- Timestamp proofs.
- Public verification records.

Blockchain use must remain optional and must not be required for core identity, credentials, reputation, or privacy functions.

### Hardware Wallet Plugin

Provides integration with compatible hardware security devices for:

- DID keys.
- Signing keys.
- Credential issuance.
- Credential presentation.
- Recovery operations.

### Mobile Wallet Plugin

Provides native mobile interfaces for:

- Identity management.
- Credential storage.
- Credential presentation.
- Reputation viewing.
- Selective disclosure.
- Secure notifications.

### Browser Plugin

Provides browser-based access to PeopleLayer functionality.

Capabilities include:

- Identity-aware websites.
- Credential presentation.
- Reputation verification.
- Selective disclosure.
- Website trust indicators.
- Permission management.

### Open Source Contribution Plugin

Connects PeopleLayer to open-source development platforms.

Capabilities include:

- Contribution verification.
- Commit verification.
- Merge request verification.
- Issue resolution credentials.
- Documentation contribution credentials.
- Maintainer attestations.
- Project participation credentials.

### Civic Participation Plugin

Provides credentialing for verified civic activities.

Capabilities include:

- Election observation.
- Public meeting participation.
- Community organizing.
- Public records research.
- Civic monitoring.
- Verified volunteer activities.
- Community service.

### Security Contribution Plugin

Provides credentials for verified security contributions.

Capabilities include:

- Security research.
- Vulnerability reporting.
- Defensive activity.
- Incident response.
- Threat analysis.
- Security testing.
- Verified defense hours.

### AI Agent Plugin

Provides integration with AI agent systems.

Capabilities include:

- Agent registration.
- Agent credentials.
- Agent reputation.
- Human-agent authorization.
- Agent contribution tracking.
- Agent action provenance.
- Human approval workflows.
- Agent trust verification.

### CivicTrust Plugin

Provides integration with CivicTrust and compatible agent trust infrastructure.

Capabilities include:

- Human steward relationships.
- Agent trust signals.
- Contribution exchange.
- Steward credentials.
- Human-agent reputation relationships.

### VoteInsight Plugin

Provides integration with VoteInsight.

Capabilities include:

- Election observer credentials.
- Precinct audit records.
- Election verification contributions.
- Civic research credentials.
- Verified observation history.

### ShieldGrid Plugin

Provides integration with ShieldGrid.

Capabilities include:

- Defense activity records.
- Security contribution credentials.
- Verified defense hours.
- Incident response credentials.
- Security reputation signals.

### CommonGuard Plugin

Provides integration with CommonGuard.

Capabilities include:

- Case completion credentials.
- Verified issue resolution.
- Contribution records.
- Community protection credentials.
- Case-based reputation signals.

### Reputation Marketplace Plugin

Provides optional discovery of communities and applications that accept PeopleLayer credentials or reputation signals.

Capabilities include:

- Credential acceptance discovery.
- Reputation model discovery.
- Community discovery.
- Skill matching.
- Contribution opportunities.
- Trust policy discovery.

The plugin must not sell or transfer ownership of a user's identity or reputation.

### Schema Marketplace Plugin

Provides optional discovery and publication of community-defined schemas for:

- Credentials.
- Contributions.
- Reputation signals.
- Trust policies.
- Steward roles.
- Agent roles.

### Collaboration Matching Plugin

Uses verified credentials and user-approved reputation information to identify potential:

- Collaborators.
- Volunteers.
- Researchers.
- Maintainers.
- Stewards.
- Civic participants.
- Security contributors.
- Community members.

Matching must respect user privacy and disclosure preferences.

### Gamification Plugin

Provides optional reputation-oriented features including:

- Levels.
- Badges.
- Achievement systems.
- Contribution streaks.
- Community challenges.
- Opt-in leaderboards.
- Anonymous rankings.

Gamification must remain optional and must not determine a user's underlying identity or access to essential functionality.

### AI Reputation Auditor Plugin

Provides automated analysis for:

- Duplicate contributions.
- Suspicious activity.
- Credential anomalies.
- Reputation manipulation.
- Coordinated abuse.
- Fraud indicators.
- Conflicting trust signals.

AI-generated findings must be treated as signals for review rather than automatic proof of misconduct.

### Analytics Dashboard Plugin

Provides advanced visualization for:

- Contribution history.
- Reputation changes.
- Credential activity.
- Trust relationships.
- Community participation.
- Verification activity.
- Credential adoption.

### Federation Gateway Plugin

Provides compatibility with external federated networks and trust registries.

Capabilities include:

- Registry discovery.
- Trust signal exchange.
- Credential synchronization.
- Federation policy management.
- Peer authentication.
- Conflict resolution.

## Privacy Requirements

PeopleLayer implementations must follow privacy-first principles.

The system should:

- Collect the minimum information necessary.
- Keep sensitive information under user control.
- Avoid unnecessary centralized identity databases.
- Separate identity from reputation where possible.
- Support pseudonymous operation.
- Support selective disclosure.
- Minimize metadata.
- Provide explicit consent controls.
- Make disclosure understandable to users.
- Prevent silent identity correlation.
- Provide mechanisms for credential revocation.
- Provide mechanisms for identity rotation.
- Protect private keys.
- Avoid exposing location information by default.

## Security Requirements

PeopleLayer implementations must:

- Use modern cryptographic primitives.
- Protect private keys from unauthorized access.
- Validate credential signatures.
- Validate credential status.
- Protect against replay attacks.
- Protect against credential forgery.
- Protect against unauthorized reputation modification.
- Protect synchronization channels.
- Provide secure recovery mechanisms.
- Provide clear security boundaries between plugins.
- Log security events without unnecessarily exposing sensitive information.
- Treat compromised identities and credentials as revocable security objects.

## Reputation Principles

PeopleLayer reputation must follow these principles:

- Reputation belongs to the user.
- Reputation must be based on verifiable evidence where possible.
- Reputation must be explainable.
- Reputation should distinguish verified facts from opinions.
- Reputation should distinguish contribution quantity from contribution quality.
- Reputation should account for freshness.
- Reputation should allow correction and dispute.
- Reputation should not be permanently defined by a single mistake.
- Communities may define independent reputation models.
- Users must control which reputation information they disclose.
- Reputation must not become a centralized social credit system.

## Credential Principles

Credentials should:

- Identify their issuer.
- Identify their subject without unnecessary personal information.
- Define their claims clearly.
- Include provenance.
- Support expiration where appropriate.
- Support revocation where appropriate.
- Support verification.
- Support selective disclosure where technically possible.
- Be portable across compatible implementations.
- Avoid unnecessary personally identifiable information.

## Integration Principles

External applications integrating with PeopleLayer should:

- Request only necessary permissions.
- Respect user disclosure settings.
- Avoid creating hidden identity dependencies.
- Preserve credential provenance.
- Preserve reputation provenance.
- Clearly identify credential issuers.
- Clearly identify trust sources.
- Support credential revocation.
- Support user-controlled disconnects.
- Avoid locking users into a single platform.

## Governance Principles

PeopleLayer is designed to support pluralistic trust rather than a single universal authority.

Communities may establish their own:

- Credential issuers.
- Reputation models.
- Steward requirements.
- Verification standards.
- Dispute procedures.
- Trust policies.
- Contribution definitions.
- Membership rules.

Users must remain able to determine which communities, issuers, applications, and trust sources they recognize.

## Interoperability Requirements

A conforming implementation should provide interoperable mechanisms for:

- Identity creation.
- Identity verification.
- Credential issuance.
- Credential presentation.
- Credential verification.
- Credential revocation.
- Selective disclosure.
- Reputation exchange.
- Trust registry exchange.
- Plugin integration.
- Data export.
- Data portability.

Implementations should document protocol versions and compatibility requirements.

## Human Oversight

PeopleLayer supports automation but does not require automated decisions to be final.

High-impact actions should support human review, including:

- Credential revocation.
- Reputation penalties.
- Identity suspension.
- Trust registry disputes.
- Fraud determinations.
- Steward removal.
- Agent authority changes.

Automated systems should provide evidence and reasoning signals that authorized humans can review.

## Ethical Requirements

PeopleLayer must not be designed as a universal social ranking system.

Implementations should prevent:

- Hidden reputation scoring.
- Mandatory public reputation.
- Permanent punishment for ordinary mistakes.
- Unconsented identity exposure.
- Unconsented reputation sharing.
- Centralized control over all trust decisions.
- Discrimination based on irrelevant personal information.
- Reputation manipulation through artificial activity.
- Automated blacklisting without review.

## Conformance

An implementation conforms to the PeopleLayer specification when it implements the required core modules appropriate to its deployment profile and follows the identity, credential, privacy, security, interoperability, and governance principles defined by this specification.

Optional plugins may extend functionality without being required for base conformance.

Conforming implementations should document:

- Supported identity methods.
- Supported credential formats.
- Supported privacy mechanisms.
- Supported reputation models.
- Supported federation protocols.
- Supported plugins.
- Supported interoperability standards.
- Security assumptions.
- Recovery mechanisms.

## Development Principles

PeopleLayer development should prioritize:

- Open-source implementation.
- Local-first operation.
- User sovereignty.
- Privacy by design.
- Security by design.
- Interoperability.
- Modularity.
- Transparency.
- Human oversight.
- Community governance.
- Vendor independence.
- Long-term portability.

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
  - [https://roxanneardary.com/peoplelayer/](https://roxanneardary.com/peoplelayer/)

---

## License & Notice Requirements

PeopleLayer is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PeopleLayer specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  

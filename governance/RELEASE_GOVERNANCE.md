# Release Governance Policy

## Purpose
This policy governs the creation, validation, and publication of official releases of this repository.

It ensures that each release represents a stable, auditable, and trustworthy snapshot of regulatory data.

## Release Authority
Only repository maintainers may:
- Approve releases
- Tag versions
- Modify `latest.json`
- Freeze schema versions

## Pre-Release Validation
Before any release is tagged, all checks in the Release Validation Checklist must pass, including:

### Structural Validation
- JSON validates against the locked schema
- Required fields are present
- No extraneous keys exist

### Temporal Validation
- publication_date does not exceed the release cutoff
- latest.json points to the most recent qualifying instrument
- archive entries remain immutable

### Source Integrity
- official_url resolves to an authoritative government source
- source field is explicitly declared
- No scraped or inferred content is included

### Jurisdiction Validation
- All entries belong to the repository’s jurisdiction
- Devolved instruments are clearly labeled
- Cross-jurisdictional instruments are excluded unless retained in law

### Semantic Validation
- Relevance flags are conservatively applied
- False positives are documented
- No record is removed solely due to uncertainty

## Versioning
- Semantic versioning (v1.0, v1.1, v2.0)
- v1.0 represents schema freeze

## Versioning Rules
- Major versions (e.g. v1.0) represent frozen snapshots
- Schema changes require a major version increment
- Minor updates may add data without schema changes
- Patch updates may correct metadata errors only

## Freeze Semantics
When a version is marked as “Frozen”:
- Schema is locked
- Archive data is immutable
- Historical records will not be altered
- Only new releases may introduce additional data

## Release Tagging
Releases are tagged using Git tags (e.g. v1.0).
Each release must include:
- A changelog entry
- A declared schema version
- A release date
- A frozen status indicator
- Git tag applied at repository root
- CHANGELOG updated

## Post-Release Handling
After release:
- latest.json may move forward in future versions
- archive.json remains preserved
- Prior versions remain accessible indefinitely

## Release Conditions
- Validation checklist must pass
- Schema lock must not be violated
- Sources must be verified

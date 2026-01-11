# Schema Lock Declaration
## Schema Lock Declaration (v1.0)

### Purpose
This declaration formally establishes the locked metadata schema used by this repository for regulatory and legislative records.

From the point of release tagging v1.0, the schema defined herein is considered frozen and authoritative.
No backward-incompatible changes may be introduced without a major version increment.

This lock ensures:
- Structural stability for downstream users
- Deterministic parsing and validation
- Long-term reproducibility of regulatory datasets
- Cross-jurisdictional consistency between US, UK, and EU repositories

### Scope
This schema applies to all JSON records published in this repository, including but not limited to:
- latest.json
- All files under archives/
- Any future time-series or batch exports

The schema governs metadata only and does not apply to:
- Source documents hosted externally
- Linked legislative or regulatory texts
- Jurisdiction-specific legal instruments themselves

### Locked Fields (Canonical)
- The following top-level JSON fields are mandatory and fixed in name and semantic meaning:
- title
- jurisdiction
- document_type
- year
- publication_date
- last_updated
- source_agency
- summary
- relevance_to_digital
- relevance_to_data
- relevance_to_ai
- official_url
- source

Field presence is mandatory.
Nullable values are permitted only where explicitly defined by the schema.

No additional top-level fields are allowed.

### Data Type Guarantees
- Dates MUST be ISO-8601 compliant (YYYY-MM-DD or full timestamp where available)
- Boolean relevance indicators MUST be expressed as descriptive strings, not raw booleans
- URLs MUST resolve to authoritative, official sources
- jurisdiction MUST match the repository scope exactly

### Immutability Rules
- Entries committed to archives/ are immutable
- Historical records MUST NOT be altered, removed, or reclassified
- Corrections require the addition of a new record with a later timestamp
latest.json MUST always reference the most recent qualifying record under the validation rules.

### Change Control
The locked schema MAY ONLY be modified if:
1. A breaking change is unavoidable
2. A new major version is declared (e.g. v2.0)
3. The change is documented in:
  - A new Schema Lock Declaration
  - A migration guide
  - Release notes

Minor and patch releases MUST NOT alter schema structure or field semantics.

### Jurisdictional Consistency
This schema is identical across US, UK, and EU repositories.

Jurisdictional differences are expressed only through values, never structure.

This guarantees:
- Cross-region compatibility
- Unified tooling
- Shared validation logic

### Licensing and Use

This schema, its structure, and its documentation are original works released under the repository license (MIT).

The schema governs only metadata and derived summaries.
Underlying regulatory texts remain subject to their issuing authorities.

### Effective Date

This schema lock is effective as of:

Release: v1.0

Date: 12th January 2026

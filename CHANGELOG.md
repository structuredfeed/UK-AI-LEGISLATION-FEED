# CHANGELOG
## v1.0 — Initial Unified Release

### Status

#### Frozen / Locked
This release establishes the first stable, production-ready version of the regulatory metadata repositories for the United States, United Kingdom, and European Union.

### Scope of Release
This release includes:
- Fully validated regulatory metadata records
- Locked and unified JSON schema across all jurisdictions
- Authoritative source attribution
- Conservative AI / Digital / Data relevance classification
- Immutable archival records
- Explicit licensing and reuse boundaries

### Included Jurisdictions
- United States
- United Kingdom
- European Union

All three jurisdictions use:
- The same schema
- The same validation rules
- The same versioning and immutability guarantees

Jurisdictional differences are expressed only in field values, never structure.

### Schema Governance
- Schema frozen under SCHEMA_LOCK.md
- No new fields permitted without a major version bump
- No backward-incompatible changes permitted in v1.x
- Archives are immutable once committed
- latest.json always points to the most recent qualifying instrument

### Source Integrity
All records in this release:
- Originate from official, authoritative public-sector sources only
- Use publisher-provided APIs, feeds, or structured endpoints
- Do not rely on scraping, mirroring, or derived-only datasets
- Include a resolvable official_url

### Jurisdictional Source Notes
- US: Public-domain federal sources (e.g. Congress, Federal Register)
- UK: Open Government Licence v3.0 sources (e.g. legislation.gov.uk, GOV.UK, ICO, CMA)
- EU: European Union legislative sources reused under the EU Open Data Directive and EUR-Lex reuse policy

Only metadata, summaries, and links are distributed.

### Licensing & Compatibility
- Repository code, schemas, and metadata structures are licensed under MIT
- Public-domain and open-government materials are used in compliance with:
  - US public-domain doctrine
  - Open Government Licence v3.0 (UK)
  - EU Open Data Directive and EUR-Lex reuse policy

No full legislative texts are redistributed where reuse restrictions apply.

### Validation Guarantees
All records in v1.0 have passed:
- Structural validation against the locked schema
- Temporal validation (publication dates ≤ release cutoff)
- Jurisdictional validation
- Source integrity checks
- Conservative semantic tagging review

False positives are documented, not deleted.

### What Is Explicitly Out of Scope
This release does not include:
- Automated scraping
- Full-text redistribution of legislation
- Legal interpretation or advice
- Predictive or probabilistic AI analysis
- Post-v1.0 amendments or live updates

### Change Policy Going Forward
- v1.x: Data additions only (schema unchanged)
- v2.0: Schema changes only with migration documentation
- Historical records will never be rewritten

### Release Freeze
As of this release:
- US v1.0 — Frozen
- UK v1.0 — Frozen
- EU v1.0 — Frozen

Any future updates will occur under a new version tag.

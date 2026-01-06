# Data Governance Policy

## Purpose
This policy governs the ingestion, handling, validation, and preservation of data within this repository.

Its objective is to ensure that all data remains authoritative, legally compliant, jurisdictionally correct, and suitable for automated and commercial use.

## Scope
This policy applies to:
- All contributors
- All maintainers
- All data added to `latest.json` and `archive.json`
- All jurisdictions covered by this repository

## Principles
- Accuracy
- Source fidelity
- Immutability of historical records
- Conservative classification

## Source Control
- Only official government sources are permitted
- No scraping
- No unofficial mirrors

## Data Integrity
- Records are immutable once archived
- Corrections result in new entries, not overwrites

## Auditability
- Each record links to its authoritative source
- Versioned releases provide point-in-time snapshots

## Authoritative Sources Only
Only data derived from official public-sector sources may be included.

Permitted sources include:
- Official legislative publishers
- Government regulatory bodies
- Statutory repositories
- Official APIs, RSS feeds, and XML endpoints

Prohibited sources include:
- Scraped websites
- Secondary aggregators
- Blogs, commentary, or analysis sites
- AI-generated legal interpretations

## Data Types Permitted
This repository may include:
- Metadata
- Titles
- Dates
- Issuing authorities
- Short factual summaries
- Classification indicators
- Official source URLs

This repository must NOT include:
- Full legislative or regulatory texts
- Copyrighted commentary
- Judicial opinions (unless explicitly within scope)
- Legal interpretations or advice

## Jurisdictional Integrity
Each repository is jurisdiction-specific.

Rules:
- All entries must belong to the repository’s jurisdiction
- Devolved or retained instruments must be clearly labeled
- Cross-jurisdictional instruments are excluded unless officially incorporated

## Metadata Fidelity
- Metadata must reflect the authoritative source exactly
- Missing or incomplete fields must remain null
- Data must not be inferred or filled speculatively
- Corrections may only be applied using official updates

## Relevance Classification
Relevance flags (AI / Digital / Data):
- Must be applied conservatively
- Are informational only
- Do not imply legal interpretation
- May include documented false positives

## Immutability
Once published to `archive.json`:
- Records are immutable
- No deletions are permitted
- Corrections require a new entry or documented exception

## Accountability
All changes must be traceable via version control.
Contributors are responsible for verifying source authenticity and compliance.

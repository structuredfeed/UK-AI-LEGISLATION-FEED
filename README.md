# Machine Readable AI Legislation Feed (UK)

This repository provides a machine-readable feed of UK legislation and regulatory signals relevant to artificial intelligence (AI).

## Purpose
The goal of this project is to make it easier for developers, researchers, and organizations to monitor official UK legal and regulatory developments related to AI in a structured, automated way.

## Product Packaging

This repository represents a jurisdiction-specific SKU within a multi-region AI regulatory dataset.

Each SKU conforms to the same locked schema and governance model, enabling seamless combination across regions.

## Scope
This repository includes:
- Acts of Parliament
- Statutory Instruments
- Official regulatory notices and guidance

Only AI-relevant items are included.

## Data Structure
- `data/latest.json` — the most recent UK AI-related legislative or regulatory item
- `data/archive.json` — historical archive of all accepted items

## Data Sources
See `sources/uk_sources.md` for a full list of official sources.

## Schema Governance

This repository uses a locked metadata schema.
The schema is frozen as of v1.0 and governed by the Schema Lock Declaration.

See: `SCHEMA_LOCK.md`


## Versioning & Data Scope
This repository follows a rolling release model.
- Version identifiers (e.g. v1.0) represent a stable snapshot of all qualifying regulatory instruments available at the time of release.
- The latest.json file points to the most recently published qualifying instrument at build time.
- The archive/ directory contains all previously indexed instruments preserved immutably.

## Inclusion Criteria
This dataset includes:
- Primary legislation (Acts)
- Secondary legislation (e.g. Regulations, Statutory Instruments)
- Official amendments and commencement instruments where applicable
- Devolved or federal equivalents where within scope (e.g. Welsh Statutory Instruments)

## Metadata Completeness
- Some official sources publish legislation with partial metadata (e.g. missing titles or summaries at time of publication).
- Such records are included unaltered to preserve fidelity with the authoritative source.
- Metadata completeness may improve in later versions without altering historical records.

## AI, Data, and Digital Relevance Flags
- Relevance indicators are generated using conservative classification rules.
- Flags may include false positives where legislation references automation, systems, or electronic processes without explicitly regulating artificial intelligence.
- These indicators are informational only and do not constitute legal interpretation.

## Jurisdictional Integrity
- Each repository is jurisdiction-specific.
- Cross-jurisdictional instruments are indexed only where they are officially incorporated or retained within the relevant legal framework.

## Methodology
Items are sourced exclusively from official UK government publications.  
Only titles, publication dates, issuing bodies, short summaries, and source URLs are stored.

Full legal texts are not redistributed.

## Legal Notice
This repository does not provide legal advice.  
All content is provided for informational purposes only.

## Update Frequency
Updates are performed automatically when new relevant regulatory signals are detected.
If no qualifying updates are published, no changes are made.

## Intended Use
This feed is intended for:
- Regulatory monitoring
- Internal policy tracking
- Risk awareness
- Research and analysis
- Automation and tooling

Users are responsible for determining how the information is used within their own compliance or decision-making processes.

## Compatibility Statement
This repository aggregates metadata derived from official public-sector sources.
- US sources: US Government works, public domain
- UK sources: Crown copyright, Open Government Licence v3.0
- EU sources: © European Union, reused under the EU Open Data Directive and EUR-Lex reuse policy

Public Domain content is fully compatible with the MIT License.
Open Government Licence v3.0 and EU Open Data licences are permissive and MIT-compatible when:
- Attribution is preserved
- No endorsement is implied

This repository:
- Does not redistribute full legislative, regulatory, or copyrighted text where restrictions apply
- Provides metadata, summaries, and links only
- Is compatible with MIT / Apache-2.0 / CC-BY-4.0 downstream use
Users are responsible for verifying downstream reuse requirements of linked source material.

## Repository License

This repository is licensed under the MIT License.

The MIT License applies only to:
- Original code
- Original JSON structures
- Metadata schemas
- Generated prompts and classification logic

This repository provides a licensed structured representation of public information.
Underlying regulatory and legislative texts remain governed by their respective issuing authorities.

## Disclaimer
This feed is provided "as is" without warranties of any kind.
No liability is assumed for errors, omissions, or interpretations.
Users should consult qualified legal professionals for regulatory or compliance advice.

## Current Release
- Version: v1.0
- Status: Frozen

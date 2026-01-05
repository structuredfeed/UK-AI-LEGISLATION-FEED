# Methodology

## Overview
This project provides structured regulatory intelligence by aggregating metadata from official public-sector sources related to artificial intelligence, digital systems, and data governance.

The objective is to improve accessibility, monitoring, and automation—not to interpret or enforce law.

## Source Selection
Only authoritative government sources are used, including:
- Official legislation repositories
- Government regulatory bodies
- Statutory publishers
- Official RSS and API endpoints

No scraping, inference, or third-party aggregation is performed.

## Data Capture
For each qualifying instrument, we record:
- Title (as published)
- Jurisdiction
- Document type
- Publication and update dates
- Issuing authority (where available)
- Official source URL
- Short, non-interpretive summary
- Relevance indicators (AI / digital / data)

Full legal texts are never redistributed.

## Inclusion Criteria
Items are included when they:
- Are official legislative or regulatory instruments
- Originate from authoritative publishers
- Contain direct or indirect relevance to AI, digital systems, or data governance

## Relevance Classification
Relevance flags are applied conservatively:
- AI: Explicit references to artificial intelligence or automated decision-making
- Digital: References to electronic systems, online services, or digital infrastructure
- Data: References to data processing, access, sharing, or governance

False positives are tolerated and documented; exclusions are minimized.

## Versioning & Integrity
- Each release represents a stable snapshot
- Historical records are immutable
- Schema changes require major version updates
- Latest pointers reflect the most recent qualifying publication

## Limitations
This dataset:
- Does not provide legal interpretation
- Does not guarantee regulatory completeness
- Should be used as a monitoring and awareness tool

Users should consult qualified professionals for compliance decisions.

# Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)  
**Community Policy & Volunteer Guide**  

**Version 1.0 (Draft)**  
**Last updated:** April 2026  
**Project repository:** https://github.com/MLDCHA (placeholder – to be created by core team)  
**License:** CC-BY-SA 4.0 for documentation & data; MIT for code  

---

## 1. Introduction & Project Scope

The **Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)** is an open, volunteer-driven platform that harvests, integrates, enriches, and redistributes cultural heritage data from Galleries, Libraries, Archives, and Museums (GLAM institutions) worldwide.  

Our **core output** is a massive, living collection of **multi-part IIIF (International Image Interoperability Framework) Collections and Manifests**, organized by curated subject categories. Every manifest is automatically reconciled against the following authoritative vocabularies:

- **AAT** – Getty Art & Architecture Thesaurus  
- **TGN** – Getty Thesaurus of Geographic Names  
- **LCSH** – Library of Congress Subject Headings  
- **LCTGM** – Library of Congress Thesaurus for Graphic Materials  
- **Wikidata** – for additional global identifiers and multilingual labels  

The entire system is built as a **public GitHub-first community** with transparent governance, version-controlled workflows, and **crowdfunding integrated directly through GitHub Sponsors, GitHub Discussions, and issue-level sponsorships**. No central institution owns the data; the community collectively stewards it.

**Key principles**  
- Open standards only (IIIF, RDF, OWL, SHACL, Linked Open Data)  
- Radical interoperability and reusability  
- Ethical sourcing and respect for source institutions’ rights  
- Merit-based contribution (skills > credentials)  
- Full transparency via Git history  

---

## 2. Mission & Vision

**Mission**  
To democratize access to cultural heritage by creating the largest open, semantically rich, IIIF-native aggregator maintained by a global volunteer community.

**Vision**  
A single, freely queryable IIIF “super-collection” containing millions of reconciled digital objects, grouped into thematic sub-collections (e.g., “Islamic Manuscript Traditions”, “Industrial Revolution Visual Culture”, “Indigenous Art of Oceania”), ready for researchers, educators, artists, and GLAM institutions to reuse instantly.

---

## 3. Community Structure & Roles

All work happens in the public GitHub organization. Everyone uses Git, GitHub Issues, Projects, Discussions, and Pull Requests.

| Role | Primary Responsibilities | Required Skills | Time Commitment |
|------|---------------------------|-----------------|-----------------|
| **Document Creators / Content Contributors** | Write policy, tutorials, glossaries, metadata guidelines | Markdown, research, clear writing | Flexible (1–5 hrs/week) |
| **Session Moderators** | Run weekly community calls, onboarding sessions, hackathons | Zoom/Discord moderation, facilitation | 2–4 hrs/week |
| **Technical Staff – Harvesting Layer** | Build & maintain connectors for GLAM APIs | Python/Node.js, REST, IIIF API, web scraping (ethical), rate-limit handling | 5–15 hrs/week |
| **Data Science Experts** | RDF transformation, ontology mapping, SHACL validation, reconciliation pipelines | RDFlib/rdflib, OWL, SHACL, SPARQL, entity linking (Wikidata, AAT) | 5–12 hrs/week |
| **Software Developers** | Core platform code, IIIF manifest generation, enrichment services | Python/Django or FastAPI, IIIF libraries (iiif-prezi, manifester), Git | 5–15 hrs/week |
| **DevOps Experts** | CI/CD, containerization, scalable harvesting infrastructure, GitHub Actions | Docker, Kubernetes (optional), GitHub Actions, monitoring | 4–10 hrs/week |
| **General Volunteers / Reviewers** | Test connectors, review PRs, label issues, enrich sample data | Any of the above + enthusiasm | Flexible |

**Onboarding**  
1. Read this document  
2. Join the GitHub organization (request via Discussion #1)  
3. Complete the “Hello World” contribution (add your name to `VOLUNTEERS.md`)  

---

## 4. Technical Architecture – The Multi-Layered Model

The platform is deliberately separated into clear, Git-managed layers so volunteers can focus on their expertise.

### Layer 1: Harvesting & Connectors (Data Acquisition)
- **Goal**: Pull raw metadata and images from GLAM sources.  
- **Preferred sources** (in order):  
  1. IIIF Presentation API 2.0/3.0 compliant endpoints  
  2. RESTful APIs (Europeana, Digital Public Library of America, etc.)  
  3. OAI-PMH  
  4. Ethical web scraping (only when no API exists and robots.txt permits)  
- **Deliverables per connector**:  
  - Python module in `/connectors/`  
  - `README.md` with usage, rate limits, authentication notes  
  - GitHub Action workflow for periodic harvesting  
  - Sample harvested JSON-LD output  

### Layer 2: Integration & Enrichment (Semantic Layer)
- **Goal**: Convert everything into a unified RDF graph that is flexible across multiple OWL ontologies.  
- **Core technologies**:  
  - RDF (JSON-LD 1.1 preferred)  
  - Multiple OWL ontologies (CIDOC-CRM, EDM, BIBFRAME, Schema.org, plus custom extensions)  
  - **SHACL shapes** for validation and quality control  
- **Reconciliation pipeline** (mandatory):  
  1. Extract entities (persons, places, concepts, materials)  
  2. Reconcile against AAT, TGN, LCSH, LCTGM, Wikidata using automated + human-in-the-loop tools  
  3. Generate `skos:exactMatch`, `owl:sameAs`, `dcterms:conformsTo` statements  
- **Output**: Validated RDF graphs stored in `/data/enriched/`  

### Layer 3: IIIF Collection Assembly (Output Layer)
- **Goal**: Generate huge, categorized, multi-part IIIF Collections.  
- **Structure**:  
  - Top-level `collection.json` (the “super-collection”)  
  - Thematic sub-collections (e.g., `subject/islamic-art/collection.json`)  
  - Every manifest must contain reconciled metadata in `metadata[]` and `seeAlso` links to RDF graphs  
- **Automation**: GitHub Actions automatically regenerate collections when enriched data changes.  

---

## 5. Crowdfunding & Sustainability Model

The project runs **entirely through GitHub**:

- **GitHub Sponsors** at organization level  
- **Issue-level sponsorships** (label `💰 funded` – community votes on priorities)  
- **GitHub Discussions** for funding proposals and transparent budget reports  
- All funds are used only for:  
  - Cloud credits for harvesting infrastructure  
  - Domain & hosting  
  - Occasional bounties for complex connectors  
  - Legal advice on cultural heritage rights  

**Transparency rule**: Monthly financial summary published in `FINANCES.md`.

---

## 6. Volunteer Tasks & Contribution Workflow

### General Git Workflow (mandatory for all)
1. Fork → Branch (naming: `feature/connector-europeana`, `fix/shacl-validation`)  
2. Work in small, reviewable commits  
3. Open PR with checklist in template  
4. Request review from at least two people (one technical, one domain)  
5. Merge only after CI passes and SHACL validation is green  

### Role-Specific Task Examples

**Harvesting Team**  
- Create new connector for a IIIF-compliant museum  
- Write test suite that validates output against IIIF spec  
- Document any required API keys or scraping strategies  

**Data Science Team**  
- Map a new GLAM metadata schema to our RDF model  
- Write SHACL shapes for a new subject category  
- Run reconciliation campaigns (e.g., “Reconcile 10,000 place names to TGN”)  

**IIIF Assembly Team**  
- Curate new subject category (propose via issue)  
- Generate manifests with enriched metadata  
- Review collection thumbnails and navigation structure  

**Documentation Team**  
- Maintain `GLOSSARY.md` (IIIF, RDF, SHACL, AAT, etc.)  
- Write step-by-step tutorials for new volunteers  
- Translate key documents  

---

## 7. Code of Conduct & Ethics

- **Be kind, be constructive, assume best intent** (Contributor Covenant adopted)  
- **Respect source institutions**: Never harvest restricted content; always credit original providers  
- **Data sovereignty**: GLAMs retain copyright; we only aggregate public-domain or openly licensed material  
- **No commercial exploitation** without explicit community approval  
- **Diversity & inclusion**: We actively welcome volunteers from all geographies and backgrounds  

---

## 8. Tools & Technology Stack (Recommended)

- **Language**: Python 3.11+ (core), JavaScript/Node for front-end utilities  
- **RDF**: rdflib + pyshacl  
- **IIIF**: iiif-prezi3, loris/cantaloupe (optional)  
- **Version control**: Git + GitHub  
- **CI/CD**: GitHub Actions  
- **Ontology editing**: Protégé (optional)  
- **Communication**: GitHub Discussions + monthly community calls  

---

## 9. Getting Started – Your First Week

1. Star and fork the repo  
2. Read `CONTRIBUTING.md` and this policy  
3. Join the weekly onboarding call (link in Discussion #2)  
4. Claim your first issue (label `good-first-issue`)  
5. Introduce yourself in the `#introductions` Discussion  

---

## 10. Roadmap (High-Level)

**Phase 1 (0–3 months)**: Core connectors (Europeana, Getty, British Library, Smithsonian) + basic RDF pipeline  
**Phase 2 (3–9 months)**: SHACL validation suite + first 5 thematic IIIF collections  
**Phase 3 (9–18 months)**: Public API + community dashboard + 50+ connectors  
**Phase 4**: Integration with major IIIF viewers and Linked Open Data cloud  

---

**This document is living.**  
All changes must be proposed via Pull Request and approved by the current volunteer maintainers (elected every 6 months via GitHub poll).  

Welcome to the team!  
Together we are building the future of open cultural heritage.  

**— The MLDCHA Community**

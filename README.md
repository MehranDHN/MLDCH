```markdown
# Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)  
**Community Policy & Volunteer Guide**  

**Version 1.6 (Draft)**  
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
- Radical interoperability and reusability (FAIR principles)  
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
| **Document Creators / Content Contributors** | Write policy, tutorials, glossaries, metadata guidelines, educational content | Markdown, research, clear writing, cultural heritage knowledge | Flexible (1–5 hrs/week) |
| **Session Moderators** | Run weekly community calls, onboarding sessions, hackathons, community engagement | Facilitation, moderation, communication, inclusivity | 2–4 hrs/week |
| **Technical Staff – Harvesting Layer** | Build & maintain connectors for GLAM APIs | Python/Node.js, REST, IIIF API, web scraping (ethical), rate-limit handling | 5–15 hrs/week |
| **Data Science Experts** | RDF transformation, ontology mapping, SHACL validation, reconciliation pipelines | RDFlib/rdflib, OWL, SHACL, SPARQL, entity linking (Wikidata, AAT) | 5–12 hrs/week |
| **Software Developers** | Core platform code, IIIF manifest generation, enrichment services | Python/Django or FastAPI, IIIF libraries (iiif-prezi, manifester), Git | 5–15 hrs/week |
| **DevOps Experts** | CI/CD, containerization, scalable harvesting infrastructure, GitHub Actions | Docker, Kubernetes (optional), GitHub Actions, monitoring | 4–10 hrs/week |
| **General Volunteers / Reviewers** | Test connectors, review PRs, label issues, enrich sample data, curate themes | Any of the above + enthusiasm, attention to detail | Flexible |

**Humanities & Cultural Heritage Experts** (a cross-cutting group within Document Creators, Session Moderators, General Volunteers/Reviewers, and even some Data Science volunteers) bring deep domain knowledge in art history, museum curation, library science, archival studies, and related fields. Their collaboration with technical staff is essential for accurate ontologies, meaningful subject categories, and culturally sensitive data enrichment.

---

## 4. Volunteer Onboarding Checklist

Complete this checklist in your first 7–10 days to become a fully active community member. All steps are tracked via GitHub for transparency.

### Step 1: Preparation (Day 1)
- [ ] Read this entire **Community Policy & Volunteer Guide** (this document)
- [ ] Review `CODE_OF_CONDUCT.md` and `CONTRIBUTING.md` (will be created in repo)
- [ ] Create or update your GitHub profile with:
  - A clear display name and bio mentioning your skills/interests (e.g., “Python + RDF enthusiast | Cultural heritage volunteer”)
  - Link to your location/timezone if comfortable
- [ ] Install required tools:
  - Git
  - Python 3.11+
  - A good code editor (VS Code recommended with GitHub Copilot or extensions for Markdown/RDF)
  - Optional but helpful: Protégé (for ontology work), Postman/Insomnia (for API testing), OpenRefine (for reconciliation)

### Step 2: Join the Community (Day 1–2)
- [ ] Go to the main repository and click “Fork”
- [ ] Request to join the GitHub Organization via the pinned **Discussion #1 – “New Volunteer Onboarding”** (include your GitHub username and desired role)
- [ ] Introduce yourself in the **#introductions** Discussion thread:
  - Share your background, skills, why you joined, and any prior experience with Git, IIIF, RDF, or cultural heritage
  - Mention your availability (hours per week)
- [ ] Join any linked communication channels (e.g., GitHub Discussions, monthly Zoom calls – link in Discussion #2)

### Step 3: First Contribution – “Hello World” (Day 2–3)
- [ ] Add your name, GitHub handle, skills, and join date to `VOLUNTEERS.md` (create the file if it doesn’t exist) via a Pull Request
- [ ] Use the PR template and request review from at least one existing member
- [ ] Once merged, you are officially a listed volunteer!

### Step 4: Skill Assessment & First Task (Day 3–7)
- [ ] Browse the **Good First Issues** (label: `good-first-issue`) and claim one that matches your skills
  - Examples:
    - Documentation: Improve a README or glossary entry
    - Harvesting: Test an existing connector and report issues
    - Data: Manually reconcile 10 sample records against Wikidata/AAT using OpenRefine
    - General: Label or triage 5 open issues
- [ ] Work on your task in a new branch (`feature/your-task-name` or `docs/your-task-name`)
- [ ] Open a Pull Request with clear description and checklist
- [ ] Participate in at least one community call or Discussion thread to ask questions

### Step 5: Learning & Setup (Ongoing during onboarding)
- [ ] Complete the **Core Tutorials** (links will be in `TUTORIALS.md`):
  - Introduction to IIIF Manifests & Collections
  - Basic RDF and JSON-LD for Cultural Heritage
  - Our Reconciliation Pipeline (AAT/TGN/LCSH/Wikidata) with OpenRefine
  - SHACL Validation Basics
- [ ] Set up your local development environment:
  - Clone the repo
  - Run `setup.sh` or follow `DEVELOPMENT.md` to install dependencies
  - Run tests for at least one connector or the RDF pipeline
- [ ] Familiarize yourself with key directories:
  - `/connectors/` – Harvesting scripts
  - `/data/enriched/` – RDF outputs
  - `/iiif-collections/` – Generated IIIF files
  - `/ontology/` – OWL & SHACL shapes
  - `/docs/` – All documentation

### Step 6: Activation & Role Confirmation (Day 7–10)
- [ ] Attend or watch recording of the next **Onboarding Session** (moderated by Session Moderators)
- [ ] Update your role in `VOLUNTEERS.md` once you feel confident (e.g., “Harvesting Team – Python contributor” or “Humanities Expert – Reconciliation Reviewer”)
- [ ] Subscribe to notifications for labels relevant to your skills (`harvesting`, `rdf-enrichment`, `iiif`, `documentation`, `reconciliation-review`)
- [ ] Optional: Propose one improvement or new idea in a GitHub Issue

**Onboarding Complete!**  
Once all checkboxes are done and your first PR is merged, you will receive the “Active Volunteer” badge/label in the organization. You can now claim more substantial issues and participate in voting for priorities.

**Need help?**  
- Post in `#onboarding-help` Discussion
- Tag `@maintainers` in any issue
- Session Moderators are available for 1:1 mentoring sessions

---

## 5. Technical Architecture – The Multi-Layered Model

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

#### 5.2.1 RDF Reconciliation Pipeline

**Reconciliation** is the core semantic enrichment process. It links ambiguous or variant entities from harvested GLAM metadata (artists, places, materials, subjects, genres, etc.) to canonical identifiers in trusted authorities. This creates a rich, interoperable Linked Open Data graph that powers cross-collection discovery, multilingual support, and advanced IIIF applications.

**Objectives**  
- Reduce duplication and ambiguity  
- Add value through hierarchies, related concepts, and multilingual labels  
- Ensure provenance and traceability for every link  
- Support uncertainty modeling for complex cases  
- Align with FAIR principles  

**5-Step Reconciliation Workflow**

1. **Entity Extraction & Normalization**  
   Parse raw metadata using rule-based patterns, NLP, and RDF lifting scripts in `/services/extractor/`. Target entity types: Agents, Places, Concepts/Subjects/Materials, Works/Events, Genres. Normalize labels and preserve original source strings with provenance.

2. **Automated Candidate Generation**  
   Run batch reconciliation using our core service and **OpenRefine**. Primary authorities: Getty Vocabularies (AAT + TGN), LCSH/LCTGM, Wikidata. Supporting tools: rapidfuzz, fuzzy matching, and OpenRefine reconciliation services.

3. **Human-in-the-Loop Review & Uncertainty Handling**  

   Medium/low-confidence matches are reviewed in **OpenRefine** or via GitHub Issues.

   **Visual Guide to OpenRefine Reconciliation**

   **Figure 1: OpenRefine main project view** – Facets on the left, data rows with reconciliation status, and the matching popup showing candidate details.
<img width="1069" height="891" alt="image" src="https://github.com/user-attachments/assets/bf4406c2-ce85-48c7-bd18-48cf68d3fd92" />

   **Figure 2: Reconciliation setup dialog** – Choose services such as AAT search, TGN search, or Wikidata. Include additional columns to improve matching accuracy
<img  alt="image" src="[https://github.com/user-attachments/assets/bf4406c2-ce85-48c7-bd18-48cf68d3fd92](https://openrefine.org/assets/images/reconcileParis-dd3d74a30c832ae23f778928098ff50b.gif)" />   

   **Figure 3: OpenRefine project with cultural heritage data** – Tabular view of museum-style records ready for reconciliation.
<img width="906" height="620" alt="image" src="https://github.com/user-attachments/assets/ba2cb337-a09a-4095-9b37-eaa0488441b4" />

4. **Link Creation & Graph Enrichment**  
   Add strong links: `skos:exactMatch`, `owl:sameAs`, `dcterms:conformsTo`. Enrich with additional data from authorities while preserving original metadata.

5. **SHACL Validation, Quality Assurance & Finalization**  
   Run validation with `pyshacl`. Enforce that every core entity has at least one `skos:exactMatch` or documented uncertainty note, with full provenance.

**Reconciliation Deliverables per Task**  
- Updated mapping configs in `/ontology/reconciliation-mappings/`  
- New or improved SHACL shapes  
- Pull Request including before/after RDF samples and decision log  

**Turtle Example**  
```turtle
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .

<ex:artwork/123> crm:P14_carried_out_by <http://vocab.getty.edu/aat/300022164> ;
                 skos:exactMatch <https://www.wikidata.org/entity/Q5599> .
```

**Pro Tips for Volunteers**  
- Start with small batches using OpenRefine + Getty service.  
- Always keep original labels.  
- Use the `#reconciliation` Discussion channel for questions.

### Layer 3: IIIF Collection Assembly (Output Layer)
- **Goal**: Generate huge, categorized, multi-part IIIF Collections.  
- **Structure**:  
  - Top-level `collection.json` (the “super-collection”)  
  - Thematic sub-collections (e.g., `subject/islamic-art/collection.json`)  
  - Every manifest must contain reconciled metadata in `metadata[]` and `seeAlso` links to RDF graphs  
- **Automation**: GitHub Actions automatically regenerate collections when enriched data changes.  

---

## 6. Crowdfunding & Sustainability Model

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

## 7. Volunteer Tasks & Contribution Workflow

### General Git Workflow (mandatory for all)
1. Fork → Branch (naming: `feature/connector-europeana`, `fix/shacl-validation`, `docs/glossary-update`, `moderation/session-summary`)  
2. Work in small, reviewable commits  
3. Open PR with checklist in template  
4. Request review from at least two people (one technical, one domain/non-technical where appropriate)  
5. Merge only after CI passes and SHACL validation is green (for data-related PRs)  

### Role-Specific Task Examples

Non-technical roles are **crucial** to the project’s success. While technical teams build the infrastructure, non-technical volunteers ensure the platform is usable, well-documented, welcoming, high-quality, and community-driven.

#### **Document Creators / Content Contributors**
- Maintain and expand core documentation: `GLOSSARY.md`, `TUTORIALS.md`, `METADATA-GUIDELINES.md`  
- Write beginner-friendly guides and educational resources  
- Translate key documents  
- Review public-facing content for clarity and cultural sensitivity  

#### **Session Moderators**
- Plan, host, and moderate weekly calls, hackathons, and onboarding sessions  
- Monitor Discussions and enforce the Code of Conduct  
- Prepare session summaries and celebrate contributor milestones  

#### **General Volunteers / Reviewers**
- Test deliverables and review Pull Requests  
- Label and triage issues  
- Curate new thematic subject categories  
- Perform manual enrichment and usability testing  
- Assist with ethical outreach  

#### **Ubiquitous Language: Bridging Humanities Experts and Technical Staff**

**Humanities & Cultural Heritage Experts** bring deep domain knowledge. To collaborate effectively with technical staff, we maintain a **Ubiquitous Language** — a single, shared vocabulary used consistently in every Issue, PR, Discussion, and meeting.

**Why this matters**  
- Prevents errors in ontologies and metadata  
- Makes technical work more accurate and reusable  
- Builds respect and collaboration across backgrounds  

**Practical Ways to Build & Maintain Ubiquitous Language**

1. **Living Shared Glossary (`GLOSSARY.md`)**  
   Humanities experts define domain terms; technical staff add code mappings. Every term includes plain-language definition + technical equivalent + example.

2. **Joint Terminology Workshops**  
   Monthly sessions: domain story by humanities expert followed by technical mapping.

3. **Pairing & Mentoring**  
   Pair humanities and technical volunteers on tasks; document new terms immediately.

4. **Consistent Language in All Communication**  
   Use glossary terms in Issues, PRs, code comments, and Discussions. Moderators gently enforce clarity.

5. **Domain-Driven Examples**  
   Every technical document must include real-world cultural heritage examples chosen by humanities volunteers.

6. **Feedback Loops & Audits**  
   Humanities experts perform language audits on PRs (label: `ubiquitous-language-review`).

**How Humanities Experts Can Contribute Immediately**  
- Claim `ubiquitous-language` or `glossary` issues  
- Join terminology workshops  
- Review PRs touching ontologies or metadata  

---

## 8. Code of Conduct & Ethics

- **Be kind, be constructive, assume best intent** (Contributor Covenant adopted)  
- **Respect source institutions**: Never harvest restricted content; always credit original providers  
- **Data sovereignty**: GLAMs retain copyright; we only aggregate public-domain or openly licensed material  
- **No commercial exploitation** without explicit community approval  
- **Diversity & inclusion**: We actively welcome volunteers from all geographies and backgrounds  

---

## 9. Tools & Technology Stack (Recommended)

- **Language**: Python 3.11+ (core), JavaScript/Node for front-end utilities  
- **RDF**: rdflib + pyshacl  
- **IIIF**: iiif-prezi3, loris/cantaloupe (optional)  
- **Reconciliation**: **OpenRefine** (strongly recommended), rapidfuzz, Getty & Wikidata services  
- **Version control**: Git + GitHub  
- **CI/CD**: GitHub Actions  
- **Ontology editing**: Protégé (optional)  
- **Communication**: GitHub Discussions + monthly community calls  

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
```

This is the complete, single, valid Markdown document with all sections properly arranged and consistent. You can copy and paste it directly into a `.md` file.

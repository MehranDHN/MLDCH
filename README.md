# Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)  
**Community Policy & Volunteer Guide**  

**Creator: Mehrandhn**
**Version 1.0 (Draft)**  
**Last updated:** April 2026  
**Project repository:** https://github.com/MLDCHA (placeholder – to be created by core team)  
**License:** CC-BY-SA 4.0 for documentation & data; MIT for code  

---

## 1. Introduction & Project Scope

The **Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)** is an open, volunteer-driven platform focused on the harvesting, integration, enrichment, and open redistribution of Persian cultural heritage resources, primarily sourced from Galleries, Libraries, Archives, and Museums (GLAM institutions) worldwide.
The project also leverages the Internet Archive as a complementary open-access repository to surface and preserve important resources that have not been digitized or published by major GLAM institutions, along with materials generously contributed by community volunteers.

![Project Banner](https://github.com/MehranDHN/MLDCH/blob/main/images/ig_01.jpg?raw=true) 

Our **core output** is a massive, living collection of **multi-part IIIF (International Image Interoperability Framework) Collections and Manifests**, organized by curated subject categories. Every manifest is automatically reconciled against the following authoritative vocabularies:

- **AAT** – Getty Art & Architecture Thesaurus  
- **TGN** – Getty Thesaurus of Geographic Names  
- **LCSH** – Library of Congress Subject Headings  
- **LCTGM** – Library of Congress Thesaurus for Graphic Materials  
- **Wikidata** – for additional global identifiers and multilingual labels  

The entire system is built as a **public GitHub-first community** with transparent agenda, governance, version-controlled workflows, and **crowdfunding integrated directly through GitHub Sponsors, GitHub Discussions, and issue-level sponsorships**. No central institution owns the data; the community collectively stewards it.

**Key principles**  
- Open standards only (IIIF, RDF, OWL, SHACL, Linked Open Data)  
- Radical interoperability and reusability  
- Ethical sourcing and respect for source institutions’ rights  
- Merit-based contribution (skills > creden fortials)  
- Full transparency via Git history 
- Full observability with **Knowldge Graph** for future planning

---

## 2. Mission & Vision

**Mission**  
To democratize access to high quality cultural heritage resources and data by creating the largest open, `semantically rich`, `IIIF-native` aggregator maintained by a global volunteer community. The primary focus are in digital resources that scattered around the word spetialy for those that seems available but they are not accessible.

**Vision**  
To create a single, freely queryable IIIF “super-collection” containing millions of reconciled digital objects, organized into rich thematic nested sub-collections (e.g., “Islamic Manuscript Traditions”, “Persian Architecture and Art”, “Oriental Photography”, “Illuminated Manuscripts”, “Historical Documents”, “Oral History”, and many others). These collections will be instantly accessible and reusable by researchers, educators, artists, and GLAM institutions worldwide.
From a technical perspective, the platform will serve as a robust foundation for AI engines and intelligent agents to discover complex relationships between resources, forming a vast, boundary-free Big Data network of interconnected digital cultural heritage materials.

![Overview](/images/Connecting_Our_Digital_Past.mp4)

### The differences between Availability and Acceptability
Availability means a cultural resource exists and is preserved under institutional custody it is “there” in a literal sense. Accessibility, however, means that people can actually discover, view, study, enjoy, interpret, and build upon it without unreasonable technical, linguistic, geographic, or economic barriers.
Availability is necessary but not sufficient. 

A masterpiece can be safely stored in a museum vault, locked behind a paywall, buried in outdated databases, or separated by language and distance, yet remain effectively inaccessible to the communities that value it most.

In the case of Persian cultural heritage, this gap is particularly visible. Many artifacts are preserved in major international institutions and technically “available,” but they lack rich, structured, interoperable metadata and modern presentation technologies. This prevents meaningful engagement by researchers, educators, artists, Iranian communities, and the general public.
Rich structured metadata, delivered through open standards such as RDF (Resource Description Framework) combined with IIIF (International Image Interoperability Framework), is one of the most powerful ways to bridge this gap. RDF provides machine-readable, linked semantic descriptions (connecting objects to people, places, concepts, and historical contexts), while IIIF enables high-resolution, zoomable, annotatable, and interoperable image viewing. Together, they transform static records into dynamic, reusable, and truly accessible digital cultural resources.

### Closing the Gap: What MLDCHA Can Realistically Do
Lets focus on a real example an ornate 48.3 cm diameter steel shield from the early Qajar period in Iran's history, currently in the [Saint Louis Art Museum](https://www.slam.org/collection/objects/2592/)'s collection, praising its highly detailed engravings, gold inlays, and Persian calligraphy visible on the attached.

MLDCHA focuses on practical, scalable actions that turn availability into genuine accessibility:

![Qajar Shield (sipar)](https://d23gjylftzdlen.cloudfront.net/db_photo/d4279/u16742792/1851957dig_1_o2.jpg)

- Full-spectrum digitization as the default
  High-resolution 2D photography is an excellent starting point. When museums make these images openly available, we can harvest them, enrich them with structured metadata, and present them through IIIF manifests that allow deep zooming, side-by-side comparison, and annotation. There are thousands examples [here in IIIFDexir](https://github.com/MehranDHN/MLDCH).
- Rich structured metadata using RDF + IIIF
  We enrich raw images and basic records with detailed, linked metadata: artist/school, historical period, materials and techniques, iconography, inscriptions (with transcription and translation), provenance, and connections to related works. Using RDF and standard ontologies, these descriptions become interoperable and queryable. IIIF then makes the visual content interactive and embeddable anywhere, turning isolated museum records into living parts of a global Persian cultural heritage network.
- Virtual repatriation through technology
  Instead of physical return (which involves complex legal and preservation issues), we create high-fidelity digital surrogates. These can be explored in Persian, with contextual layers added by Iranian scholars and community experts, making the artifact meaningfully accessible to its cultural homeland and the diaspora.  
- Open-access-first policies and Linked Open Data
  We encourage institutions to provide downloadable high-resolution files together with rich, multilingual metadata and API access. MLDCHA aggregates and reconciles this data, linking it to Wikidata (Q8279 for the Shahnama, for example), AAT, TGN, and other authorities, so developers, educators, and AI tools can easily build new experiences around the objects.
- Collaborative digital heritage projects
  We actively partner with Iranian individuals, diaspora experts, and passionate volunteers. Joint curation, shared metadata enrichment, and co-created thematic IIIF collections help transform “object held in a Western museum” into “shared human heritage openly accessible to all.”
- Physical access as a complement, not the only option
  Rotating loans, traveling exhibitions, or even pop-up displays in Tehran or other Iranian cities are powerful—but they’re expensive and temporary. Digital access is permanent and scales globally.
- Leverage modern tools (AI, crowdsourcing, open platforms)
  AI can assist with transcription and translation of Persian inscriptions, while crowdsourcing allows Persian-speaking volunteers to add cultural context, correct attributions, or propose new connections. The enriched data is then integrated into Wikipedia, Wikidata, Google Arts & Culture, and our own IIIF super-collection.
- Advocacy + funding
  Individuals can amplify the conversation (as the original tweet does), push museums via social media, or support grants specifically for digitization of Islamic/Persian collections. Foundations, tech companies, and governments already fund this—it's a matter of prioritizing it.

The shield itself in our typical example is stunning evidence of Qajar craftsmanship. Its real power, though, isn't in being "safe" in St. Louis—it's in being seen, studied, and loved by as many people as possible, especially those whose ancestors made it. Availability protects the object. Accessibility protects its meaning.  
We already have the technology to make almost any preserved cultural resource truly accessible. What we need now is the will—and the smart, collaborative strategies—to close the gap. 

### Availability protects the physical object. Accessibility protects its living cultural meaning.
MLDCHA exists to close this critical gap by combining high-quality images with rich, structured, semantic metadata delivered through RDF and IIIF standards. With community effort, we can make Persian cultural heritage truly discoverable, reusable, and meaningful for scholars, students, artists, and the wider public — regardless of physical location or institutional barriers.
 

---

## 3. Community Structure & Roles

All work happens in the public GitHub organization. Everyone uses Git, GitHub Issues, Projects, Discussions, and Pull Requests.

| Role | Primary Responsibilities | Required Skills | Time Commitment |
|------|---------------------------|-----------------|-----------------|
| **Document Creators / Content Contributors** | Write policy, tutorials, glossaries, metadata guidelines | Markdown, research, clear writing | Flexible (1–5 hrs/week) |
| **WikiData Editors** | Create/Edit WikiData's Q Codes | WikiData Ontology | Flexible (1–5 hrs/week) |
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
  - Optional but helpful: Protégé (for ontology work), Postman/Insomnia (for API testing)

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
    - Data: Manually reconcile 10 sample records against Wikidata/AAT
    - General: Label or triage 5 open issues
- [ ] Work on your task in a new branch (`feature/your-task-name` or `docs/your-task-name`)
- [ ] Open a Pull Request with clear description and checklist
- [ ] Participate in at least one community call or Discussion thread to ask questions

### Step 5: Learning & Setup (Ongoing during onboarding)
- [ ] Complete the **Core Tutorials** (links will be in `TUTORIALS.md`):
  - Introduction to IIIF Manifests & Collections
  - Basic RDF and JSON-LD for Cultural Heritage
  - Our Reconciliation Pipeline (AAT/TGN/LCSH/Wikidata)
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
- [ ] Update your role in `VOLUNTEERS.md` once you feel confident (e.g., “Harvesting Team – Python contributor”)
- [ ] Subscribe to notifications for labels relevant to your skills (`harvesting`, `rdf-enrichment`, `iiif`, `documentation`)
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
![MLDCHA Architecture Overview](/images/mldcha_architecture_fixed.svg)
### Layer 1: Harvesting & Connectors (Data Acquisition)
- **Goal**: Pull raw metadata and images from GLAM sources.  
- **Preferred sources** (in order):  
  1. IIIF Presentation API 2.0/3.0 compliant endpoints  
  2. RESTful APIs (Europeana, Digital Public Library of America, etc.)  
  3. XML, CSV, OAI-PMH  
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

#### 5.2.1 RDF Reconciliation Pipeline (Detailed)
**Reconciliation** is the heart of our semantic enrichment process. It links extracted entities from harvested GLAM metadata (e.g., artist names, place names, materials, subjects, genres) to canonical identifiers in external authorities. This creates a Linked Open Data (LOD) graph that is interoperable, queryable via SPARQL, and automatically enriches every IIIF manifest.

**Why reconciliation matters**  
- Prevents duplication (e.g., “Esfahan” vs. “Isfahan” vs. “Исфахан”)  
- Enables cross-collection discovery (e.g., all objects linked to the same AAT concept for [Calligraphy](http://vocab.getty.edu/page/aat/300053162) as a process vs [Calligraphy](http://vocab.getty.edu/page/aat/300266660) as visual works)  
- Adds multilingual labels, hierarchies, and related concepts for free  
- Powers advanced IIIF viewers and external tools (Europeana, Google Arts & Culture, etc.)

**Mandatory 4-Step Reconciliation Workflow** (applied to every harvested record)

1. **Entity Extraction**  
   - Automatically parse harvested metadata using rule-based + NLP pipelines (spaCy + custom RDF patterns) and direct supervising.  
   - Target entity types:
     - Events (Event-based approach)  
     - Agents (persons, organizations)  
     - Places (cities, regions, sites)  
     - Concepts / Subjects (art styles, materials, techniques, processes)  
     - Temporal Entities / Historical periods
   - Output: Temporary RDF triples with `rdfs:label` and source provenance (`dcterms:provenance`).

2. **Automated Matching (Batch Phase)**  
   - Use our core reconciliation service (`/services/reconciler/`) built with:  
     - **Official APIs** (preferred):  
       - Getty Vocabularies API (AAT + TGN)  
       - Library of Congress Linked Data Service (LCSH + LCTGM)  
       - Wikidata SPARQL endpoint + MediaWiki API  
     - **Libraries & Tools**:  
       - `rdflib` + `pyshacl` for graph operations  
       - Fuzzy + phonetic matching (`fuzzywuzzy` / `rapidfuzz`)  
       - Embedding-based similarity (optional: Sentence-Transformers for advanced volunteers)  
       - `OpenRefine` reconciliation API (for quick manual batches)  
   - Generate candidate links with confidence scores (0–100).  
   - Threshold rules:  
     - ≥ 95% → auto-accept  
     - 70–94% → flag for human review  
     - < 70% → discard or route to manual queue  
   - Create properties:  
     - `skos:exactMatch` (strongest link)  
     - `owl:sameAs` (for broader equivalence)  
     - `dcterms:conformsTo` (links to the authority vocabulary itself)

3. **Human-in-the-Loop Review**  
   - All medium-confidence matches are turned into GitHub Issues (label: `reconciliation-review`).  
   - Volunteers review via:  
     - Web-based preview tool (included in repo) showing side-by-side source label vs. candidate authority record 
     - Bulk JSON export/import for power users 
     - Bulk CSV export/import for power users  
     - Discussion threads for disputed cases  
   - Data Science volunteers can claim batches (e.g., “Reconcile 500 Islamic manuscript places to TGN”).  
   - Approved links are committed back to the RDF graph.
   - Any successful Commits automaticaly trigers CI/CD pipeline and Knowledge Grap Generator.

4. **SHACL Validation & Finalization**  
   - Run full SHACL validation (`pyshacl` via GitHub Action).  
   - Required shapes include:  
     - Every entity must have at least one `skos:exactMatch` to an approved vocabulary  
     - No broken links (HTTP 200 checks)  
     - Provenance tracking for every reconciliation decision  
   - If validation passes → merge to `/data/enriched/`.  
   - If fails → automatic PR comment with error report.

**Reconciliation Deliverables per Volunteer Task**  
- Updated reconciliation config files (`/ontology/reconciliation-mappings/`)  
- New SHACL shapes for custom entity types  
- Pull Request with before/after RDF samples  
- Documentation of any new matching rules added

**Example**  
Harvested record: `creator: "Mir Ali Tabrizi" or "Mir Mossavir"`  
→ Auto-matches to Wikidata Q4115137 + AAT 300266660 (with confidence >=95%)  
→ Final triple:  
```turtle
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .

<ex:artwork/123> crm:P14_carried_out_by <http://vocab.getty.edu/aat/300266660> ;
                 skos:exactMatch <https://www.wikidata.org/entity/Q4115137> .
```

**Pro Tips for Volunteers**  
- Start with `good-first-issue` reconciliation tasks (small batches of 10–50 records).  
- Always preserve original source labels in `rdfs:label` (never overwrite).  
- Use the `#reconciliation` Discussion channel for questions or new authority suggestions.  

### Layer 3: IIIF Collection Assembly (Output Layer)
- **Goal**: Generate huge, categorized, multi-part IIIF Collections.  
- **Structure**:  
  - Top-level `collection.json` (the “super-collection”)  
  - Thematic sub-collections (e.g., `subject/islamic-art/collection.json`)  
  - Every manifest must contain reconciled metadata in `metadata[]` and `seeAlso` links to RDF graphs
  - IIIF Annotation for richer contents and navPlace Extension for needed Spatial Data  
- **Automation**: GitHub Actions automatically regenerate collections when enriched data changes.  
![MLDCHA Architecture Overview](/images/MLDCHA_IIIF_Collection.jpg)
---
## 6. Crowdfunding & Sustainability Model

The project runs **entirely through GitHub**:

- **GitHub Sponsors** at organization level  
- **Issue-level sponsorships** (label `💰 funded` – community votes on priorities)  
- **GitHub Discussions** for funding proposals and transparent budget reports  
- All funds are used only for:  
  - Cloud credits for harvesting infrastructure  
  - Domain & hosting
  - Database and GraphDB services  
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
- `Europeana`, `Cultural Japan`, `Biblissima`and `LUX` R&D  

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
#### Contributing to Wikidata: Enhancing the Public Knowledge Base

**Wikidata** serves as one of the world’s largest **open, public-access knowledge bases** and a central hub in the Linked Open Data ecosystem. It functions as a vast, collaborative ontology that anyone can edit, containing millions of structured entities (identified by **Q codes**) and relationships (defined by **P properties**). Its strength lies in its flexibility, multilingual support, and ability to connect disparate sources — making it ideal for cultural heritage projects like MLDCHA.

By contributing to Wikidata, volunteers help create reliable, machine-readable links that our reconciliation pipeline can automatically use. Every edit improves discoverability not only for MLDCHA but for the entire global research community.

**Why Wikidata is crucial for MLDCHA**  
- It acts as a bridge between GLAM metadata, AAT, TGN, LCSH, and our IIIF manifests.  
- It supports complex nested structures (e.g., a literary work containing episodes, characters, and specific manuscript copies).  
- All reconciliations in MLDCHA aim to create strong `skos:exactMatch` or `owl:sameAs` links to Wikidata Q items.

**How to Contribute – Practical Steps**  
1. Create a free Wikidata account (uses the same login as Wikipedia).  
2. Search for existing items before creating new ones.  
3. Add or improve **statements** (facts), **qualifiers**, **references**, and **labels/aliases** in multiple languages.  
4. Use the **“Add statement”** button and follow community guidelines (be bold but verify with reliable sources).  
5. For complex cultural heritage items, document your sources clearly.  
6. After editing, add the improved Q code to our reconciliation mappings or reconciliation-review issues in the MLDCHA repository.

**Example: The Shahnama (Shahnameh) of Ferdowsi**

The **Shahnama** (Q8279) is the iconic Persian epic poem written by Ferdowsi around 1000 CE. In Wikidata, the main item Q8279 represents the abstract **literary work** itself.

Key statements typically include:
- `instance of (P31)` → literary work / epic poem
- `author (P50)` → Ferdowsi (Q43459)
- `language of work (P407)` → Persian
- `publication date (P577)` → circa 1010
- `has part (P527)` or nested structures for its many episodes/stories

The Shahnama contains dozens of **nested episodes** featuring historical, mythical, and fictional characters — both human and supernatural creatures (e.g., Rostam, Sohrab, Simurgh, Divs/demons). These can be modeled in Wikidata as:
- Separate items for major episodes or characters
- Linked back to Q8279 via properties like `part of (P361)` or `narrative entity (P840)`

**Excellent Real-World Example: The Shahnama of Shah Tahmasp (Q3114572)**

This 16th-century illuminated manuscript (also known as the Houghton Shahnameh) is one of the most magnificent copies ever produced, containing 258 miniatures.

In Wikidata:
- **Q3114572** represents this specific **manuscript** (a physical exemplar).
- It is linked to the main literary work via the property **`exemplar of (P1574)`** → pointing to **Q8279** (Shahnama).

This relationship allows us to distinguish between:
- The abstract work (Q8279)
- Specific manuscript copies (like Q3114572)
- Individual folios or miniatures (which can have their own Q items linked as `part of` the manuscript)

**How this helps MLDCHA**  
When we harvest a digital image or metadata of a folio from the Shah Tahmasp Shahnama, our pipeline can reconcile it to Q3114572 → which links via P1574 to Q8279 → enabling rich connections to all other Shahnama-related resources, characters, episodes, and multilingual descriptions.

**Volunteer Tasks Related to Wikidata**
- Improve existing Shahnama-related items (add missing miniatures, folios, or references).
- Create or enhance items for Persian cultural heritage entities that are missing or incomplete.
- Add `IIIF Manifest` URLs or `digital representation of` statements when appropriate.
- Participate in reconciliation campaigns focused on Persian literary works and manuscripts.
- Document your edits in MLDCHA GitHub issues (label: `wikidata-contribution`).

**Best Practices**
- Always cite reliable sources (e.g., scholarly publications, museum catalogs).
- Use Persian labels and aliases whenever possible.
- Coordinate complex edits via the `#reconciliation` or new `#wikidata` Discussion channel in our repository.
- For beginners: Start by improving labels, descriptions, or adding external identifiers on well-known items like Q8279.

By actively contributing to Wikidata, you directly strengthen the semantic backbone of MLDCHA and help build a truly global, interconnected Persian cultural heritage knowledge graph.

---
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
- **RDF**: rdflib + pyshacl + Jupiter Notebook 
- **IIIF**: iiif-prezi3, loris/cantaloupe (optional)  
- **Version control**: Git + GitHub  
- **CI/CD**: GitHub Actions  
- **Ontology editing**: Protégé (optional)  
- **Communication**: GitHub Discussions + monthly community calls  
- **GraphDB &Knowledge Graph**: ONTOTEXT GraphDB Desktop, Stardog, Neo4J 

---

## 10. Getting Started – Your First Week

1. Star and fork the repo  
2. Read `CONTRIBUTING.md` and this policy  
3. Join the weekly onboarding call (link in Discussion #2)  
4. Claim your first issue (label `good-first-issue`)  
5. Introduce yourself in the `#introductions` Discussion  

---

## 11. Roadmap (High-Level)

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

## Credits & Acknowledgments

### Project Leadership
**Founder & Primary Maintainer:** Mehrandhn  
**Repository:** [github.com/MehranDHN/MLDCH](https://github.com/MehranDHN/MLDCH)

### AI Assistance & Development Tools
This documentation was created with assistance from:
- **Claude** (Anthropic) – Documentation structure, policy framework, and technical guidance
- **Grok** (xAI) – Ideation and content refinement
- **NotebookLM** (Google) – Research synthesis and organization

### Technology Stack & Standards
Built on open standards maintained by:
- **IIIF Consortium** – International Image Interoperability Framework
- **W3C** – RDF, OWL, SHACL, and SKOS specifications
- **Getty Research Institute** – Art & Architecture Thesaurus (AAT), Thesaurus of Geographic Names (TGN)
- **Library of Congress** – Subject Headings (LCSH) and Thesaurus for Graphic Materials (LCTGM)
- **Wikidata** – Collaborative knowledge base
- **CIDOC-CRM** – Conceptual Reference Model for cultural heritage

### Institutional Inspiration
This project draws inspiration from exemplary digital cultural heritage initiatives:
- **Europeana** – European digital cultural heritage aggregation
- **Digital Public Library of America (DPLA)**
- **Biblissima** – French manuscript aggregation
- **Cultural Japan** – Japanese heritage digitization
- **LUX (Yale Collections Discovery)**

### Community Contributors
Active volunteer contributors are listed in `VOLUNTEERS.md`. We welcome and acknowledge all contributors regardless of background or technical expertise.

### Funding & Sustainability
MLDCHA operates as a transparent, community-funded project via:
- GitHub Sponsors (organization level)
- Issue-level sponsorships
- All financial reports published monthly in `FINANCES.md`

### Rights & Licensing
- **Documentation & Data:** CC-BY-SA 4.0
- **Code:** MIT License
- **Content sourced from GLAM institutions:** Respective institutional licenses apply
- **Respect for source institutions:** We acknowledge and credit all original content providers

### Special Thanks
To the global GLAM community for their commitment to open access, and to all volunteers who contribute their time, expertise, and passion to preserving and sharing Persian cultural heritage.

---

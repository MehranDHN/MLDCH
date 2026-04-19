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

(unchanged – refer to previous version)

---

## 5. Technical Architecture – The Multi-Layered Model

(unchanged – including the full RDF Reconciliation Pipeline with OpenRefine screenshots)

---

## 6. Crowdfunding & Sustainability Model

(unchanged)

---

## 7. Volunteer Tasks & Contribution Workflow

### General Git Workflow (mandatory for all)
1. Fork → Branch (naming: `feature/connector-europeana`, `fix/shacl-validation`, `docs/glossary-update`, `moderation/session-summary`)  
2. Work in small, reviewable commits  
3. Open PR with checklist in template  
4. Request review from at least two people (one technical, one domain/non-technical where appropriate)  
5. Merge only after CI passes and SHACL validation is green (for data-related PRs)  

### Role-Specific Task Examples

Non-technical roles are **crucial** to the project’s success. While technical teams build the infrastructure, non-technical volunteers ensure the platform is **usable, well-documented, welcoming, high-quality, and community-driven**. Without strong documentation, moderation, curation, and review, even the best code and data would remain inaccessible to most users and new volunteers. These roles scale the project, improve adoption by GLAMs and researchers, and maintain the human-centered spirit of open cultural heritage.

#### **Document Creators / Content Contributors** (Non-Technical – Core Educational Role)
(unchanged – refer to previous version)

#### **Session Moderators** (Non-Technical – Community & Governance Role)
(unchanged – refer to previous version)

#### **General Volunteers / Reviewers** (Non-Technical – Quality & Curation Role)
(unchanged – refer to previous version)

#### **Ubiquitous Language: Bridging Humanities Experts and Technical Staff**

**Humanities & Cultural Heritage Experts** (often called “domain experts” or “human science experts” in this policy) play a vital role in ensuring that technical decisions reflect real-world GLAM knowledge. However, technical and humanities teams traditionally speak different languages: one full of RDF triples, SHACL shapes, and Git workflows; the other full of curatorial terms, iconographic analysis, provenance research, and subject-specific nuances.

To eliminate miscommunication and create truly meaningful data, we adopt the concept of **Ubiquitous Language** — a single, shared vocabulary that everyone in the community uses consistently. This is not jargon-heavy; it is a practical, evolving set of terms that both sides agree upon and use in every Issue, PR, Discussion, meeting, and code comment.

**Why this matters**  
- Prevents errors (e.g., a technical volunteer implementing a “subject” field that does not match how a curator understands “iconography”).  
- Makes ontologies and IIIF metadata more accurate and reusable.  
- Builds respect and collaboration across skill sets.  
- Accelerates onboarding for everyone.

**Practical Ways Humanities Experts and Technical Staff Build & Maintain Ubiquitous Language**

1. **Living Shared Glossary (Core Tool)**  
   - The `GLOSSARY.md` file is the single source of truth.  
   - Humanities experts lead definitions for domain terms (e.g., “provenance”, “iconographic motif”, “thematic collection”, “culturally sensitive entity”).  
   - Technical staff add precise mappings to code concepts (e.g., “how ‘motif’ appears as an AAT concept in RDF”).  
   - Every major term must have: plain-language definition + technical equivalent + example from a real GLAM record.  
   - Updated via PRs; reviewed in every community call.

2. **Joint Terminology Workshops & “Translation” Sessions**  
   - Held monthly in community calls (moderated by Session Moderators).  
   - Format: 15-minute “domain story” by a humanities expert (e.g., “How we describe Persian miniature paintings”) followed by technical mapping (e.g., “Here’s how that becomes RDF triples and IIIF metadata”).  
   - Outcome: New glossary entries + updated SHACL shapes or reconciliation rules.

3. **Pairing & Mentoring Across Roles**  
   - Humanities experts and technical volunteers are encouraged to pair on small tasks (e.g., “Review this new connector together”).  
   - Use GitHub’s “Pairing” label for Issues.  
   - During pairing: speak only in ubiquitous language; document any new terms immediately.

4. **Consistent Language in All Communication**  
   - **GitHub Issues & PRs**: Use glossary terms only. If a new term is needed, link to or propose its definition first.  
   - **Code & Comments**: Technical volunteers must include humanities-friendly comments (e.g., `# This SHACL shape enforces curator-defined rules for 'artistic technique'`).  
   - **IIIF Manifests & RDF**: Metadata labels must include human-readable descriptions alongside machine terms.  
   - **Discussions & Calls**: Session Moderators gently enforce “Let’s use the glossary term here” when confusion arises.

5. **Domain-Driven Examples in Technical Documentation**  
   - Every technical README or tutorial must contain at least one real-world cultural heritage example chosen by humanities volunteers.  
   - E.g., “Reconciliation example: Matching a 16th-century Ottoman calligrapher to AAT and Wikidata.”

6. **Feedback Loops & Regular Audits**  
   - Humanities experts perform “language audits” on merged PRs (label: `ubiquitous-language-review`).  
   - Quarterly community survey: “Did technical explanations make sense?”  
   - Maintainers track and celebrate improvements in shared understanding.

**How Humanities Experts Can Contribute Immediately**  
- Claim issues labeled `ubiquitous-language` or `glossary`.  
- Join or propose a terminology workshop.  
- Review any PR that touches ontologies, reconciliation, or IIIF metadata for clarity.  
- Suggest new terms during reconciliation reviews (especially for culturally nuanced entities).

By maintaining this ubiquitous language, we ensure that the technical layers truly serve the cultural heritage mission — and that every volunteer, regardless of background, feels empowered to contribute at the highest level.

---

## 8. Code of Conduct & Ethics

(unchanged)

---

## 9. Tools & Technology Stack (Recommended)

(unchanged, with OpenRefine still highlighted for all volunteers)

---

## 10. Getting Started – Your First Week

(unchanged)

---

## 11. Roadmap (High-Level)

(unchanged)

---

**This document is living.**  
All changes must be proposed via Pull Request and approved by the current volunteer maintainers (elected every 6 months via GitHub poll).  

Welcome to the team!  
Together we are building the future of open cultural heritage.  

**— The MLDCHA Community**

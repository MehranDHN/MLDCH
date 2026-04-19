Here's the updated **MLDCHA Community Policy & Volunteer Guide** with the addition of **OpenRefine screenshots** in the RDF Reconciliation Pipeline section.

The screenshots are placed inline with clear captions to make the workflow more visual and educational for volunteers (especially those new to reconciliation). They illustrate:
- The main OpenRefine project view with facets and matching options.
- The reconciliation setup dialog (showing AAT/TGN support).
- The side-by-side preview and matching interface.

---

# Multi-Layered Digital Cultural Heritage Aggregator (MLDCHA)  
**Community Policy & Volunteer Guide**  

**Version 1.4 (Draft)**  
**Last updated:** April 2026  
**Project repository:** https://github.com/MLDCHA (placeholder – to be created by core team)  
**License:** CC-BY-SA 4.0 for documentation & data; MIT for code  

---

## 1. Introduction & Project Scope

(unchanged)

---

## 2. Mission & Vision

(unchanged)

---

## 3. Community Structure & Roles

(unchanged)

---

## 4. Volunteer Onboarding Checklist

(unchanged)

---

## 5. Technical Architecture – The Multi-Layered Model

### Layer 1: Harvesting & Connectors (Data Acquisition)

(unchanged)

### Layer 2: Integration & Enrichment (Semantic Layer)

- **Goal**: Convert everything into a unified RDF graph that is flexible across multiple OWL ontologies.  
- **Core technologies**:  
  - RDF (JSON-LD 1.1 preferred)  
  - Multiple OWL ontologies (CIDOC-CRM, EDM, BIBFRAME, Schema.org, plus custom extensions)  
  - **SHACL shapes** for validation and quality control  

#### 5.2.1 RDF Reconciliation Pipeline (Revised with Visuals)

**Reconciliation** is the core semantic enrichment process. It links ambiguous or variant entities from harvested GLAM metadata (artists, places, materials, subjects, genres, etc.) to canonical identifiers in trusted authorities. This creates a rich, interoperable Linked Open Data graph that powers cross-collection discovery, multilingual support, and advanced IIIF applications.

**Objectives**  
- Reduce duplication and ambiguity  
- Add value through hierarchies, related concepts, and multilingual labels  
- Ensure provenance and traceability for every link  
- Support uncertainty modeling for complex cases  
- Align with FAIR principles  

**5-Step Reconciliation Workflow**

1. **Entity Extraction & Normalization**  
   (unchanged)

2. **Automated Candidate Generation**  
   (unchanged – uses Getty, LCSH, Wikidata, fuzzy matching, and **OpenRefine**)

3. **Human-in-the-Loop Review & Uncertainty Handling**  
   Medium/low-confidence matches are reviewed in **OpenRefine** (highly recommended tool) or via GitHub Issues.

   **Visual Guide to OpenRefine Reconciliation**




**Figure 1: OpenRefine main project view** – Facets on the left, data rows with reconciliation status, and the matching popup showing candidate details (e.g., artist name with lifespan and profession). Volunteers can match individual cells or all identical values at once.
<img width="906" height="620" alt="image" src="https://github.com/user-attachments/assets/b95b1ccf-c740-4d27-b8f1-7607bf840f9b" />




**Figure 2: Reconciliation setup dialog** – Choose services such as AAT search, TGN search, or Wikidata. You can include additional columns (e.g., dates or context) to improve matching accuracy and set auto-match thresholds.

<img width="906" height="620" alt="image" src="https://github.com/user-attachments/assets/f65adb47-dc7e-4d42-ac66-3ed15b69da96" />



**Figure 3: OpenRefine project with cultural heritage data** – Example tabular view of museum-style records ready for reconciliation. Columns can include titles, descriptions, creators, and places.

<img  alt="image" src="https://openrefine.org/assets/images/reconcileParis-dd3d74a30c832ae23f778928098ff50b.gif" />



4. **Link Creation & Graph Enrichment**  
   (unchanged)

5. **SHACL Validation, Quality Assurance & Finalization**  
   (unchanged)

**Reconciliation Deliverables per Task**  
(unchanged)

**Turtle Example**  
(unchanged)

**Pro Tips for Volunteers**  
- **Start here**: Download OpenRefine (free, open-source) and practice with the sample projects in `/examples/openrefine/`.  
- Use the Getty reconciliation service for AAT/TGN and Wikidata for broader coverage.  
- Export reconciled projects as RDF/JSON-LD directly for import into our pipeline.  
- For complex batches, share your OpenRefine project file (.tar.gz) in a GitHub Issue for collaborative review.  
- Always document your decisions in the project notes or a linked Discussion thread.

### Layer 3: IIIF Collection Assembly (Output Layer)

(unchanged)

---

## 6. Crowdfunding & Sustainability Model

(unchanged)

---

## 7. Volunteer Tasks & Contribution Workflow

(unchanged)

---

## 8. Code of Conduct & Ethics

(unchanged)

---

## 9. Tools & Technology Stack (Recommended)

- **Language**: Python 3.11+ (core), JavaScript/Node for front-end utilities  
- **RDF**: rdflib + pyshacl  
- **IIIF**: iiif-prezi3, loris/cantaloupe (optional)  
- **Reconciliation**: **OpenRefine** (strongly recommended for human review), rapidfuzz, Getty & Wikidata services  
- **Version control**: Git + GitHub  
- **CI/CD**: GitHub Actions  
- **Ontology editing**: Protégé (optional)  
- **Communication**: GitHub Discussions + monthly community calls  

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

---

This addition makes the reconciliation section much more beginner-friendly by providing concrete visual references. The screenshots are rendered at LARGE size for clarity while keeping the document flow clean.

Would you like any adjustments to captions, more/less images, or further expansions (e.g., adding a dedicated "Tools Setup" subsection with OpenRefine installation instructions)?

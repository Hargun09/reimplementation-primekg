# Reimplementation-PrimeKG

An independent reimplementation of [PrimeKG](https://github.com/mims-harvard/PrimeKG) - the **Precision Medicine Knowledge Graph** originally built by Payal Chandak, Kexin Huang, and Marinka Zitnik at the Zitnik Lab, Harvard Medical School.

>  **Original repository:** https://github.com/mims-harvard/PrimeKG

>  **Original paper:** [Building a knowledge graph to enable precision medicine](https://www.nature.com/articles/s41597-023-01960-3) 
---

**This repository is not affiliated with or endorsed by the original PrimeKG authors.** All credit for the original design, methodology, and dataset goes to the Harvard team

---

## Input

- disease.zip - compressed archive of disease.csv, containing disease-protein association records (UniProt Disease evidence, association scores, gene expression fold-changes, and drug/source references) linked to MONDO disease IDs
- mondo.csv - MONDO disease ontology terms with standardized IDs, names, and definitions
- mondo_parent.csv - MONDO parent-child relationships, defining the disease ontology hierarchy
- protein.csv - protein/gene records with UniProt IDs, gene symbols, and cross-references (STRING, DTO)

## Output

- out_prime.csv - the final merged knowledge graph, joining disease, MONDO ontology, and protein/gene tables

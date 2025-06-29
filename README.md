# p53 Mutation Knowledge Graph for Therapeutic Exploration

## Overview

This project constructs a structured **knowledge graph of TP53 mutations**, associated **cell lines**, **protein variants**, and **chemical modulators**. Using a custom-built ontology and SPARQL queries in Python, it enables exploration of therapeutic strategies targeting wild-type and mutant p53, a critical tumor suppressor frequently mutated in cancer.

## Objectives

- Corresponding **p53 protein variants**, and **targeted therapies**
- Use SPARQL/DL queries to extract biologically meaningful drug-target-cell line triplets
- Visualize interaction networks to highlight therapeutic opportunities and assay-readiness

## Tools 

| Tool         | Purpose                            |
|--------------|-------------------------------------|
| Protégé     | Ontology design (OWL DL)            |
| Python + RDFLib | Querying OWL ontology (SPARQL)   |
| NetworkX     | Graph-based visualization          |
| Flow cytometry assays | For apoptosis & cell cycle validation |
| Pandas       | Data manipulation & tabular view   |


## Contents

- `TP53_onto.ttl` – Custom OWL ontology of p53 mutations, drugs, and cell lines
- `p53_query.ipynb` – Jupyter notebook with SPARQL queries and graph visualizations
- `README.md` – Project summary and guidance


## Biological Focus

### Mutation Targets
- **Wild-type p53**
- **Missense mutations**: R175H, R273H, R248Q/W, Y220C

### Assay-Compatible Effectors
- **Cell Cycle Arrest**: p21 (CDKN1A), GADD45α, 14-3-3σ
- **Apoptosis Inducers**: PUMA, NOXA, BAX

### Modulator Classes
- **Restorative agents** (e.g., APR246 for R175H)
- **MDM2 inhibitors** for wild-type p53 stabilization
- **Transcriptional activators** for downstream genes


## Example Visual Output

![image](https://github.com/user-attachments/assets/a0de2691-010f-4546-b09f-327e23aa873b)

![image](https://github.com/user-attachments/assets/4ffbc637-6fc6-436b-8ada-a7d13f5ebf18)

![image](https://github.com/user-attachments/assets/f3751940-447a-41cd-a665-74ce64716f26)


## Future Directions

- Integrate with **machine reasoning** tools (e.g., graph neural networks)
- Expand to cover **PTEN**, **BRCA1**, and other tumor suppressors
- Link to public datasets (e.g., TCGA, DepMap) for large-scale screening
- Add **confidence scores** or **evidence strength** per triple (from literature mining)


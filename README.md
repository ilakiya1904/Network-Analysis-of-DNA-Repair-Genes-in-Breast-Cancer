# Network Analysis of DNA Repair Genes in Breast Cancer

This mini-project focuses on the intersection of DNA repair mechanisms and breast cancer using network biology tools like STRING and Cytoscape. It identifies overlapping genes between DNA repair pathways and breast cancer-associated genes, then visualizes and analyzes the protein–protein interaction (PPI) network to identify key hub genes.

---

## Objective

To uncover key DNA repair genes that may play a pivotal role in breast cancer by:
- Extracting gene data from reliable databases.
- Mapping interactions using STRING.
- Analyzing topological features via Cytoscape.

---

## Data Sources

- **Breast Cancer Genes**: [GDC Data Portal](https://portal.gdc.cancer.gov/)
- **DNA Repair Genes**: [Reactome Pathway Database](https://reactome.org/)
- **PPI Network**: [STRING Database](https://string-db.org/)

---

## Methodology

1. **Gene Collection**
   - Extracted breast cancer mutation genes from GDC.
   - Retrieved curated DNA repair genes from Reactome.

2. **Intersection Analysis**
   - Found **29 overlapping genes** between breast cancer and DNA repair sets.

3. **Network Construction**
   - Entered overlapping genes into the STRING database.
   - Exported interaction file (TSV) with confidence scores.

4. **Cytoscape Analysis**
   - Imported STRING interactions into Cytoscape.
   - Applied the **Organic layout** for clarity.
   - Used **CytoHubba** plugin to calculate **node degree**.
   - Identified the **Top 5 hub genes** based on degree.

---

## 🧬 Top 5 Hub Genes (by Degree)

| Rank | Gene    |
|------|---------|
| 1    | **ATM**   |
| 2    | **CHEK2** |
| 3    | **CHEK1** |
| 4    | **BRCA1** |
| 5    | **BRCA2** |

> *These hub genes are crucial players in the DNA damage response and repair pathways and are frequently mutated or dysregulated in breast cancer.*

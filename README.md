
# Single-Cell RNA-Seq Analysis using Scanpy

### Project Summary
This project reproduces a core single-cell RNA sequencing (scRNA-seq) analysis pipeline using **Scanpy** in Python.  
The dataset contained immune cells originally labeled as “bone marrow,” and the goal was to perform preprocessing, clustering, and biological interpretation of the identified cell populations.

---

## What I Did
✔️ Loaded scRNA-seq data and created an AnnData object  
✔️ Performed quality control (mitochondrial filtering, gene filtering)  
✔️ Normalized and log-transformed the dataset  
✔️ Identified highly variable genes  
✔️ Performed PCA → Neighbors graph → UMAP  
✔️ Clustered cells using Leiden clustering  
✔️ Computed marker genes and annotated cell types  
✔️ Interpreted biological meaning of clusters  

---

## Biological Findings

### Cell Types Identified
- IL7R⁺ T cells
- Cytotoxic T / NK-like T cells
- NK cells
- Classical monocytes
- Inflammatory monocytes
- B cells
- Memory / activated B cells
- Plasma cells
- Proliferating immune cells
- Megakaryocytes/platelet lineage

---

### Key Biological Interpretation
- The dataset shows **fully mature immune cells**, not early bone marrow progenitors  
- Lacks stem cells, erythroid precursors, and granulocyte precursors  
  The sample likely reflects **PBMC / peripheral blood**, not classical bone marrow

- Expanded inflammatory monocytes  
- Strong cytotoxic / NK activation  
- Presence of plasma cells and proliferating cells  
  Suggests **infection or immune activation**, not a healthy baseline

  ## How to Run This Notebook
### Install Dependencies
pip install scanpy decoupler anndata pandas numpy matplotlib

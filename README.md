# Single-Cell RNA-Seq Analysis of Bone Marrow

## Project Overview
This project reproduces a standard single-cell RNA-seq analysis workflow using Scanpy to process bone marrow data from raw counts to biologically interpretable cell type clusters.

## Analysis Pipeline
1. **Data Loading & QC**: Load bone marrow dataset and perform quality control
2. **Preprocessing**: Normalization, log transformation, HVG selection
3. **Dimensionality Reduction**: PCA, UMAP, and clustering
4. **Cell Type Annotation**: Marker-based identification using Decoupler
5. **Biological Interpretation**: Cell type roles and health assessment

## Key Findings
- **Cell Types Identified**: Neutrophils, Monocytes, T cells, B cells, NK cells, Erythrocytes, Megakaryocytes
- **Tissue Source**: Likely bone marrow based on progenitor presence and cell type distribution
- **Health Status**: Patient shows normal bone marrow composition

## Files
- `bone_marrow_analysis.ipynb` - Main analysis notebook
- `bone_marrow_annotated.h5ad` - Annotated dataset
- `cell_type_assignments.csv` - Cell type assignments
- `analysis_summary.csv` - Analysis metadata
- `linkedin_umap.png` - UMAP visualization for carousel

## Requirements
```bash
scanpy>=1.9.0
pandas>=1.5.0
numpy>=1.21.0
matplotlib>=3.5.0
decoupler>=1.4.0
```

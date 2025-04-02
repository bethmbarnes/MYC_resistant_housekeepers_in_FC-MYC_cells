# Analysis of RNA-seq of MYC-Low and MYC-High FC-MYC Cells Following SUMOylation Inhibition with SAEi ML-792 Using MYC-Resistant Housekeeping Genes

## Overview

This repository contains the analysis pipeline for RNA-seq data generated from MYC-low and MYC-high FC-MYC cells treated with the SUMOylation inhibitor ML-792 (SAEi). By leveraging MYC-resistant housekeeping genes identified from the Loven *et al.* (2012) dataset, we normalize RNA-seq data and examine differential gene expression and transcriptional responses in distinct MYC backgrounds under SUMOylation inhibition.

This dataset and analysis aim to provide insights into the synthetic lethality between MYC and SUMOylation, with potential implications for therapeutic strategies targeting MYC-driven cancers.

---

## Background

The synthetic lethal relationship between MYC and SAE2 has been described previously in FC-MYC cells using RNAi (Littler *et al.*, 2019). Building on this foundational work, we conducted transcriptomic analyses on MYC-low and MYC-high cells treated with SAEi to study the differential impact of SUMOylation inhibition on cells with varying MYC activity.

### Experimental Design:
- **Cell Model**: FC-MYC cells grown in MYC-low and MYC-high conditions.
  - MYC-low: 24 hours in the absence of tetracycline.
  - MYC-high: 24 hours in the presence of 500 ng/mL tetracycline.
    
- **Treatments**:
  - Vehicle control (DMSO).
  - SAEi ML-792 (25 nM).
    
- **Replicates**: Three biological replicates per condition.
  
## Objectives

1. **Identify MYC Non-Responders**: Use RNA-seq data from Loven *et al.* (2012) to identify genes resistant to MYC’s transcriptional amplifier effect. These genes serve as normalization references (housekeeping genes) for downstream analysis.
   
2. **Normalize RNA-seq Data**: Incorporate MYC-resistant housekeeping genes into the normalization process, replacing standard size factor estimation in DESeq2.

3. **Analyze Differential Expression**:
   - Compare MYC-low vs. MYC-high cells under DMSO and SAEi treatments.
   - Investigate interaction effects of MYC status and SAEi treatment on gene expression.

4. **Gene Set Enrichment Analysis**: Evaluate Hallmark MYC target genes for enrichment across conditions.

## Viewing rendedered files

Download files from notebooks_rendered and open in web browser to see R code with rendered graphics

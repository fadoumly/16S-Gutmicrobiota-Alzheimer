# Mouse Microbiota Analysis

## Background
This work is part of our multi-omics research project aiming to establish a relationship between gut microbiota composition and Alzheimer’s disease onset. Biological samples (feces) were collected from transgenic (Tg) mice developing tauopathies (Tg4510, hTauP301L) and will be compared with healthy wild-type (WT) control mice.

The analysis focuses on identifying sequences from a specific 16S ribosomal RNA region. During a lab session, we extracted raw DNA from the bacterial microbiota in the cecum of each mouse using the E.Z.N.A. Stool DNA Kit (OMEGA). The extracted DNA was then sequenced on an Illumina MiSeq platform at the ICM (Institut du Cerveau et de la Moelle Epinière, Paris).

## Description
This repository contains an R script (script_16S_R.txt) for analyzing the mouse gut microbiota using the OTU table (see `traitement_16Sseq`).

## Analysis Workflow

1. **Alpha Diversity Indices**
   - Calculates alpha diversity indices, such as richness, Shannon index, and evenness.
   - Results are exported to a text file for further analysis.

2. **Alpha Diversity Visualizations**
   - Generates bar plots to visualize richness, evenness, and the Shannon index across different thresholds.

3. **Beta Diversity and Hierarchical Clustering**
   - Computes the Bray-Curtis dissimilarity matrix.
   - Performs hierarchical clustering and generates a dendrogram.
   - Visualizes results using a heatmap.

4. **Redundancy Analysis (RDA)**
   - Imports OTU data and explanatory variables.
   - Centers and scales data for analysis.
   - Runs RDA to examine relationships between explanatory variables and OTUs.


# MRG-Bioinformatics
Current list of work being carried out in the MRG in Bioinformatics

---

## Jess Tarn / Dennis Lendrem
* GLM Code support - Useful collaboration for Arthur's eQTL Projects

---

# Long Term Projects
## Faye Cooles - NanoString
* Evaluate Raw Data Distribution
* Design model for experimental design - Question 5 still to go
* Assess suitability of DESeq2 as analysis framework for NanoString Data
  * Check NanoStringNorm, and normalise using housekeepers (geometric mean)
  * Limma Voom (Don't pre normalise - Size factors, or TMM at most)
* Volcano Plots
* Pairings
* Correlation of Retrotransposon genes against everything else (cor.test)
  * Subset by Cell Type
* IPA
  * PO
* Rubber Duck
* Send results

---

## Fai Ng
### Resolve Therapeutics - qPCR Arrays
* Evaluate Raw Data
* Assess batch effects and suitability of combining Data
* Re-run against original analysis
* Rubber Duck
* Report results

### Tenascin C Project
* Extract Gene expression data in Discovery and Validation data sets
* Test for correlations against phenotype data (waiting for clinical phenotypes of interest)
* Rubber Duck
* Report results

---

## Stuart Watson
### Methylation Arrays
* Inspect Gender specific effects
* Waiting on Stuart to confirm sample-to-sample matchings

---

## John Loughlin
### Jaume Machine Learning
* Test Machine Learning Results against Linear Model tests for differential methylation
* Expectation is that some combinations from Jaume may not be found using typical differential methylation techniques

---

## Louise Reynard
### Methylation Collaboration Project
* Scripps Data
  * Age Regression
* Compile Code for Project
* Migrate to long term github Project
* Document

### Data Queries
* Gene Expression Query from Arthur's Datasets - CD4+/CD8+ for CHST11
* Genotype Query from Arthur's Datasets - See email for list

### mQTL Analysis
* mQTL Pipeline Design (use parts from Arthur's project)
  * Bespoke
  * MatrixEQTL (CRAN)
* Combine Preprocessed Genotype Data - From Rebecca
* Genotype Raw IDAT files (need GenomeStudio, CRLMM is not viable)
* Impute Genotyped IDAT files (1000G Phase 3)

### GEO Data request
* GSE80071
  * Awaiting Contrasts of interest

---

## Sophie Hambleton
### PID Exome Project
* Re-run Joint Genotyping - Waiting on preprocessing.
* Create test that checks relatedness against known pedigrees
* Create Test to detect duplicate sample IDs in pedigree file, that have different family IDs

---

## Arthur Pratt
### T-Cell Dataset
* Query - See email, differential expression test between groupings
* GLM / LM differences based on - x ~ y * z / LRT
* eQTL of ~1000 Genes (ranked by variability)
* Interaction effect research
  * Try Multinomial Log-linear Model for i ~ x * y (i = Disease, x = GE, y = Geno)
  * Implement Logistic regression approach
  * Run over 7,000 gene expression probes ranked by variance
  * Parallelise (40 Threads on Sulaco overnight)
  * Plot top results
    * 15,760,003 Tests - Could be limited using LD and MAF
    * 4 Pass FDR (Not convincing)
    * 67 (-4) P < 0.0001
    * Limited on Power due to Genotype, Disease Split
  * Meeting Friday 2pm


### B-Cell Dataset
* No current Tasks
* Support / teaching of Nish's PhD

---

## Desa Lilic
### CiC Project
* Awaiting Data - Expected mid to end of July

---

## David Young
### NOF OA RNA Seq Dataset
* Genotyping Analysis Results

### 1000 Families miRNA Seq - Tania/Fraser
* Get Raw Data
* Publication Quality Tables and Figures

### DNA Sequencing
* No current Tasks
* Expecting email about meeting

### Cardiff collaboration
* Low frequency support requests

---

## Amanda Villalvilla
### arcOGEN Data Queries
* No tasks

---

## Adrian Falconer
### HT12 Experiment
* Experimental Design Meeting 2pm 25th July 2016
  * 4 Factorials (Stimulations), Time points
  * IPA
    * PO
  * Volcano Plots
  * Take Raw Data / Phenotype data and make archive
  * Preprocess using LumiDat binary

---

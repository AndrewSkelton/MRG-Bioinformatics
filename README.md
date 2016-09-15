# MRG-Bioinformatics
Current list of work being carried out in the MRG in Bioinformatics

---

# Long Term Projects
## Faye Cooles - NanoString
* Differential Expression
  * IGS split by RA/Healthy - Check.
  * All the combinations.
* Assess suitability of DESeq2 as analysis framework for NanoString Data
  * Check NanoStringNorm, and normalise using housekeepers (geometric mean)
  * Limma Voom (Don't pre normalise - Size factors, or TMM at most)
* IPA Training / Teaching


---

## Fai Ng
### Resolve Therapeutics - qPCR Arrays
* Evaluate Raw Data
* Assess batch effects and suitability of combining Data
* Re-run against original analysis
* Rubber Duck
* Report results

---

## Stuart Watson
### Methylation Arrays
* Inspect Gender specific effects
* Waiting on Stuart to confirm sample-to-sample matchings
* Compare SWAN against FunNorm
* Reply to Abstract Query

---

## John Loughlin
### Jaume Machine Learning
* Test Machine Learning Results against Linear Model tests for differential methylation
* Expectation is that some combinations from Jaume may not be found using typical differential methylation techniques

---

## Louise Reynard
### Methylation Collaboration Project
* Compile Code for Project
* Migrate to long term github Project
* Document
* RA Hip RA Knee - Methylation dataset ? - Check which.

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
* Create Test to detect duplicate sample IDs in pedigree file, that have different family IDs
* Find a solution to multiple patient samples in a single run (DNA / Fibroblasts)
* ExomeDepth Strikes back! - Test code and re-implement.
* New RDW file migration causes issues in mass network transfer, waiting on possible solution from NUIT/Arron.
* Non-Coding variant prediction research
* Full implementation of MultiQC
* Gemini testing
  * Comp-Het


---

## Arthur Pratt
### T-Cell Dataset
* Paper Amendments
  * HLA-DRB6
    * Probe Sequence SNPs MAFs
    * Email Arthur with SNP IDs
    * Check for patients with two copies.
    * Exclude HLA regions
  * T-Cell Expression Dataset
    * Parallel eQTL using logistic Regression
    * Parallel eQTL using linear regression
    * Formally produce results table
    * Send through to Arthur
  * B-Cell Expression set
    * Parallel eQTL using logistic Regression
    * Parallel eQTL using linear regression
    * Formally produce results table
    * Send through to Arthur
    * Check RPS26
  * B/T Cell Results
    * Basic Sets comparisons (Union, SetDiff)
    * Check HLA-DRB6 (which )


* Incorporate MAF in somehow
  * Dataset MAF (Use Plink to filter)
  * 1000G PIII MAF (biomaRt?)

* Phil - Methotrexate Queries
  * Add to phenotype data
  * Design LM
  * Test for survival differences
  * Send results through


### B-Cell Dataset
* Support / teaching of Nish's PhD
* Followup Email Helen for B-Cell Data

---

## Desa Lilic
### CiC Project
* Volcano Plots - Make X Axis Static (-10:10?)
* Perform set union for IFNa and IFNg: (CMCa - CMCu) ∪ (HCa - HCu)
  * Check Direction of FC
* Repeat analysis for Fibroblasts
* IFNa Inducible genes from papers sent by Desa
  * Plot - Display between conditions.

---

## David Young
### NOF OA RNA Seq Dataset
* Genotyping Analysis Results

### 1000 Families miRNA Seq - Tania/Fraser
* Get Raw Data - Awaiting Fastq Files
* Publication Quality Tables and Figures

### Exome Sequencing
* Requested Fastq Files

### Cardiff collaboration
* Low frequency support requests

---

## Amanda Villalvilla
### arcOGEN Data Queries
* No tasks

---

## Adrian Falconer
### HT12 Experiment
* Venn Diagrams

---

## Laura Ridgley
### HT12 Experiment
* Set up Pandoc Notes

---

## Colin Shepherd
### NOF OA Dataset Queries
* Methods for quantification
  * Kallisto
  * TPMs
  * DESeq2 trnacript aggregation?

---

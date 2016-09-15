# MRG-Bioinformatics
List of Complete Bioinformatics work

---

## Louise Reynard
### Methylation Collaboration Project - Time Commitment ~4.05 Days
* Scripps Data
  * Transcription Factor Enrichment Analysis
  * Age Regression
    * Beta Query
* Mandy Transcription Factor Enrichment Analysis
  * MSC - chondrocyte
  * MSC - OB
  * MSC - Tenocyte
  * Subset for Final CpG list for original collaboration
* Followup Enrichment analysis (TXF/ ENCODE Chromatin) for DM lists
* San Diego Data
  * Create Pheno table
  * Read in Raw Data, normalise, filter (Sex Chr, MAF, DPVal)
  * PCA
    * Outlier samples (2, NA RA sample, RA Hip Sample)
    * Remove NA samples and RA Hip samples
  * Fit linear Model
    * Differential Methylation of RAHip-RAKnee (and with OA)
    * Significant Probes (3,291, and 212 respectively)
  * mAge/cAge Ratio Regression

### GEO Data request - Time Commitment ~0.15 Days
* Query and Get IDAT files for GSE80071
  * Archive Data
  * Get GEO Phenotype entry to match IDATs
* Query and Get IDAT files for GSE46364
  * Requires collaboration to share IDAT files

### Data Queries - Time Commitment ~0.25 Days
* Gene Expression Query from Arthur's Datasets - CD4+/CD8+ for CHST11
* Genotype Query from Arthur's Datasets - See email for list

---

## Stuart Watson
### Methylation Arrays - Time Commitment ~2.25 Day
* Report results of non-linear effects
* Methods Section writing - Kelly
* Kelly - Data Queries
* Kelly - Cutom Plots

---

## Faye Cooles
### NanoString - Time Commitment ~3.75 Days
* Design model for experimental design
* Assess suitability of DESeq2 as analysis framework for NanoString Data
* Develop Contrasts
* Visualisations
* Export Results
* Discuss results and plan follow up work / analyses
* Pairings
  * Cant be used as the pairings are across scan batches.
* Correlation of Retrotransposon genes against everything else (cor.test)
  * Subset by Cell Type
  * 2 Statistically Significant Results; LTR_5 - MAVS in PDc, and L1-5_UTR - ILF3 in CD4
* Volcano Plots
* Additional Model fit + Term (IGS High Vs IGS Low)
  * RA specific (RA High Vs RA Low)
  * General - RA High Vs (RA Low + HC Low)
* Version 2 of Report
* Version 3 of Report
* IPA Prep
* IPA Run

---

## Sophie Hambleton
### PID Exome Project - Time Commitment ~5 Days
* Re-label mixed samples
* Change ReadGroups - Easier to run preprocessing.
* Implement check for Missing bam files for a given sample map element
* Fix bug in pedigree reporting
  * Split for Families and singletons
  * Issue with sex allocation resolved
  * Gender issue with spaces in Sample Map (implemented in bash)
* 22nd July - Gender Issue on remapped samples - Still Issues, waiting on relatedness check.
  * Samples D180850,GNB051015,GNB120815,NG002,NG003,NG008,NG009 Appear to be wrong post re-label
  * Informed Jon - Waiting for confirmation to send MT Bams
  * Remapping was interpreted the opposite way around
  * Re-Labeled, Applying preprocessing
  * Preprocessing All good
* Preprocessing of August 2016 Batch (9 Samples)
* Joint Genotyping of All samples
  * Known Issues:
    * Gender Mismatch: D180850 (2013December Batch, Logged Gender F, actual M).
    * Relatedness:
      * Issues from AROS batches, but nothing critical that can be altered now.
* Create test that checks relatedness against known pedigrees
* Contact Arron Scott to address copying issue to migrated share
  * Sent through commands used - Waiting on checks.
  * Something still not right - most files copy fine (overnight), however some fail on IO error
    * Isolated to migration, nothing on cluster end to blame
* Mass TAR backup to MRG NAS - Due to complications with RDW, better safe than sorry
  * Tar compression + gz
  * Copy over to MRG NAS once Complete
* Create MRG NAS Share for PID Project
  * Host Alignments
    * Copying 2016 Alignments now
  * Create accounts if needed for share
* Create overview document of Pipeline
  * Photoshop A2


---

## Colin Shepherd
### Data request - Time Commitment ~1.2 Days
* NOF OA RNA Seq data for genes of interest
  * Find transcript ID to gene ID mappings
  * Get TPMs
  * Get Gene Level normalised counts
  * Create output (openxlsx)
  * Send results
  * Additional Gene for Extraction (ALDH1A2)
  * Plotting advice and quick coding
  * Methods section + References
  * Methods section2 + References

---

## John Loughlin
### arcOGEN Data - Time Commitment ~0.6 Days
* Phenotype data requested
* Imputed (1000G Phase 1, GRCh37 Assembly) Data requested
* Data sent through via Globus Online
  * Phenotype Data - Split into two stages
  * Imputed Plink files (fam bed bim), 1000G P1 hg19
* Followup Britt - Phenotype FTP error

---

## Amanda Villalvilla
### arcOGEN Data Queries - Time Commitment ~0.35 Days
* SNP List Extract using Plink / R
  * Create SNP list from email
  * Subset Plink files, create transposed matrix of genotypes
    * Use Plink 1.9 on Sulaco
  * Send Results

---

## Fai Ng
### MSc Supervision - Time Commitment ~6 Days
* Weekly meeting to assess progress and guide
* Low Frequency support

### Tenascin C Project - ~0.25 Days
* Extract Gene expression data in Discovery and Validation data sets
* Test for DE Between Control and PSS
  * Repeat for Discovery and Validation
* Plot Image of TNC expression
* Rubber Duck
* Report results

---

## Jess Tarn
### PSS Datasets - Time Commitment ~0.25 Days
* Normalised, not batch corrected dataset
  * Validation set
  * Discovery set
  * Add to shared drive (pss_archive)

---

## Arthur Pratt
### T-Cell Dataset - Time Commitment ~4.5 Days
* eQTL of ~1000 Genes (ranked by variability)
* Interaction effect research
  * Try Multinomial Log-linear Model for i ~ x * y (i = Disease, x = GE, y = Geno)
  * Implement Logistic regression approach
  * Run over 7,000 gene expression probes ranked by variance
    * Ran over 1,000 probes with low variance - 3 Results, Variance rank seems to work.
  * Parallelise (40 Threads on Sulaco overnight - ~8Hrs)
  * Plot top results
    * 15,760,003 Tests - Could be limited using LD and MAF
    * 4 Pass FDR (Not convincing) - Appears to be systematic (batch corrections? Dataset combination?)
    * 67 (-4) P < 0.0001
    * Limited on Power due to Genotype, Disease Split
  * Meeting Friday 2pm
* Paper Amendments
  * HLA-DRB6
    * Get Probe Quality information
    * 2 Probes available in annotation
    * Lots of SNPs
      * ILMN_2066060 - 11 Overlapping SNPs in 50bp capture seq
      * ILMN_2066066 - 6 Overlapping SNPs in 50bp capture seq
* Birmingham
  * See email (Jane Falconer)
  * Spreadsheet - Two sheets for contrasts from melded T-Cell dataset
* Email Follow Helen
* Copy Number Variation using Plink
  * Can't be done without BirdSuite to call the Copy numbers
  * Birdsuite restricted to Affy and Illumin 660 Quads
  * Emailed Arthur with details

---

# Adrian Falconer
### HT12 Experiment - Time Commitment ~3 Days
* Experimental Design Meeting 2pm 25th July 2016
* Prep Data from IDAT -> S|CPP
* QC
* DE Analysis - Between TPs for each Sample Type
* DE Results (Padj < 0.05 & LFC > 2)
* Create Report in Markdown
  * Compile to PDF
* IPA Prep
* IPA Run
* IPA Training
* Custom Plots
  * XY Scatters (LogFC vs LogFC) * 4

---

## Desa Lilic
### CiC Project - Time Commitment ~7.2 Days
* Awaiting Data - Expected mid to end of July
  * Data arrived Afternoon Thurs 4th August
* Archive Raw Data
* NextSeq Prep
  * Concatenate the 4 lanes for each sample.
  * Data Split onto two flowcells to achieve read numbers
  * Concatenate 8 fq files per sample
* QC
  * Fastqc
  * MultiQC
    * Seems like 2 Donors (6 samples), contaminated based on GC distribution
    * Samples removed (CMCa32/CMCa39) - Anaemic, higher proportion of red blood cells.
* Quantification
  * FMSCluster - Kallisto, against GRCh38 Transcriptome (10 cores per job, 100 bootstraps per sample)
* Differential Expression
  * DESeq2
    * Model of ~Treatment_Disease * CellType
      * Contrasts are far too complex to interpret
      * Model Fit Slow
      * PCA Shows a possible batch effect explained by Extraction variable
        * Effect is due to extraction kit (First one was a trial, Date should still encompass that effect)
    * Model of ~Treatment_Disease + ExtractDate (longer fit ~40mins), doesn't account for batch effect
  * Voom - Much faster
    * Model of ~Treatment_Disease + ExtractDate (subsetting by PBMCs / Fibroblasts)
    * PCA looks good with corrected expression set
    * High differential expression numbers with standard cutoffs (FDR < 0.05 & FC > 1.5), switching to be more stringent
* Write Markdown Report
* Send Markdown Report
* Send PDF Quality Report from GeomeScan
* Send Phenotype File (Output as CSV)
* Add heatmap into the Volcano Mix - Top 100 DE Genes for all Conditions
* Dot Plot Examples of Top 10 per contrasts
* Additional Contrasts - noGOF-CMC in IFNa/g and Unstim
* IPA Prep
* IPA Run
* Heatmap - Something that embodies the whole experiment
  * Adjustments and Customisation.
* Fibroblast Data
  * Extract normalised expression set for Chun
  * Adjust for date effect (could be kit)
  * Appears to be a donor effect between CMC patients, unable to correct
  * May require a paired model :( - Will need to work on designing contrasts between pairs.
* Stimulation Index (SI)
  * Relative logFC for alpha stimuli
* Custom Plots
* Custom Heatmaps

---

## Laura Ridgley
### HT12 Experiment - Time Commitment ~1.5 Days
* Get IDAT files from Array provider
* Create Phenotype table
* LumiDat - IDAT -> SPP/CPP
  * 30 Probes excluded due to low bead numbers
* Generate Script
* Set up basics of the experiment (based on phenotype table)
  * Need to check my assumptions
    * 6 uneven time points
    * 2 Cell types Naive and Memory (B Cells?)
    * Treatment of IL-6 (Paired, w + w/o Stim)
    * Looking for differences in stimulation over time
    * between cell types for now
  * Raw data assessment
  * Normalisation
    * Everything seems normal, PCA needs a lot of factors to make sense
    * Boxplots look a bit variable, likely due to pairs or high background
  * HotellingT2 test
    * Filter? P-Value? - Using HT2 > 500 for now.
  * Linear model
    * Set up as grouped analysis
    * Paired analysis (blocking), will take more work to design contrasts between pairs. edgeR manual has clues.
* Set up Pandoc Notes

---

## David Young
### Exome Sequencing - Time Commitment ~0.05 Days
* Emailed Peter Bell (IGM) - Waiting on dropoff of exome Samples

---

## Drew Rowan
### GEO Upload - ~0.75 Days
* Build GEO Archive
  * Normalised / Raw expression data
  * Phenotype data
* Send to Curators
* Get GEO Accession
  * Forward to Drew
* Hold accession until specified

---

## Dennis Lendrem
### Paper - Time Commitment ~0.25 Days
* Read + Comment Paper
* Added comment about bootstrapping train/ test sets

---

## Administration
### NAS Storage - Time Commitment ~2.25 Days
* Share Creation - PID Project
* Migration - PID Backup and Alignment
  * Transfer took ~ 1 Week
* Monthly Drive Scrubbing
* User Creation - Laura
* Folder in AP_Archive created + populated for Laura's project

### Emails - Time Commitment ~3% per day


### Interviews - Time Commitment 0.75 Days
## Daniel Rico

---

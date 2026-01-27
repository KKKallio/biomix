############
Introduction
############

==============================================
Methods of Omics Technologies
==============================================

Cellular function is often framed by **Central Dogma**: ``DNA ⇌ RNA → Protein``. These biopolymers are specific sequences of nucleotides or amino acids whose order determines structure and function. They interact in complex, dynamic networks to maintain homeostasis, with ``metabolites`` serving as products of metabolism and feeding back to regulate gene expression and protein activity.

**Omics** collectively refers to experimental approaches that characterize these molecular layers on a large scale—such as **genomics**, **transcriptomics**,
**proteomics**, and **metabolomics**. Each omic layer captures a distinct aspect of molecular biology, and together they provide a comprehensive understanding of how biological systems function.

----------------------------------------------
Core Principles of Omics Technologies
----------------------------------------------

Understanding biomolecules requires analytical methods that can detect, identify, and quantify them with precision. Modern omics technologies are built upon several core methods including **probe-based recognition**, **sequencing**, and **spectrometry**.

(1). Probe-based Methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Probe-based methods** detect molecules through specific **binding interactions**.

- **Hybridization:**
  DNA or RNA molecules can bind to complementary sequences. This principle is used in Southern, Northern blots, and FISH (Fluorescence In Situ Hybridization).
- **Protein affinity:**
  Proteins are often detected by antibodies that recognize specific targets. Examples include Western blots and ELISA, and imaging methods such as
  IF (ImmunoFluorescence).

These methods evolved into **Microarray**, where thousands of probes are fixed on a chip. When labeled DNA or RNA binds to these probes.

(2) Sequencing-based Methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Sequencing-based methods** determine the **sequence** of nucleotides in DNA or RNA molecules to analyze genetic and transcriptional information.

- **Sanger sequencing** uses dideoxynucleotide (ddNTP) chain termination to read DNA sequences. It is highly accurate and still used for small-scale validation.

- **Next-Generation Sequencing (NGS)** uses sequencing-by-synthesis with fluorescently labeled reversible terminators to generate millions of short reads in parallel.

- **Third-Generation Sequencing (TGS)** introduced long-read, single-molecule sequencing, represented by **PacBio SMRT** and **Oxford Nanopore** platforms.

    - **PacBio SMRT** detects fluorescent flashes in real time inside nanoscopic chambers, allowing continuous observation of DNA synthesis on individual molecules.

    - **Oxford Nanopore** measures ionic current changes as DNA or RNA molecules pass through a nanopore, which also enables the detection of nucleotide modifications such as methylation.

(3) Spectrometry-based Methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Spectrometry-based methods** identify and quantify molecules by their **physical properties**, such as mass/charge ratio or magnetic resonance.

- **Mass Spectrometry** (MS) detects ionized molecules by their mass/charge ratio (m/z), typically using LC-MS (Liquid Chromatography–Mass Spectrometry) or GC-MS (Gas Chromatography–Mass Spectrometry), with ionization sources such as ESI (Electrospray Ionization) and MALDI (Matrix-Assisted Laser Desorption/Ionization).

- **NMR Spectroscopy** measures the magnetic behavior of atomic nuclei to determine molecular structure, composition, and concentration.

----------------------------------------------
Single-Cell and Spatial Omics Technologies
----------------------------------------------

To capture both single cell information and spatial organization, single-cell and spatial omics technologies have been developed based on three main strategies: **physical separation**, **molecular indexing**, and **image-based detection**. Each approach enables the profiling of individual cells or spatial regions within tissues while preserving biological context.

(1) Physical Separation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Physical separation methods isolate individual cells or specific tissue regions before molecular profiling.

- Single cells can be manually picked using a **micropipette** or sorted automatically using **FACS** (*Fluorescence-Activated Cell Sorting*), which separates cells based on fluorescent markers. (eg. smart-seq)

- For spatially defined sampling, **LMD** (*laser microdissection*) is used to precisely cut and collect cells or regions from tissue sections under a microscope. (eg. Nanostring GeoMx.)

(2) Single-Cell and Spatial Indexing
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In high-throughput single-cell and spatial assays, each cell or tissue position is labeled with a unique barcode that records its identity or spatial coordinates. During library preparation, these barcodes enable molecules from many cells or regions to be pooled together for sequencing and later separated computationally.

- **Microfluidic droplet barcoding** encapsulate individual cell with barcoded beads inside tiny droplets. Each droplet serves as an isolated reaction chamber, where all molecules from that cell are labeled with a unique cellular barcode before sequencing. (eg. 10x Chromium and Drop-seq.)

- **Combinatorial indexing** applies a split-and-pool strategy, in which cells or nuclei undergo repeated rounds of barcoding across wells or plates. Each round adds a new barcode, and the unique combination of these barcodes identifies the cell of origin. (eg. sci-RNA-seq, sci-ATAC-seq, and SHARE-seq.)

- **Spatial barcoding** use a slide carries a predefined barcode that records spatial coordinates, allowing gene expression to be mapped directly back to its original tissue structure. (eg. Slide-seq, 10X Visium, and Stereo-seq.)

(3) Image-based Methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Image-based methods directly visualize molecular features within intact cells or tissues using **high-resolution microscopy** combined with **multiplexed labeling**, enabling simultaneous measurement of molecular identity, abundance, and localization within their native tissue context (eg. seqFISH, MERFISH and CODEX). Image-based methods usually involves **cell segmentation** algorithms in data analysis.

----------------------------------------------
Advances and Integration in Modern Omics
----------------------------------------------

Over the past several decades, omics technologies have transformed from single-target analytical tools into comprehensive, high-throughput platforms that map the molecular landscape of living systems. Driven by advances in detection chemistry, microfluidics, imaging, and computational analysis, modern omics enables measurements across multiple molecular layers, scales, and time points.

- From **low-throughput** to **high-throughput**:
  Early molecular biology methods, such as blotting or Sanger sequencing, analyzed only a few molecules at a time. Modern platforms—including microarrays, Next-Generation Sequencing (NGS), and mass spectrometry can now measure millions of molecular features simultaneously with exceptional sensitivity and precision.

- From **bulk** to **single-cell** and **subcellular** resolution:
  Traditional bulk assays average signals from populations of cells, obscuring cellular heterogeneity. Single-cell and spatial omics now resolve gene expression, chromatin accessibility, protein abundance, and metabolite profiles at single cell level and even specific subcellular compartments.

- From **individual omics** to **integrated multi-omics**:
  Multi-omics strategies, such as combining scRNA-seq with ATAC-seq or integrating proteo-transcriptomics, provide a multidimensional view of cellular regulation by connecting transcriptional, translational, and metabolic processes within the same biological context.

- Incorporating **spatial** and **temporal** dimensions:
  The next generation of omics technologies preserves spatial architecture and captures molecular dynamics over time. By linking molecular profiles to tissue structure and developmental or disease progression, researchers can reconstruct how cells organize, communicate, and evolve within complex biological systems.

Collectively, these advances mark the transition from molecular biology to systems biology, where diverse molecular data are combined to reveal emergent properties of living systems.

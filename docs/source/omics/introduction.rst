############
Introduction
############

Cellular function is often framed by **central dogma**: ``DNA ⇌ RNA → Protein``. DNA and RNA are polymers of nucleotides, and proteins are polymers of amino acids. **sequence** constrains higher-order structure and biological function. In addition, ``metabolites``, produced or consumed by enzymatic reactions, reflect the physiological state of a cell and can regulate gene expression and protein activity through signaling and feedback mechanisms. These molecular layers interact in complex, dynamic networks to maintain homeostasis.

**Omics** collectively refers to experimental approaches that characterize these molecular layers on a large scale—such as **genomics**, **transcriptomics**,
**proteomics**, and **metabolomics**. Each omic layer captures a distinct aspect of molecular biology, and together they provide a comprehensive understanding of how biological systems function.

----------------------------------------------
Core principles of omics
----------------------------------------------

Omics measurements require analytical methods that can detect, identify, and quantify biomolecules reproducibly across many features and samples. Most modern omics platforms rely on three broad measurement principles: probe-based recognition, sequencing, and spectrometry.

(1) Probe-based recognition
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Probe-based recognition** detect molecules through specific **molecular recognition**.

- **Nuclei acid hybridization**
  DNA or RNA molecules can bind to complementary sequences. This principle is used in southern, northern blotting, and fluorescence in situ hybridization (FISH).
- **Protein affinity recognization**
  Proteins are often detected by antibodies that recognize specific targets. Examples include western blotting and ELISA, and imaging methods such as
  immunofluorescence (IF).

These concepts scale to high throughput in **microarrays** (e.g., expression arrays, SNP arrays, DNA methylation arrays) and many **spatial omics** platforms that use large sets of probes to label molecules in tissues.

(2) Sequencing
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Sequencing** read the order of nucleotides in DNA or RNA, enabling the measurement of genetic variation, gene expression, and regulatory features. 

- **Sanger sequencing** uses dideoxynucleotide (ddNTP) chain termination to generate fragments that reveal the DNA sequence. It is highly accurate and still used for small-scale validation.

- **Next-generation sequencing (NGS)** uses sequencing-by-synthesis with fluorescently labeled reversible terminators to generate millions of short reads in parallel.

- **Third-generation sequencing (TGS)** introduced long-read, single-molecule sequencing, represented by **PacBio SMRT** and **Oxford Nanopore** platforms.

    - **PacBio SMRT** detects fluorescent flashes in real time inside nanoscopic chambers, allowing continuous observation of DNA synthesis on individual molecules.

    - **Oxford Nanopore** measures ionic current changes as DNA or RNA molecules pass through a nanopore, which also enables the detection of nucleotide modifications such as methylation.

(3) Spectrometry
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Spectrometry** identify and quantify molecules by their **physical properties**, such as mass/charge ratio or magnetic resonance.

- **Mass spectrometry (MS)** detects ionized molecules by their mass/charge ratio (m/z), typically coupled to chromatography: **liquid chromatography–mass spectrometry (LC-MS)** or **gas chromatography–mass spectrometry (GC-MS)**, with ionization sources such as **electrospray ionization (ESI)** and **matrix-assisted laser desorption/onization (MALDI)**.

- **NMR Spectroscopy** measures the magnetic behavior of atomic nuclei to determine molecular structure, composition, and concentration.

----------------------------------------------
Single-cell and spatial omics
----------------------------------------------

To capture both single cell information and spatial organization, single-cell and spatial omics have been developed based on three main strategies: **physical separation**, **molecular indexing**, and **image-based detection**. Each approach enables the profiling of individual cells or spatial regions within tissues while preserving biological context.

(1) Physical separation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Physical separation methods isolate individual cells or specific tissue regions before molecular profiling.

- Single cells can be manually picked using a **micropipette** or sorted automatically using **fluorescence-activated cell sorting(FACS)**, which separates cells based on fluorescent markers. (eg. palte-based protocol such as smart-seq)

- For spatially defined sampling, **laser microdissection(LMD)** is used to precisely cut and collect cells or regions from tissue sections under a microscope. (eg. Nanostring GeoMx)

(2) Single-cell and spatial indexing
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In high-throughput single-cell and spatial assays, each cell or tissue position is labeled with a unique barcode that records its identity or spatial coordinates. During library preparation, these barcodes enable molecules from many cells or regions to be pooled together for sequencing and later separated computationally.

- **Droplet microfluidics barcoding**: individual cells are encapsulated with barcoded beads in droplets, creating isolated reaction chambers. Molecules from the same cell receive a shared **cell barcode** (often plus unique molecular identifiers, UMIs). (eg. 10x Chromium and Drop-seq.).

- **Combinatorial indexing**: cells or nuclei undergo repeated rounds of split-and-pool barcoding across wells. The unique combination of barcodes identifies the cell of origin. (eg. sci-RNA-seq, sci-ATAC-seq, and SHARE-seq.)

- **Spatial barcoding**: tissue sections are placed on barcoded surfaces so that captured molecules inherit location information. (eg. Slide-seq, 10X Visium, and Stereo-seq.)

(3) Image-based methods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Image-based approaches measure molecular features in situ using multiplexed labeling and microscopy, preserving cellular and tissue architecture. (eg. seqFISH, MERFISH, 10X Xenium and CODEX) Downstream analysis often involves **cell segmentation** and **spatial statistics** to assign signals to cells and quantify spatial patterns.

----------------------------------------------
Advances in modern omics
----------------------------------------------

Over the past several decades, omics have progressed to comprehensive, high-throughput platforms that map the molecular landscape of living systems. Driven by advances in detection chemistry, microfluidics, imaging, and computational analysis, modern omics enables measurements across multiple molecular layers, scales, and time points.

- From **low-throughput** to **high-throughput**:
Classical methods (e.g., blotting and sanger sequencing) quantify a limited number of targets per experiment, whereas modern platforms can profile thousands to millions of features in parallel.

- From **bulk** to **single-cell/subcellular** resolution:
Bulk assays report population averages. Single-cell and spatial omics revealcelluar heterogeneity in gene expression, chromatin accessibility, protein abundance, and sometimes metabolites, enabling identification of rare populations and spatial microenvironments.

- From **single omics** to **multi-omics**:
Combining modalities (e.g., scRNA-seq with ATAC-seq; paired transcriptome–proteome measurements) links regulatory layers and improves mechanistic interpretation by connecting genotype, regulation, and phenotype.

- Incorporating **spatial** and **temporal** dimensions:
Next-generation omics preserves spatial architecture and captures molecular dynamics over time. By linking molecular profiles to tissue structure and developmental or disease progression, researchers can reconstruct how cells organize, communicate, and evolve within complex biological systems.

Collectively, these developments support a shift from descriptive molecular profiling toward systems-level models that explain how molecular networks generate cellular behavior.

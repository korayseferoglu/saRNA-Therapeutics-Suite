# saRNA Therapeutics Suite: Integrated Design & Optimization Platform
An end-to-end bioinformatics ecosystem for the discovery, thermodynamic validation, and bioprocess optimization of Small Activating RNA (saRNA) candidates.



## Suite Overview
This suite bridges the gap between genomic data and laboratory synthesis by providing researchers with high-precision tools for **RNA Activation (RNAa)** drug discovery.

### Advanced saRNA Designer (Scientific AI Edition)
*The core analytical engine for precise candidate scoring.*
- **Thermodynamic Engine:** Implements the **Nearest-Neighbor (NN) Model** using Turner parameters to predict RNA-RNA duplex stability.
- **Calculation Nuances:** Includes **Helix Initiation Penalties** (+3.4 kcal/mol) and **Terminal AU Penalties** (+0.5 kcal/mol) to align with gold-standard tools like ViennaRNA.
- **Regulatory Rules:** Applies **Reynolds (2004)** and **Ui-Tei** asymmetry rules to ensure optimal RISC complex loading.

### saRNA Generator (High-Throughput Screening)
*Massive-scale scanning and selection interface.*
- **Sliding Window Scanning:** Automatically fragments long promoter sequences into customizable target windows (e.g., 21-mers).
- **Candidate Docking System:** Features a unique "Dock" mechanism to temporarily store and compare the most promising leads side-by-side.
- **GC Logic:** Real-time monitoring of GC content (Optimal range: 35-55%) to prevent off-target effects and structural instability.

### saRNA Converter (Bioprocess & Synthesis)
*The final bridge to laboratory execution.*
- **Synthesis Readiness:** Automatically generates the **Guide Strand (Antisense)** in the correct 5' → 3' orientation required for commercial oligo synthesis.
- **Visual Mapping:** Dynamically renders hydrogen-bonding duplex structures for quick verification of hybridization.

---

## Scientific Basis & Methodology
The algorithms in this suite are based on established peer-reviewed literature:
- **Energy Parameters:** Integrated **Mathews et al. (2004)** and **Freier et al. (1986)** nearest-neighbor thermodynamics.
- **RNA Activation:** Optimized for targeting promoter regions as discovered by **Li et al. (2006)** and **Portnoy et al. (2011)**.



## Technical Architecture & Privacy
- **Client-Side Computing:** Built with Vanilla JavaScript to ensure 100% data privacy. No genomic target data is sent to a server; all calculations happen locally in the user's browser.
- **High Performance:** Designed with lazy-rendering and batch pagination to process multi-kilobase genomic sequences without UI lag.
- **Compatibility:** TSV-formatted data exports ensure 100% compatibility with LIMS and electronic lab notebooks (ELN) like Benchling.


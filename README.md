# THESIS STRUCTURE: PHASE TRANSITIONS AND CRITICAL DYNAMICS IN SEEG NETWORKS

## CHAPTER 1: INTRODUCTION AND PHYSICAL-CLINICAL FRAMEWORK

1.1 The brain as a critical complex system: Basic physiology and epilepsy as a phase transition (Medical/physical bibliographic sources).

1.2 From time series to functional networks: Basic concepts of Network Theory applied to brain connectivity (Mathematical definitions conforming to the course).

1.3 Objectives of the work: Mapping the pre-ictal/ictal transition, decoupling from spatial coordinates through purely topological analysis.

## CHAPTER 2: MATERIALS, METHODS, AND COMPUTATIONAL DATA MANAGEMENT

2.1 The sEEG dataset and data extraction: Large-scale file management, memory mapping (mmap_mode), transition window slicing, and channel-wise z-score (Snippet: chunk extraction for RAM optimization).

2.2 Construction of the dynamic network: The signed Pearson correlation tensor ($W_{ij} \in [-1, 1]$). Abandoning the absolute value to discriminate between cooperation and competition (Snippet: sliding window calculation).

2.3 Statistical epochs and artifact removal: Filtering of extracranial channels (POL/ECG) and definition of time windows (Baseline, Premonitory, Onset, Ictal) to stabilize metrics against noise.

## CHAPTER 3: MULTISCALE ANALYSIS OF THE TRANSITION (RESULTS AND DISCUSSION)

### 3.1 Act I (Macroscopic) - Percolation and Criticality

Motivation: Searching for global symmetry breaking.

Results: Behavior of the Giant Connected Component S(t) and Topological Susceptibility.

Criticality: Dependence on the binarization threshold theta.

### 3.2 Act II (Mesoscopic) - Modularity Collapse

Motivation: Investigating the reorganization of functional subsystems.

Results: Modularity Q(t) (Louvain) and community collapse at onset.

Criticality: Limitations of the Louvain algorithm on densely connected graphs.

### 3.3 Act III (Microscopic) - Premonitory Decoupling and Hub Recruitment

Motivation: Isolating the seizure driver nodes (clinical hypothesis).

Results: Eigenvector centrality, identification of anticorrelated isolated channels, and 2D Role Map (Initiators, Amplifiers, Counter-phase).

Criticality: Limitations of clinical prediction, strong inter-patient variability, and lack of validation on inter-ictal epochs far from the seizure.

## CHAPTER 4: CONCLUSIONS AND FUTURE PERSPECTIVES

4.1 Summary of obtained results (Validity of the topological framework).

4.2 Methodological limitations of the exploratory study (Absence of spatial coordinates, non-generalizability as a live diagnostic tool).

4.3 Future developments (Integration of contact map, testing on extended clinical cohorts).

## BIBLIOGRAPHY

Articles on pre-ictal decoupling, modularity, brain percolation, and course lecture notes.

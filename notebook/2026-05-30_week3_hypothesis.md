# Date: 2026-05-30  |  Entry #1  |  Time: [12:30]

## Goal
Write and date my working hypothesis before any data collection begins.

## Hypothesis

Cryptochrome proteins with experimentally supported radical-pair function can be classified from FAD-binding control proteins with an AUC of at least 0.80 using aromatic residue frequency, charged residue frequency, FAD-binding motif presence, metal ion count, and per-residue conservation score. Proteins with higher aromatic and charged residue frequencies, FAD-binding motifs, greater metal ion counts, and stronger conservation near functionally important residues will be more likely to be classified as radical-pair cryptochromes.

## Independent variables
- Aromatic residue frequency (% Trp, Phe, Tyr in the sequence)
- Charged residue frequency (% Asp, Glu, Lys, Arg)
- FAD-binding motif presence (binary: Y/N from HETATM check)
- Metal ion count (from PDB HETATM entries)
- Per-residue conservation score (from MAFFT alignment)

## Dependent variable
The model will predict class membership where cryptochrome with radical-pair function will be represented as, 1, and FAD-binding control with no radical-pair role will be represented as, 0.

## Controlled variables
- Protein family- cryptochromes
- Label assignment standard (positive label requires at least one peer-reviewed citation for radical-pair function — no exceptions)
- Structure source rules (PDB experimental structure preferred; AlphaFold only when no PDB exists, logged consistently)
- Structure source rules (PDB experimental structure preferred; AlphaFold only when no PDB exists, logged consistently)
- Protein size matching (positive and control sets roughly matched by residue count and domain count, so size alone isn't doing the classifying)
- Feature extraction pipeline (same QuantumBioScreen script version on every protein)

## Predicted result
Higher aromatic residue frequency is expected to increase quantum susceptibility by facilitating long-range electron transfer and stabilizing radial-pairs.
Higher charged residue frequency is expected to increase quantum susceptibility by stabilizing electron movement and radical-pair reactions.
Proteins with FAD-binding motifs are expected to have a higher relevancy to quantum phenomena due to the involvement of flavins in radical-pair formation
Higher metal ion frequency is expected to increase electron transfer activity in a protein
Highly conserved residues may indicate important quantum-related structural features preserved through evolution. 
The model will achieve a cross-validated AUC > 0.80 and a p-value < 0.05

## Sources read today
- Lambert, N., Chen, YN., Cheng, YC. et al. Quantum biology. Nature Phys 9, 10–18 (2013). https://doi.org/10.1038/nphys2474
- Thoradit T, Thongyoo K, Kamoltheptawin K, Tunprasert L, El-Esawi MA, Aguida B, Jourdan N, Buddhachat K and Pooam M (2023) Cryptochrome and quantum biology: unraveling the mysteries of plant magnetoreception. Front. Plant Sci. 14:1266357. doi: 10.3389/fpls.2023.1266357
- P. J. Hore, Henrik Mouritsen. 2016. The Radical-Pair Mechanism of Magnetoreception. Annual Review Biophysics. 45:299-344. https://doi.org/10.1146/annurev-biophys-032116-094545

---
*Printed and initialed: ___Isabel Kim____ (Isabel)   Date: ___5/30/2026____*

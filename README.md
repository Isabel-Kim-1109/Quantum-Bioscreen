# QuantumBioScreen

**Machine learning classification of quantum-relevant proteins**
Isabel Kim  |  Stuyvesant High School  |  Mentor: Clara Tucker
Regeneron STS 2027  /  ISEF via Terra NYC

---

## What this project does
QuantumBioScreen is a feature-based classifier that distinguishes cryptochromes
with documented radical-pair function from structurally similar FAD-binding proteins
that lack this quantum-biological role. It compares hand-crafted structural features
against ESM-2 protein language model embeddings (Lin et al., Science 2023).

## Repository structure
- `notebook/`  -- lab notebook entries (one Markdown file per session)
- `data/`      -- protein sequences (FASTA), labels, and feature CSVs
- `src/`       -- Python scripts for feature extraction and classification
- `results/`   -- model metrics, figures, and validation outputs

## Installation
```
pip install biopython scikit-learn transformers torch pandas matplotlib
```

## Usage
```python
python src/quantumbioscreen.py --input data/proteins.fasta --output results/features.csv
python src/esm2_embed.py --input data/proteins.fasta --output data/esm2_embeddings.csv
python src/train_classifier.py --features results/features.csv --labels data/labels.csv
```

## License
MIT License -- free to use, modify, and build on with attribution.
Copyright (c) 2026 Isabel Kim


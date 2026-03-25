# OCR Model

A repository evaluating OCR models through accuracy metrics and error rate analysis.

---

## Testing Methods

### 1. General Performance Evaluation
Calculates overall accuracy and classifies types of recognised characters.

- [Documentation (KRAKEN)](https://github.com/FoNDUE-HTR/Documentation/blob/master/KRAKEN.md)
- [Python split script](https://github.com/FoNDUE-HTR/Documentation/tree/master/split)

### 2. Per-File Error Rate Analysis
Studies each file individually, computing:

| Metric | Description |
|--------|-------------|
| **WER** | Word Error Rate |
| **WACC** | Word Accuracy |
| **CER** | Character Error Rate |

Results are exported as a `.csv` file.

- Method: [kamiCLI](https://github.com/FoNDUE-HTR/kamiCLI) + custom Python script
- *Note: The latest Kraken release now supports these metrics natively.*

---


## Tested Models

| # | Model | Source |
|---|-------|--------|
| 1 | `Gallicorpora+_best.mlmodel` | Pinche & Gabay (2022). *Gallicorpora+*. Zenodo. [doi:10.5281/zenodo.7410529](https://doi.org/10.5281/zenodo.7410529) |
| 2 | `Lamertus_test-10.mlmodel` | [↓ Download](https://github.com/FourbeFlo/OCR_test/releases/download/ml.model/lambertus_test_mai_best.mlmodel) |
| 3 | `Lambertus_03_best.mlmodel` / `gallicorpora_adjuste.mlmodel` | Same model, two repositories: [↓ Lambertus_03](https://github.com/FourbeFlo/Lambertus/releases/download/model/Lambertus_03_best.mlmodel) · [↓ gallicorpora_adjuste](https://github.com/16thExegesisDH/OCR-model/releases/tag/OCR) |
| 4 | `nfd_best.mlmodel` | Provided by S. Gabay |

---

## Results

### Metric Comparison

![Mean of HTR Metrical Analysis](https://github.com/FourbeFlo/OCR_test/blob/fc319c95a30c4b6f40db78a22ab7805ee4da0a48/comparison_metrics2.png)

* Repository
```bibtex
@misc{Goy_OCR_model,
  author={Floriane Goy },
  title={OCR-model for Latin printed book from 16th Century},
  version={1.0},
  address={Genève},
  publisher={université de Genève},
  year={2023-2026},
  url={https://github.com/16thExegesisDH/OC-model},
}
```

* Model
```
Goy, F. (2024). gallicorpora_ajuste (v.1.2.0). Zenodo. https://doi.org/10.5281/zenodo.19218113
```


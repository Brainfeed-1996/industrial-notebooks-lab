# Industrial Notebooks Lab

Portfolio-grade repository of **industrial notebook patterns** for reproducible ML experiments.

## Features

- **Reproducible Experiments**: Versioned data, code, and environment
- **Data Generation**: Synthetic data generators with validation
- **ML Pipelines**: Feature engineering → Training → Evaluation
- **Experiment Reporting**: Automated metrics and visualization
- **CI Integration**: Notebook validation on every commit

## Notebooks

| Notebook | Topic | Status |
|----------|-------|--------|
| `01_experiment_template.ipynb` | Template for reproducible experiments | ✅ Executed |

## Structure

```
industrial-notebooks-lab/
├── notebooks/
│   ├── 01_experiment_template.ipynb
│   └── README.md
├── src/
│   ├── data/           # Data generation utilities
│   ├── features/       # Feature engineering
│   ├── models/         # Model training
│   └── evaluation/    # Metrics and reporting
├── tests/
│   └── test_notebooks.py
├── .github/workflows/
│   └── validate-notebooks.yml
└── README.md
```

## Usage

```bash
# Clone with LFS for large files
git lfs install

# Run notebook
jupyter lab notebooks/01_experiment_template.ipynb
```

## CI/CD

Notebooks are validated on every push:
- ✅ JSON validity check
- ✅ Cell execution verification
- ✅ Output clearing (optional)

## License

MIT

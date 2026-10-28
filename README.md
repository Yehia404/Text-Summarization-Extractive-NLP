# Text-Summarization-Extractive-NLP

An extractive text summarization project that compares transformer-based sentence representations with traditional classifiers. The notebook trains and evaluates two summarization pipelines on CNN/DailyMail data, then exposes the results through an interactive dashboard.

## Run The Notebook

1. Create and activate a Python environment.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open and run all cells in `Extractive_Summarization_Project.ipynb`.

The notebook downloads datasets and transformer models on first use. It also uses `fastcoref` with spaCy for coreference resolution; if the notebook requests a spaCy language model, install the requested model in the active environment before continuing.

## What It Includes

- Dataset loading from CNN/DailyMail
- DistilBERT and MiniLM sentence embeddings
- Logistic Regression and XGBoost model comparison
- ROUGE-based oracle labels and summary evaluation
- Coreference resolution and Maximal Marginal Relevance (MMR)
- NER, TF-IDF keyword extraction, plots, and an interactive dashboard
- Saved models and evaluation outputs in `outputs/`

## Project Artifacts

- `artifacts/NLP Report.pdf`
- `artifacts/Extractive_Summarization.pptx`
- Trained classifier files in `outputs/`

The committed model files are reusable checkpoints. New notebook runs may create additional evaluation files in `outputs/`.
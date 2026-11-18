# Credit Card Fraud Detection

This project uses a credit card transactions dataset to build and evaluate a fraud detection model. It includes data loading, preprocessing, model training, and evaluation.

## Structure

- `src/credit_fraud_detection/`
  - `data.py` - load and summarize dataset
  - `model.py` - train and evaluate model
  - `pipeline.py` - end-to-end training pipeline
  - `storage.py` - model save/load utilities
  - `visualization.py` - plotting utilities
  - `utils.py` - helper functions
- `src/run_pipeline.py` - runnable script for executing the pipeline
- `creditcard.xls` - dataset file

- `requirements.txt` - project dependencies

## How to run

1. Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
   ```
2. Run the pipeline:
   ```bash
   python src/run_pipeline.py
   ```

## Output

- `models/fraud_detector.joblib` — serialized trained model
- Printed dataset summary and evaluation metrics

## Notes

The dataset contains anonymized transaction features `V1` to `V10`, `Amount`, and target `Class`.

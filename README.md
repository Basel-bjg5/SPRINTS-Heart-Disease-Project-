# Heart_Disease_Project
Comprehensive ML pipeline on UCI Heart Disease dataset.

## Structure
- data/: raw + cleaned CSVs
- notebooks/: step-by-step Jupyter notebooks
- models/: saved .pkl pipeline and model
- ui/: Streamlit app (app.py)
- deployment/: ngrok instructions
- results/: evaluation metrics and plots

## Quick start
1. Create virtual env and install:
   pip install -r requirements.txt
2. Put your dataset at data/heart_disease.csv
3. Run preprocessing notebook or:
   python notebooks/01_data_preprocessing.py
4. Train & save model:
   python notebooks/06_hyperparameter_tuning.py
5. Run Streamlit UI:
   streamlit run ui/app.py
6. Optionally run ngrok:
   ngrok http 8501

## Notes
- Target column expected to be `target`. If your dataset encodes disease as 0..4, the pipeline bins to 0/1.

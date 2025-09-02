# Flanker-GPT

This repository contains code and analysis for the Flanker-GPT project, adapted from [nanoGPT](https://github.com/karpathy/nanoGPT).  
The repository provides all code, scripts, and notebooks required to reproduce the results reported in the thesis.

---

## Usage Notes

- All experiments were implemented in **Google Colab** with GPU acceleration.  
- The notebooks assume a Colab environment, including:
  - Google Drive mounting (`/content/drive/MyDrive/...`)
  - File paths that may need to be adjusted for your setup.

If you run locally, please modify the file paths in the notebooks accordingly.

---

## Project Structure

- `model.py` – GPT model adapted from nanoGPT.  
- `flanker_layouts.txt` – Library of 128 symmetric layouts.  
- `trialdata74.csv` – Raw human behavioral logs (if shareable).  
- `notebooks/` – Jupyter notebooks for dataset generation, training, and evaluation.  
  - *Perfect Model.ipynb* – Deterministic baseline.  
  - *Human-Trained Model.ipynb* – Model trained on human data.  
  - *Irrelevant Clutter Model (V1).ipynb* – Noisy IC.  
  - *Flanker Dropout Model (V2).ipynb* – Noisy FD.  
  - *Interference Substitution Model (V3).ipynb* – Noisy IS.  
  - *Probabilistic Corruption Model (V4).ipynb* – Noisy PC.  

---

## Requirements

- Python 3.10  
- PyTorch ≥ 2.0  
- NumPy, Pandas, Matplotlib  

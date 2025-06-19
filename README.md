# Privacy-Preserving Synthetic Data Generation with Variational Autoencoders
This repository implements a synthetic data generation pipeline using a **Variational Autoencoder (VAE)**-based model, titled **Semi-Supervised Learning with Data Augmentation for Tabular Data (SDAT)**. The goal is to generate realistic tabular datasets for privacy-sensitive domains, enabling safe data sharing and augmentation without compromising sensitive information — all while maintaining high utility for downstream machine learning applications.

## 🧠 Project Overview

- Implements a **VAE-based generative model** tailored for tabular data  
- Produces **synthetic data** that mirrors statistical patterns of the real dataset  
- Enables ML model training with only a **0.2%–7.3% accuracy drop** compared to real data  
- Designed for domains where direct access to sensitive data is restricted  


## 🔗 Run on Google Colab

Want to try it without installing anything?

👉 [**Open in Google Colab**](https://colab.research.google.com/drive/1I7UJxNT0hxkZtidL2TCAjZNv4OOXfvXg)

To run it:
1. Click the link above  
2. Click **“Runtime > Run all”** or run step by step  

## 📌 Key Features

- ⚙️ End-to-end pipeline: data loading, preprocessing, training, generation, and evaluation  
- 🔒 Emphasis on **privacy preservation** with strong data utility  
- 📊 Evaluation metrics and visual comparisons of real vs. synthetic data  
- 🧪 All contained within a single Jupyter Notebook for ease of use  

## 💼 My Role in the Project

This was a team project. My contributions included:

- **Designed and implemented** the VAE architecture for tabular data  
- **Led development** of the preprocessing and training pipeline  
- **Evaluated** model performance and synthetic data utility  
- **Created** visualizations and comparisons to validate data quality  

## 📂 Repository Contents

- `synthetic-tabular-data.ipynb` — Full pipeline implementation in one notebook 

## 🛠️ Run Locally (Optional)

If you'd like to run the notebook locally:

```bash
git clone https://github.com/ppanthasen/synthetic-tabular-data.git
cd synthetic-tabular-data
code synthetic-tabular-data.ipynb
```
💡 Make sure you have Jupyter or VS Code with the Jupyter extension installed to run the notebook.

## 📈 Sample Results
![DistCompare1](https://github.com/user-attachments/assets/c58c15de-3ee3-43b2-95ae-d9e7d1b8bc15)
![DistCompare2](https://github.com/user-attachments/assets/7acc98ac-e236-4c4c-a75a-e2c83d236f16)
![DistCompare3](https://github.com/user-attachments/assets/2d460dd2-db0c-4367-803f-efb25dfb2107)

> *Distribution comparisons between original and synthetic data across various feature types, including binary, categorical, and continuous/count-based variables. The synthetic data closely replicates the original distributions, capturing both class proportions and skewed patterns present in real-world tabular data.*

![PCA_comparison](https://github.com/user-attachments/assets/c0eb8c48-3bbe-4996-9b7c-60a6ad735fc4)


> *PCA (left) and t-SNE (right) plots showing the distribution of real (blue) and synthetic (red) data in lower-dimensional space. Significant overlap indicates that the synthetic data successfully captures the global and local structure of the original data.*

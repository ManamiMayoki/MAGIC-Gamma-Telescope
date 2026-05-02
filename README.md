![Stars](https://img.shields.io/github/stars/ManamiMayoki/MAGIC-Gamma-Telescope?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/ManamiMayoki/MAGIC-Gamma-Telescope?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/ManamiMayoki/MAGIC-Gamma-Telescope?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![License](https://img.shields.io/badge/License-Educational-lightgrey)

# MAGIC Gamma Telescope — ML Classification

A machine learning project that classifies telescope events as **Gamma (signal)** or **Hadron (background noise)** using the [MAGIC Gamma Telescope dataset](https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope) from the UCI Machine Learning Repository.

---

## Dataset

| Property | Details |
|----------|---------|
| Source | UCI ML Repository |
| Samples | 19,020 |
| Features | 10 numerical features |
| Classes | Gamma (signal) · Hadron (background) |
| Class balance | ~65% Hadron, ~35% Gamma |

Features include shower width, length, distance, and other parameters extracted from Cherenkov telescope images.

---

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| Random Forest | 87.4% | 86.1% | 85.3% | 85.7% |
| K-Nearest Neighbors | 83.2% | 82.0% | 81.5% | 81.7% |
| Decision Tree | 81.6% | 80.4% | 79.8% | 80.1% |
| Logistic Regression | 79.3% | 78.5% | 77.9% | 78.2% |

> **Best model:** Random Forest with 87.4% accuracy.  
> *(Replace these with your actual results after training.)*

---

## Project Structure

```
magic-ml/
├── data/          # Raw and processed dataset
├── notebooks/     # Exploratory data analysis & experiments
├── src/           # Training and evaluation scripts
├── models/        # Saved trained models
└── results/       # Outputs, metrics, and plots
```

---

## Getting Started

```bash
git clone https://github.com/ManamiMayoki/MAGIC-Gamma-Telescope.git
cd magic-ml
pip install -r requirements.txt
python src/train.py
```

---

## Requirements

```
numpy
pandas
scikit-learn
matplotlib
seaborn
```

Install all at once:
```bash
pip install -r requirements.txt
```

---

## Approach

1. **Exploratory Data Analysis** — understanding feature distributions and class imbalance
2. **Preprocessing** — scaling features, handling imbalance with stratified splits
3. **Model Training** — four classifiers compared side by side
4. **Evaluation** — accuracy, precision, recall, and F1 score

---

## Future Improvements

- [ ] Try neural networks (MLP, CNN on image data)
- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Better handling of class imbalance (SMOTE, class weights)
- [ ] Feature importance analysis

---

## Contributing

Beginner-friendly contributions are welcome! Feel free to open an issue or submit a pull request.

---

## License

For educational and learning purposes only.

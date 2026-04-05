# Priced by Words?
## Flavor Vocabulary and Price Signalling in Specialty Coffee

Computational Social Science WS 2025/26

## Overview

This project investigates whether the language specialty coffee roasters use to describe their products independently predicts price, beyond physical attributes such as origin, processing method, varietal, and roaster brand.

Data was scraped from 32 specialty coffee roasters operating on the Shopify platform across Europe, North America, and Australia. OLS regression models were estimated with full physical controls and five binary vocabulary flags derived from the SCA Coffee Tasters Flavor Wheel. A flavor vocabulary uniqueness score was also constructed using TF-IDF cosine distance as an exploratory measure.

Main finding: vocabulary adds 2.9 percentage points of R2 beyond all physical controls. Floral descriptors are associated with a 13.5% price premium and chocolate descriptors with a 15% discount, both robust across multiple specifications.

---

## Repository Contents

```
specialty_coffee.ipynb    full analysis pipeline (scraping, cleaning, regression, robustness checks, visualisations)
requirements.txt          Python package dependencies
README.md                 this file
```

Raw data (CSV) is not included due to website terms of service. Running the scraper cells in the notebook will reproduce the dataset.

---

## How to Run

1. Clone the repository or download `specialty_coffee.ipynb`
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Open the notebook in Jupyter or Google Colab
4. Run cells in order. The scraper (~5 min) is in Part 1. All subsequent analysis depends on the scraped data so cells must be run sequentially.

Note: Scraping results may differ slightly from the paper depending on when the notebook is run, as roaster catalogues change over time.

---

## Dependencies

Python 3.x. See `requirements.txt` for packages. All standard packages available via pip. No API keys or authentication required.

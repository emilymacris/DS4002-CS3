
#  Presidential Inaugural Speeches: Unification or Polarization?

**A DS 4002 Case Study for Second-Year UVA Students**  
**Instructor: Prof. Loreto Alonzi**  
**Group: Data Destroyers — Karan Rawat, Kelsey Matsik, Emma Mills, Emily Macris**

---

## Project Overview

This case study invites you to explore how presidential rhetoric shapes national discourse. Specifically, you'll investigate whether **Democratic and Republican presidents differ in their use of unifying vs. polarizing language** during inaugural addresses.

Using real-world text data scraped from the UCSB American Presidency Project, you’ll apply core data science skills including:

- Web scraping
- Feature engineering with text
- Exploratory Data Analysis (EDA)
- Logistic regression modeling
- Bias and uncertainty reflection

Your goal is to **reproduce this analysis** and reflect on what your findings suggest about the relationship between language and political identity.

---

##  Repository Structure

The project is organized as follows:

```
ds4002_project1/
│
├── data/
│   ├── speech_data.csv              # Cleaned dataset for modeling
│   └── DATA_APPENDIX.pdf            # Overview of dataset construction
│
├── scripts/
│   ├── scraping_cleaning.ipynb      # Web scraping and feature engineering
│   ├── EDA.ipynb                    # Visualizations and descriptive stats
│   └── analysis.ipynb               # Logistic regression + model evaluation
│
├── HOOK_DOCUMENT.pdf                # 1-page mission document
├── RUBRIC.pdf                       # Assignment instructions and grading rubric
├── README.md                        # You are here
└── LICENSE.md
```

---

##  Getting Started

### 1. **Clone the Repository**
```bash
git clone https://github.com/your-username/ds4002_project1.git
cd ds4002_project1
```

### 2. **Set Up Your Environment**

You'll need Python 3.x and the following packages:

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `scikit-learn`
- `scipy`
- `requests`
- `beautifulsoup4`

To install dependencies:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn scipy requests beautifulsoup4
```

---

## Instructions: What to Do

### Step-by-Step Workflow

1. **Start with `scraping_cleaning.ipynb`**
   - Scrapes speeches from the [UCSB American Presidency Project](https://www.presidency.ucsb.edu/).
   - Counts unifying and polarizing phrases.
   - Outputs a cleaned dataset: `speech_data.csv`.

2. **Move to `EDA.ipynb`**
   - Load the data.
   - Explore relationships between party and language using:
     - Bar plots
     - KDE plots
     - Scatterplots
     - FacetGrids

3. **Use `analysis.ipynb`**
   - Run point-biserial correlation tests.
   - Build a logistic regression model to predict political party.
   - Evaluate using accuracy, confusion matrix, and classification report.
   - Analyze uncertainty using Brier Score and calibration curve (optional).

4. **Read `DATA_APPENDIX.pdf`**
   - Understand how word lists and ratios were constructed.
   - Get context for the `speech_data.csv` file.

---

## Your Final Deliverable

You will submit a **single Jupyter Notebook** that:

- Reproduces the scraping and data engineering process (or uses the CSV)
- Performs and explains EDA
- Builds and evaluates a model
- Includes markdown cells that explain each stage clearly
- Ends with a reflection on bias, uncertainty, and next steps

Refer to `RUBRIC.pdf` for full grading and submission criteria.

---

## Sources

- Speeches collected from: [UCSB American Presidency Project](https://www.presidency.ucsb.edu/documents/app-categories/spoken-addresses-and-remarks/presidential/inaugural-addresses)
- Word lists adapted from prior political discourse research and expanded for educational purposes.

---

##  Learning Outcomes

This case study is designed to help you:
- Practice web scraping and feature extraction
- Understand political communication through data
- Reflect on the limits and biases of automated analysis
- Build confidence in structuring and explaining real-world data workflows

---

## Project Authors

**Data Destroyers**  
University of Virginia — DS 4002 Spring 2025  
- Karan Rawat  
- Kelsey Matsik  
- Emma Mills  
- Emily Macris

---

## 📜 License

This project is released under the MIT License. See `LICENSE.md` for details.

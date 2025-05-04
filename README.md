
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
## 📂 Orientation

### 📄 Hook and Rubric Documents

Hook and Rubric Documents are both located at the top level of this repository.

- [HOOK_DOCUMENT.pdf](./HOOK_DOCUMENT.pdf) will orient you to this Case Study and provide a high-level introduction to the challenge ahead. Start here to understand the scenario and the role you'll take on.
- [RUBRIC.pdf](./RUBRIC.pdf) gives you detailed instructions on deliverables and evaluation criteria. Use this as a reference throughout the project.

Make sure to review these documents thoroughly before you begin — and revisit them as you complete each stage of the assignment.

---

### 📚 Various Materials

Also at the top level is the [`data/`](./data/) and [`scripts/`](./scripts/) folders. These contain the essential materials you’ll need for analysis and understanding.

The `data/` folder includes:
- [speech_data.csv](./data/speech_data.csv): A cleaned dataset of inaugural speeches, prepared for modeling.
- [DATA_APPENDIX.pdf](./data/DATA_APPENDIX.pdf): Describes how the dataset was constructed, including scraping methodology and feature creation.

The `scripts/` folder contains all code for the project:
- [scraping_cleaning.ipynb](./scripts/scraping_cleaning.ipynb): Scrapes and processes the speeches.
- [EDA.ipynb](./scripts/EDA.ipynb): Performs exploratory data analysis with visualizations.
- [analysis.ipynb](./scripts/analysis.ipynb): Runs a logistic regression model and evaluates its performance.





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

**Helpful Resources**
https://www.geeksforgeeks.org/text-classification-using-logistic-regression/#

https://www.r-bloggers.com/2024/08/text-analysis-of-2024-us-presidential-convention-speeches/
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

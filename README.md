# Statistical Analysis of Drug Safety Using Hypothesis Testing

![banner image](images/bannerImage.png)

## Overview
This project applies statistical hypothesis testing techniques to evaluate the safety profile of a pharmaceutical drug using clinical trial data. The goal is to determine whether the drug leads to significantly more adverse effects compared to a placebo.

The analysis is based on a randomized controlled trial dataset and focuses on comparing adverse effects, their frequency, and demographic factors such as age.

---

## Objectives

- Compare the **proportion of adverse effects** between Drug and Placebo groups
- Determine whether the **number of adverse effects** depends on treatment
- Assess whether **age is normally distributed** across groups
- Evaluate whether **age differs significantly** between the two groups

---

## Dataset

The dataset (`drug_safety.csv`) includes:

| Column | Description |
|------|-------------|
| sex | Gender of the individual |
| age | Age of the individual |
| week | Week of drug testing |
| trx | Treatment group (Drug / Placebo) |
| wbc | White blood cell count |
| rbc | Red blood cell count |
| adverse_effects | Presence of at least one adverse effect (True/False) |
| num_effects | Number of adverse effects |

---

## Methodology

The project is structured into four key tasks:

### 1. Two-sample proportions z-test
- Compares the proportion of adverse effects between Drug and Placebo groups

### 2. Chi-square test of independence
- Tests whether the number of adverse effects is independent of treatment group

### 3. Normality testing
- Uses histogram visualisation and Shapiro-Wilk test to assess age distribution

### 4. Mann-Whitney U test
- Compares age distributions between groups (non-parametric test)

---

## Results Summary

| Test | Purpose | Result |
|------|--------|--------|
| Two-sample z-test | Proportion of adverse effects | No significant difference |
| Chi-square test | Association between treatment and number of effects | No association |
| Shapiro-Wilk test | Normality of age | Not normally distributed |
| Mann-Whitney U test | Age difference between groups | No significant difference |

---

## Conclusion

The statistical analysis shows **no significant evidence** that the drug increases adverse effects compared to the placebo. Additionally, age was not found to be a confounding factor in this study.

---

## Tech Stack

- Python
- NumPy
- Pandas
- Statsmodels
- Pingouin
- Seaborn
- Matplotlib

---

## Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/OlumideOlumayegun/statistical-analysis-of-drug-safety-using-hypothesis-testing.git
cd statistical-analysis-of-drug-safety-using-hypothesis-testing
````

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the notebook

```bash
jupyter notebook
```

---

## Project Structure

```
├── dataset/
│   └── drug_safety.csv
├── notebook.ipynb
├── requirements.txt
└── README.md
```

---

## Acknowledgement

This project was completed using resources and guidance provided by **DataCamp**, whose structured learning approach supported the development of practical data science and statistical analysis skills.


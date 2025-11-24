# AI-Fairness360 
# Bias Audit on the COMPAS Recidivism Dataset Using AIF360
# Project Overview

This project conducts a fairness and bias audit of the COMPAS Recidivism dataset using IBM’s AI Fairness 360 (AIF360) toolkit. The primary goal is to assess whether the COMPAS risk scoring system exhibits racial bias—particularly disparities affecting African American defendants.

The work corresponds to Part 3 of the assignment, requiring code implementation, visualizations, and documentation of findings.

Objectives

Load and preprocess the COMPAS dataset.

Use AIF360 to compute fairness metrics such as:

Disparate Impact

Statistical Parity Difference

Equal Opportunity Difference

Average Odds Difference

Visualize disparities between protected and unprotected groups.

Propose mitigation strategies based on empirical results.

Tools & Technologies

Google Colab (execution environment)

Python 3.10+

AIF360 (fairness metric computation & mitigation)

Pandas, NumPy

Matplotlib, Seaborn (visualizations)

scikit-learn

Installation

No virtual environment is needed in Google Colab.
Run this at the top of your notebook:

!pip install aif360
!pip install matplotlib seaborn pandas scikit-learn


If installation errors occur (common with AIF360):

!pip install setuptools wheel
!pip install git+https://github.com/Trusted-AI/AIF360.git

How to Run the Notebook

Open the .ipynb file in Google Colab.

Run the installation cell.

Execute each cell in sequence to:

Load and format the COMPAS dataset

Run fairness metrics

Generate visualizations

Produce the audit report

The notebook is fully self-contained.

Included Visualizations

The Colab notebook contains:

Distribution of risk scores by race

False Positive Rate (FPR) comparison

False Negative Rate (FNR) comparison

Risk score decision boundary plots

Statistical parity bar charts

Disparate impact ratio plot

Confusion matrices for each group
(You can add or remove visualizations as needed.)

Outputs

The notebook generates:

1. Fairness Metric Table

AIF360 metrics including:

Statistical Parity Difference

Disparate Impact

Average Odds Difference

Equal Opportunity Difference

2. Visualizations

Matplotlib/Seaborn charts showing racial disparities.

3. Report (300 Words)

A written summary describing:

Audit findings

Evidence of bias

Ethical risks

Proposed mitigation strategies

Ethical Considerations

This analysis recognizes that algorithms deployed in criminal justice can reinforce unjust systemic disparities if not carefully audited. All results are interpreted within an ethical AI framework emphasizing transparency, fairness, and accountability.

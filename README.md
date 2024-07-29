# Causal Stress Project

This README provides an overview of the project, including how to set it up and run it on macOS, as well as a brief description of the project.
This repository has the code used for the Final Paper Submission from the Statistical Method of Causal Inference course from Vrije Universitet Amsterdam. It is a project made by Dudley Díaz and Emma Klasse. 

For detailed information please refer to the final report in PDF (`results/SMCI Final Assessment.pdf`).

You will find instructions to run the project, but there are a PDF and HTML files that show the code and the results too. Both can be found on the `results` folder.

## Project Description

This project investigates the impact of physical exercise on perceived stress levels among Canadian university students using Coarsened Exact Matching (CEM) and other statistical techniques. The goal is to determine whether higher levels of exercise are associated with reduced perceived stress. The analysis involves matching participants on covariates such as age, sex, ethnicity, international student status, and study program to create balanced treatment and control groups. The primary outcome variable is perceived stress, measured using the Perceived Stress Scale (PSS). Ordinary Least Squares (OLS) regression is used to estimate the treatment effect, and sensitivity analysis is performed to assess the robustness of the findings.

### Key Components:
- **Data Preparation**: Loading and preprocessing the dataset.
- **Matching Techniques**: Applying Coarsened Exact Matching (CEM).
- **Statistical Analysis**: Conducting simple difference-of-means tests, regression-adjusted tests, and sensitivity analysis.
- **Visualizations**: Creating histograms and regression coefficient plots to interpret the results.

## Requirements

To run this project on macOS, you will need the following software installed:

1. **Python 3.x**
2. **R**
3. **Jupyter Notebook**
4. **Python Packages**:
   - pandas
   - numpy
   - scipy
   - statsmodels
   - matplotlib
   - seaborn
   - rpy2

### Installation Instructions

1. **Install Python**:
   - Install Python 3 from the [official website](https://www.python.org/downloads/).

2. **Install R**:
   - Install R from the [official CRAN website](https://cran.r-project.org/).

3. **Install Jupyter Notebook**:
   - Install Jupyter Notebook using pip:
     ```bash
     pip install notebook
     ```

4. **Install Required Python Packages**:
   - Install the required Python packages using pip:
     ```bash
     pip install pandas numpy scipy statsmodels matplotlib seaborn rpy2
     ```

5. **Install Required R Packages**:
   - Open R and install the `cem` package:
     ```r
     install.packages("cem")
     ```

## How to Run the Project

1. **Clone the Repository**:
   - Clone the repository to your local machine using the following command:
     ```bash
     git clone <repository-url>
     ```
   - Navigate to the project directory:
     ```bash
     cd <repository-directory>
     ```

2. **Launch Jupyter Notebook**:
   - Launch Jupyter Notebook in the project directory:
     ```bash
     jupyter notebook
     ```

3. **Open the Notebook**:
   - Open the Jupyter Notebook file (e.g., `matching.ipynb`) and run the cells sequentially to execute the analysis.

## Project Structure

- **data**: Contains the dataset used for the analysis (`02_Student_Mental_Health_2021-10-10.csv`). It also contains a detailed descriptions of the dataset `data/00_ReadMe file_Student_Mental_Health_2022-02-21.pdf` and the mental health scoring.
- **notebooks**: Contains the Jupyter Notebook (`matching.ipynb`) with the analysis code.
- **results**: Contains the output files, including the final assessment PDF (`SMCI Final Assessment.pdf`).

## Data Source

The data used in this project is from the University Student Mental Health [Student_Mental_Health_2021-10-10] by the Behavioural Research on Aging and Illness in Neuropsychology (BRAIN) Lab. The dataset can be found at this [url](https://borealisdata.ca/dataset.xhtml?persistentId=doi:10.5683/SP3/VEIBVL).

## Brief Description of the Analysis

### Introduction

The study investigates the relationship between physical exercise and perceived stress among university students using national survey data. The analysis employs Coarsened Exact Matching (CEM) to create balanced treatment and control groups based on several covariates.

### Methods

- **Coarsened Exact Matching (CEM)**: Used to match participants on age, sex, ethnicity, international student status, and study program.
- **Ordinary Least Squares (OLS) Regression**: Used to estimate the treatment effect on perceived stress.
- **Rosenbaum Sensitivity Analysis**: Conducted to assess the robustness of the findings to unobserved confounding.

### Results

The analysis finds that higher levels of physical exercise are associated with significantly lower perceived stress scores. The results are robust to both observed and unobserved confounding, indicating that exercise effectively reduces stress among university students.

## References

- The project utilizes the Perceived Stress Scale (PSS) and the Godin-Shephard Leisure-Time Physical Activity Questionnaire for measuring stress and physical activity, respectively.
- For detailed information and references, please refer to the final assessment PDF (`SMCI Final Assessment.pdf`).

---

By following the instructions in this README, you should be able to set up and run the project on your macOS system, and explore the impact of physical exercise on perceived stress levels among university students using advanced statistical techniques.

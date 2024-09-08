# Exploratory-Data-Analysis-Mycobacterium_tuberculosis
This project performs exploratory data analysis (EDA) on bioactivity data related to Mycobacterium tuberculosis. The analysis involves cleaning the chemical structure data, generating molecular descriptors (Lipinski's rule of five), and visualizing bioactivity classes using various statistical techniques.
Overview
This project performs exploratory data analysis (EDA) on bioactivity data related to Mycobacterium tuberculosis. The analysis involves cleaning the chemical structure data, generating molecular descriptors (Lipinski's rule of five), and visualizing bioactivity classes using various statistical techniques. This project is a part of computational drug discovery research aimed at identifying potential drug candidates for Mycobacterium tuberculosis.
Project Steps
Data Cleaning:

The dataset contains bioactivity data, including chemical structures represented as SMILES strings.
Cleaned the SMILES data by splitting compound structures and selecting the longest canonical SMILES string for each entry.
Molecular Descriptors Calculation (Lipinski's Rule):

Calculated molecular descriptors such as molecular weight (MW), LogP, number of hydrogen donors, and number of hydrogen acceptors using RDKit.
These descriptors are crucial for evaluating drug-likeness based on Lipinski's rule of five.
Bioactivity Class Analysis:

The dataset is divided into active and inactive bioactivity classes.
Statistical analysis such as Mann-Whitney U tests are used to compare the descriptors between active and inactive compounds.
pIC50 Calculation:

Converted IC50 values to pIC50 values to better assess the potency of the compounds.
Normalized the bioactivity values to avoid excessively high or low outliers.
Data Visualization:

Generated visualizations to explore relationships between molecular descriptors and bioactivity classes.
Boxplots and scatter plots were used to compare molecular weight, LogP, and hydrogen donors/acceptors across active and inactive compounds.

Data Analysis
The key functions in the code include:

lipinski(smiles): Calculates molecular descriptors such as molecular weight (MW), LogP, number of hydrogen donors, and hydrogen acceptors using RDKit.
norm_value(input): Normalizes the standard bioactivity values to avoid extreme outliers.
pIC50(input): Converts IC50 values to pIC50 for better interpretation of compound potency.
mannwhitney(descriptor): Performs Mann-Whitney U tests to determine whether molecular descriptors differ significantly between active and inactive compounds.

Results
The analysis includes the following visualizations:

Frequency of Bioactivity Classes: Shows the distribution of active vs. inactive compounds.
Molecular Weight vs. LogP: Scatter plot visualizing the relationship between molecular weight and LogP for active and inactive compounds.
Boxplots for Molecular Descriptors: Boxplots for molecular weight, LogP, hydrogen donors, and hydrogen acceptors, comparing active and inactive compounds.

Conclusion
This project demonstrates the use of exploratory data analysis techniques to assess the bioactivity of chemical compounds targeting Mycobacterium tuberculosis. The combination of data cleaning, molecular descriptor calculation, statistical testing, and visualization allows for a comprehensive understanding of compound characteristics and their potential as drug candidates.

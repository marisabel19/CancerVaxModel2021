# Mathematical Model of a Personalized Neoantigen Cancer Vaccine and the Human Immune System

Cancer vaccines are an important component of the cancer immunotherapy toolkit, enhancing the immune response to malignant cells by activating CD4+ and CD8+ T-cells.  We present a mechanistic mathematical model describing key interactions of a personalized neoantigen cancer vaccine with the immune system of an individual patient. The model considers the vaccine concentration of tumor-specific antigen peptides and adjuvant, patient's major histocompatibility complexes I and II copy numbers, tumor size, T-cells, and antigen presenting cells. Model simulations predict both immune responses to the vaccine as well as clinical outcome. Our model has the potential to lay the foundation for generating in silico clinical trial data and aid the development and efficacy assessment of personalized cancer vaccines.


### Contents of this repository:
1. Code.nb is a Mathematica notebook with functions to simulate the personalized cancer vaccine model. It additionally contains the code to simulate the results of the section 'Application: impact of cancer vaccine treatment on clinical outcome' in Rodriguez Messan et al. 2021.
2. PRCC-LHS_Code.nb is a Mathematica notebook with Latin Hypercube Sampling (LHS) and Partial Rank Correlation Coefficient (PRCC) functions to perform Global Sensitivity Analysis. The functions have been adapted for the use in Mathematica from an original MATLAB code in http://malthus.micro.med.umich.edu/lab/usanalysis.html
3. Datasets needed to run both codes above: Patients_HLA_BA.xlsx, Tcellscounts.xlsx, and Best-fit_param.xlsx

### Requirements to run the Mathematica Notebook code:
- Wolfram Mathematica 12.0 (or most recent version)
- Download all files and run .nb directly using Mathematica. 
- Make sure all datasets and notebook are saved in the same directory. 
- To run the Code.nb (Shift+Enter to execute each cell):
    1. Download data from this repository (Patients_HLA_BA.xlsx, Tcellscounts.xlsx, and Best-fit_param.xlsx)
    2. Load the datasets using the corresponding cells
    2. Initialize by executing 'Initalization' cell
    3. Estimate patients' tumor size 
    4. Now you can solve the ODE system

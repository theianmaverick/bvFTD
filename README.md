# bvFTD
Design and comparison of machine learning models (logistic regression, LASSO logistic regression, and support vector machine) for prediction of behavioral variant frontotemporal dementia using snRNA gene expression data

Read Me!
Analysis and Code Done by Ian Bartlett
Dataset provided by the .

**Foreword**
In the .zip file you will find all code and datasets needed to replicate this analysis.
The analysis consists of two parts divided by the statistical software used:
1.	Python – Used for loading the large .h5ad object and filtering.
2.	R – Used for statistical analysis, sub-setting, and machine learning.

I worked in python for parts 01-03 and then transitioned to R for the machine learning parts. Many people recommend the opposite, but I felt it was best to suite my particular set of programming skills.  

In the 00_pyth_data_loading folder you will find the first parts of this analysis. Each part is labeled sequentially for a reason; later parts may reference a file, function, or formula written in a prior part. The original data file is found in the python_data folder. This folder will be the house for all the later files written by python as you run the analyses. If a part breaks or is not functional, ensure the paths to the folders are correct and follow your preliminary pathways. 

Comprehensive File List

00_pyth_data_loading
	01_anndata_subsetting.py -> produces normal_Pick_2000genes.h5ad
	02_normalization_test.py -> No file production
	03_aggregation.pv -> produces pseudobulk_expression_final.csv
R enviro
	04_PSEUDOANALYSIS.R -> produces sum_ct.csv and mean_ct.csv
	05_DIFFEXP.R -> oligo_df_final.csv
	06_UNPEN_LOG_REG.R – 08_SVM.R --> use oligo_df_final.csv and produce final model comparison csvs. 


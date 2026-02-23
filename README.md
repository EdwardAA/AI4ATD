**Code Files:**
1.	Curate_Real_Dataset.ipynb
2.	Produce_Simulated_Datasets.ipynb
3.	Train_Systematically.ipynb
4.	Test-Systematic.ipynbs
   
The package performs several operations to train and analyze machine learning models to analyze Alternating Treatment Design (ATD) graphs. All code files were produced in Google Colab. Code file (1) loads published ATD data into a format to be used for testing the models in an (n x 4 x 10) data array. The file also compares expert & MDC ratings and exports disagreements. File (2) uses an autocorrelation model to produce a dataset of simulated ATD graphs according to a set of specified parameters. This dataset is used in file (3) to systematically train feedforward deep neural network machine learning models on each combination of feature engineering techniques, using the Adam optimizer. File (4) uses the curated dataset to test for the generalizability of each of the models and analyze which feature engineering techniques perform better. The file also uses Leave-One-Out Cross Validation (LOOCV) to train models on the curated dataset with each feature engineering technique and fine-tune each of the models trained on simulated data.


<img width="591" height="332" alt="Picture1" src="https://github.com/user-attachments/assets/94789504-1060-4431-93b4-3feaa6222f7e" />

 
**Directories:**
•	Friedel_Data: Contains published ATD data used in curated dataset
•	Hall_Data: Contains published ATD data used in curated dataset
•	Datasets: Contains the curated and simulated datasets used to train & test models
•	Training_Runs: Contains systematic training runs of 32 different models, each
•	Ratings: Contains initial ratings and disagreements for the curated dataset
•	Ground_Truth: Contains reconciled ground truth labels for the curated dataset
•	LOOCV: Contains metrics for each LOOCV training iteration

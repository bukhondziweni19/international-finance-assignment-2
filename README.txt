INFI9X2 International Finance, Assignment 2
Replication of Nazlioglu, Batmaz and Gormus (2025) with an extension to African economies

FILES
  INFI9X2_A2_Replication.ipynb   The analysis notebook (run the cells from top to bottom)
  INFI9X2_A2_Data.xlsx           The data used (Bruegel real effective exchange rates), the paper's
                                 published tables, and the results written by the notebook (sheets R_...)
  null_distributions/            The 1,000 Monte Carlo and 1,000 bootstrap draws for each panel
  figures/                       The figures used in the report (recreated by the notebook)
  requirements.txt               Python packages needed

HOW TO RUN
  1. Unzip everything into one folder. The notebook, the Excel file and the null_distributions
     folder must sit side by side. If the folder is missing, the notebook stops at the Settings
     cell and says which files it cannot find.
  2. Install the packages:  pip install -r requirements.txt
  3. Open the notebook in Jupyter and choose Run All. It takes about one minute.

  The notebook loads the saved null distributions. To regenerate them from scratch, set
  RUN_SIMULATION = True in the Settings cell. This takes several hours (four to five on a typical
  laptop) and gives identical numbers, because every block of replications uses a fixed random seed.

  Close the Excel file before running: the last cell writes the result sheets into it, and Windows
  will not allow that while the file is open in Excel.

DATA SOURCE
  Bruegel Dataset (2012) 'Real effective exchange rates for 178 countries', version of
  11 October 2026, https://doi.org/10.64153/SZCG6180. Sheet REER_MONTHLY_120 (monthly, consumer
  price index based, 120 trading partners). January 1993 to October 2024.

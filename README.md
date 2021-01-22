Analysis code used for "A cautionary note on stop-signal data from the Adolescent Brain Cognitive Development [ABCD] study" [(Bissett, Hagen, Jones and Poldrack, 2020)](https://www.biorxiv.org/content/10.1101/2020.05.08.084707v1)

concat_SST.ipynb takes in raw E-Prime SST data downloaded from the [ABCD Data Repository](https://nda.nih.gov/abcd) using [nda-tools](https://github.com/NDAR/nda-tools) python package, and creates one large data file of all downloaded participants (raw_concat_{date}.csv). 

clean_SST.ipynb further culls these to participants having 360 SST trials present and writes this dataframe to SST_concat_8464_all_rows_all_columns_switched_{date}.csv. It also creates several additional columns that contain information of interest, like `correct_go_response`, which records whether or not the recorded go response was correct. 

SST_problems.ipynb walks through each issue identified in Bissett, Hagen, Jones and Poldrack 2020, and generates the figures in the manuscript. 



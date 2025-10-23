####################################################################
########Steps that need to be done manually#########################
####################################################################

####Use gpCAM Version 8.1.6:
-----------------------------------------------------------------
##############################
For multi-device optimization:
##############################

For n_batch 1
-------------
1. Add .xlsx file from drive "3printers_Oct2024_data_noise_reformattedtasks_all.xlsx" with no additional filename ending in data folder
2. Run Notebook_BOphase-batch1_3printers_notrandomchoice_stationary_withtol notebook.
3. copy new points from "data/data-experiment-"+str(n_batch) to .xlsx file in googledrive for new points and highlight data to be completed in yellow according to print order in metadata_after_BO1.yaml file, e.g. (3,2,1) means the first suggestion goes to printer3 and the second to printer2 and the 3rd to printer1

For n_batch >=2
---------------
1. Add .xlsx file from drive with "_" str(n_batch-1) filename ending
2. run Notebook_BOphase-batch2andfollowing... notebook.
3. copy new points from "data/data-experiment-"+str(n_batch) to .xlsx file in googledrive for new points and highlight data to be completed in yellow according to print order in metadata_after_BO1.yaml file, e.g. (3,2,1) means the first suggestion goes to printer3 and the second to printer2 and the 3rd to printer1

For n_batch >=12
---------------
1. Add .xlsx file from drive with "_" str(n_batch-1) filename ending
2. run Notebook_BOphase-batch12andfollowing... notebook.
3. copy new points from "data/data-experiment-"+str(n_batch) to .xlsx file in googledrive for new points and highlight data to be completed in yellow according to print order in metadata_after_BO1.yaml file, e.g. (3,2,1) means the first suggestion goes to printer3 and the second to printer2 and the 3rd to printer1


###############################
For single-device optimization:
###############################

similar but using Notebook_BOphase-only1-batch1.ipynb and Notebook_BOphase-only1-batch2_and_following.ipynb, where the acquisition function needs to be changed as described in the notebook depending on whether you are running exploration-exploitation or pure exploitation phase.


These files take the raw data from RAND-ALP *** and process and clean them to create ***

Files run in this order \

process.do : merges in end-of-survey comments, destrings variables to convert to numeric, creates useful variables for later use \
labeling.do : add variable and value labels \

export_varaibles.do : Exports variables and variable labels into Excel file \

add_conditions_text.do : Update standardized medical conditions (Q1 variables) with free text information, Must have already run freetext_conditions_clean.R to produce test.csv \

merge.do : Merges hand-coded variables \ 

recodes_full_fml.do : collapse all impairments into binary and put into same direction, creates clean data: hfcs_clean_recodes_full_fml.dta
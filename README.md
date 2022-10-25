# quick-heatmaps-for-field-trials
produces heatmaps for each variable within a dataset to get a quick look at field trials

Mainly to just get a look at everything in your field trial quickly. I used 'openxlsx' to bring in multiple datasets at once and wrote the code so that it could be used in this manner on an excel datafile containing many sheets (each a different trial) to produce heatmaps. Should be relatively stable code, even though it wasnt written in base R.

Very minimal tweaking to this code will be needed by users to begin producing their heatmaps. The code is annotated and should be easy to follow.

Notes:

Line 35 - "for (i in 10:ncol(x)) {"  "10" will need to be changed to the first column number that has variables you want visualized on the heatmap (must be numeric)

Line 37 - make sure "Pass" and "Range" are spelled/capitalized the same in your data file

Line 44 - "path =" should lead to a folder in which you want your heatmaps to be saved to.

Line 50 - users will need to change "phytophthora_field_data" to their own dataset name. Dataset will need to be a nested list of datasets as we have loaded in on Lines 19-27

# tfa_project

Section 001 (Monday)

Team 32

Team Member: Yiyao Qu (yq2331), Ziyi Liu (zl3110)


We have written two separate files to analyze the 311_Service_Requests_2020 dataset. In both files, we did not analyze the full data. Instead, we choose a zip code region (10024), filtered out the data and stored it in a variable called my_zip_dt, and proceeded with the following analysis. 

In the file Top10.ipynb, we used the groupby method in pandas to group my_zip_dt by complaint types. Then we also counted the number of calls in each type of complaint. We stored our result in a variable called type_count. 

In the file Parking.ipybn, we mainly performed two actions. First, in our sub dataset (my_zip_dt), we filtered out the rows of data which has illegal parking complaint, and stored it in park_my_zip. Then we divided the length of the dataset park_my_zip by the length of my_zip_dt to get a number which represent the fraction of illegal parking in all complaints in the zip region. Note that, since the data has no null values, the length of the dataset will represent the number of cases we have. After that, we applied the same action to the full dataset to get the fraction of illegal parking in all complaints in the all zip regions. Finally, we compared these two rate by magnitude. 

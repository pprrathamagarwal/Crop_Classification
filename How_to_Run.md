Make sure you have Columns named as Latitude, Longitude and Crop_Name in your csv files
Manually use find and replace to convert Maize-L, Maize-H to Maize etc.

Rest of the Pipeline:
1. Converts XML to CSV
2. Remove Crops such as Fallow, NA Land or Any other crop with an individual count less than 100.
3. Get the SAR data for these files
4. Structure the SAR data and flatten them
5. Get the GCVI for these files
6. Rename them from Gapfilled_LSMC to GCVI_i
7. Elbow plot, K-Means for Outlier Removals
8. Apply the Crop Taxonomy of Height, Duration, etc. on remaining Crops.
9. Run the RF classifier for results.

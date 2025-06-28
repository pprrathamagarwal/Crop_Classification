Make sure you have Columns named as Latitude, Longitude and Crop_Name in your csv files, Use find and Replace to Standardize Crop Names as per in the file: 10. Crop_Taxonomy 

Rest of the Pipeline:

1. AEZ Identifies different AEZ in a state and then for each district, if there are multiple AEZ, how many % of that AEZ is in that district.
2. Converts XML to CSV
3. Renames columns to standardize, Latitude, Longitude and Crop_Name
4. Remove Crops such as Fallow, NA Land or Any other crop with an individual count less than 250.
5. Get the SAR data for these files
6. Structure the SAR data and flatten them
7. Upload the csv files as an asset to GEE
8. Apply the Cropland Masking to remove the outliers.
9. Rename SAR cols, and remove duplicate columns.
10. Apply the crop taxonomy (please see the Crop_Name value matches in your file, otherwise the columns would be blank)
11. Split the file into train-test split
12. Downsample the data, so that we get balanced datasets/
13. Finally run the RF classifier, added an option to save the classifier as well.


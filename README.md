# nosql-challenge
1. Imported the data from the establishments.json file into a uk_food mongo database using the following command:
    mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json 

2. Confirmed the database and collection were imported successfully and assigned them to variables
3. Added a new restaurant called Penang Flavours using a dictionary of provided data
4. Queried the data for BusinessType 'Restaurant/Cafe/Canteen and found that the BusinessTypeID = 1
5. Used the update_one function to set Penang Flavour's BusinessTypeID to 1
6. Updated the data type of latitude and longitude to double, and rating to integer, and then checked that they were successfully changed

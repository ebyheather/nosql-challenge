# nosql-challenge
Parts 1 and 2: Database Setup and Updates
1. Imported the data from the establishments.json file into a uk_food mongo database using the following command:
    mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json 

2. Confirmed the database and collection were imported successfully and assigned them to variables
3. Added a new restaurant called Penang Flavours using a dictionary of provided data
4. Queried the data for BusinessType 'Restaurant/Cafe/Canteen and found that the BusinessTypeID = 1
5. Used the update_one function to set Penang Flavour's BusinessTypeID to 1
6. Updated the data type of latitude and longitude to double, and rating to integer, and then checked that they were successfully changed

Part 3: Analysis
1. Which establishments have a hygiene score equal to 20: 41 establishments have a hygiene score of 20, first result is The Chase Rest Home
2: Which establishments in London have a RatingValue greater than or equal to 4: 33 establishments, first result is Charlie's
3: What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant Penang Flavours: Lucky Food & Wine, Everest Stores Ltd, Premier Express, Fineway Cash & Carry, TIWA N TIWA African Restaurant Ltd
4: How many establishments in each Local Authority area have a hygiene score of 0? (Sorted from Highest to Lowest)
    The top 10 results listed with name and amount of establishments are:
    Thanet	1130
    Greenwich	882
    Maidstone	713
    Newham	711
    Swale	686
    Chelmsford	680
    Medway	672
    Bexley	607
    Southend-On-Sea	586
    Tendring	542

The analysis we were hired to do for UK magazine "Eat Safe, Love" focused on Food Standards Agency's hygiene ratings. 

First we gathered data from establishments.json into MongoDB database named uk_food and a collection named establishments. Included was the terminal command for data import in a markdown cell within the Jupyter Notebook. Library Import and MongoDB.

This project couldn't have been done without the dependent libraries such as PyMongo for MongoDB interaction and Pretty Print (pprint) for ERD (data display) with the Mongo Client. 

I confirmed the existence of the uk_food database by listing databases in MongoDB. Ensured the presence of the establishments collection within the database. Displayed one document from the establishments collection using pprint. Assigned the collection to a variable for further use.

New information was added to examine a new halal restaurant, "Penang Flavours," in Greenwich, which was  previously unrated. Categorization of the type of establishement was split into "Restaurant/Cafe/Canteen" and updated accordingly along with removing the documents within the data where Dover Local Authority was coded incorrectly. 

I used the update_many query to convert latitude and longitude to decimals as instructed. The same function was used to convert, "Rating Value" to integers. 

This exploratory analysis of "Eat Safe, Love" gave us a vast amount of valuable information. 

Key conclusions and valuable infoormation from this project include:
1. Establishments with a hygeine score equal to 20
2. Establishments with a hygeine score greater than or equal to 4
3. Idenification of the top 5 establishments with a,"RatingValue" of 5, organized by lowest score, and closest to the new restaraunt, "Penang Flavours"
4. Finally, we were asked to determine the number of establishments in each local authority that have a hygeine score of 0.
5. These will be sorted from highest to lowest and the top ten authority areas will be will be printed and flagged. 

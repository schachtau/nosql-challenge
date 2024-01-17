The analysis we were hired to do for UK magazine "Eat Safe, Love" focused on Food Standards Agency's hygiene ratings. 

First we gathered data from establishments.json into MongoDB database named uk_food and a collection named establishments. Included was the terminal command for data import in a markdown cell within the Jupyter Notebook. Library Import and MongoDB.

This project couldn't have been done without the dependent libraries such as PyMongo for MongoDB interaction and Pretty Print (pprint) for ERD (data display) with the Mongo Client. 

I confirmed the existence of the uk_food database by listing databases in MongoDB. Ensured the presence of the establishments collection within the database. Displayed one document from the establishments collection using pprint. Assigned the collection to a variable for further use.

New information was added to examine a new halal restaurant, "Penang Flavours," in Greenwich, which was  previously unrated. Categorization of the type of establishement was split into "Restaurant/Cafe/Canteen" and updated accordingly along with removing the documents within the data where Dover Local Authority was coded incorrectly. 

I used the update_many query to convert latitude and longitude to decimals as instructed. The same function was used to convert, "Rating Value" to integers. 

This exploratory analysis of "Eat Safe, Love" gave us valuable information. 

Establishments with Hygiene Score 20:

Displayed establishments with a hygiene score of 20, providing count, the first document, and a Pandas DataFrame. High-Rated Establishments in London:

Showcased establishments in London with a RatingValue greater than or equal to 4, presenting count, the first document, and a Pandas DataFrame.

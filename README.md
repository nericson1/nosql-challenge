# nosql-challenge

## Description
This repository is constructed in two major parts. Part 1 is `No_SQL_setup_starter.ipynb` and contains the code for creating a MongoDB database called 'uk_food'. This database houses a collection of documents called 'establishments'. A series of document modifications are made, and certain datatypes are changed for use in further analysis. 

Part 2 is `No_SQL_analysis_starter.ipynb` which further utilizes the same 'uk_food' database to conduct an analysis on food establishment quality and demographics. This analysis is created in a variety of ways, including pyMongo queries, pipeline creation, and also utilizes Pandas to turn query results into DataFrames.

## References
Much of what I needed to be successful in this analysis was presented in class notes and many of my questions were answered through discussion with my instructional team. However, after changing datatypes using the .update_many() method, I was unsure how to confirm that the datatype change had been successful. I used the link below to find the $type operator which I used in conjunction with .find_one () to determine that the change was successful. This code can be found in the last cell of the No_SQL_setup_starter file.

Link: https://www.mongodb.com/docs/manual/reference/operator/query/type/

I would also like to note that while the challenge instructions dictate to change the establishments.geocode.latitude and establishments.geocode.longitude fields to the decimal datatype, I decided to instead change them to the double datatype, per conversation with my TA. He advised that for the purpose of the analysis, the double datatype would achieve the same goal as decimal while also being more 'user friendly'.

Movie-Recommendation-Database.

Created the database based on the below background.
In this database, a movie has two attributes: id, title. A possible movie record is as follows: 54796, 2 Days in Paris (2007).

A movie can be categorized into multiple genres. A genre is selected from Action, Adventure, Animation, Children’s, Comedy, Crime and so on. A movie may not have a genre.

A user can give a 5-star scale rating (0-5) to a movie. For instance, User (ID 4) gave 4 stars to Movie “God Father”. A user can only rate a movie once. The database needs to log each rating operation. The database should not allow any out-of-range ratings

A user can also assign a tag to a movie. A user can tag a movie multiple times. For instance, User (ID 20) assigned “very cool” tag to Movie “Mission: Impossible – Ghost Protocol”. Two days later, he added a new tag “unbelievable” to the same movie. Each tag is typically a single word or short phrase. The meaning, value and purpose of a particular tag are determined by each user. The database needs to log each tagging operation.

Created 7 tables (users, movies, taginfo, genres, ratings, tags, hasagenre) based on the devised ER diagram and loaded the data into the tables. Implemented few queries for testing random results and then wrote a query to create a recommendation model using item-based collaborative filtering where the problem statement is as follows:

Given a userID, you need to recommend the movies according to the movies he has rated before. In particular, you need to predict the rating P of a movie i that the user Ua didn’t rate. In the following recommendation model, P(Ua, i) is the predicted rating of movie i for User Ua. L contains all movies that have been rated by Ua. Sim(i,l) is the similarity between i and l. r is the rating that Ua gave to l.

![image](https://user-images.githubusercontent.com/86984222/125174875-1c7c4580-e17d-11eb-8665-92d21a9577a5.png)


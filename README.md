# Netflix-movie-recommender


1. This project is aimed to recommend users the movies they liked to watch based on their watching history and their rating comment to movies they watched. I applied itemCF algorithms for this project, because the number of users is much larger than the number of users, thereofore, the running time would be long if we use UserCF and there will be OOM problem. To avoid the problem, I chose to use ItemCF algorithms, and during this project, I used 4 map/reduce jobs to finish it. 
2. The dataset is provided by Netflix, 18000 records in it, and the enviroment is Docker and Mac OS.
3. The dataset is like raw data:  User_id, Movie_id, Movie_rating
4. I am currently using Mapper-Join to optimize the project, solving OOM problem when there comes huge dataset.

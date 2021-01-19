# AutoEncoder & Recommender System Assignment
Assignment for a Spring 2019 Data Science related course at KAIST
<br>*Author: Willmer R. Quinones*

---
### 	Tasks
Using the [MovieLens 100k dataset](https://grouplens.org/datasets/movielens/100k/) and [Keras](https://keras.io/), build an Autoencoder network to estimate the movie rating for a given user. This assignment is divided into 4 subtasks: 
1. **Simple Autoencoder**: build a simple autoencoder (one -layer encoder and one-layer decoder) to reconstruct the users' ratings.
2. **Deep Autoencoder**: 4-layers encoder and 4-layers decoder, with batch normalization for each layer and a dropout of 50%.
3. **Auxiliary Information**: Adding extra information about the user (i.e. age, gender, and occupation) to try to reduce the loss of the model.
4. **Cold-Start Problem**: To cope with the [cold-start problem](https://en.wikipedia.org/wiki/Cold_start_(recommender_systems)#:~:text=Cold%20start%20is%20a%20potential,not%20yet%20gathered%20sufficient%20information.), I randomly conver the ratings equal to zero by multiplying the original ratings with a mask consisting of 80% zeros and 20% ones for those users which less ratings given.

Finally, retrieved the 10 best movies (according to the model) for a given user.

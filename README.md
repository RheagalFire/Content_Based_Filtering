# Content Based Movie Recommendation Engine
![img1](https://www.vshsolutions.com/wp-content/uploads/2020/02/recommender-system-for-movie-recommendation.jpg)
One popular technique of recommendation/recommender systems is content-based filtering. Content here refers to the content or attributes of the products you like. So, the idea in content-based filtering is to tag products using certain keywords, understand what the user likes, look up those keywords in the database and recommend different products with the same attributes.

Now let’s take an example of recommending the movie based on content filtering.

Assume a person watches a movie  **A**(Avengers) and there exists a sequel to it.It is highly likely that he is going to watch the sequel of movie **A**(say **B**(Age of Ultron)). So based on the description of the movie there would be certain keywords(say *galaxy*,*Nick*,*iron-man*) related to the movie **A** which will map to movie **B**.Using [TF-IDF](https://www.onely.com/blog/what-is-tf-idf/) model we can make a weighted matrix of several keywords and using this matrix we can use [cosine-similarity](https://towardsdatascience.com/understanding-cosine-similarity-and-its-application-fd42f585296a) / [Pearson-coefficient](https://www.includehelp.com/ml-ai/pearsons-correlation-and-its-implication-in-machine-learning.aspx#:~:text=Correlation%3D1%2C%20it%20means%20that,for%20our%20model%20to%20learn.).

Let us suppose A = (1,2,3)  *Keywords Weighted where 1 is the weight of galaxy*

& our movie B = (1,2,4)  *galaxy,Nick keyword is same in A & B*

 ![img](https://camo.githubusercontent.com/0d87ffab6466c5cb906cd55044ae581ed26d74815814b79eb9f5fea7db4fc8c0/68747470733a2f2f73697465732e74656d706c652e6564752f74756473632f66696c65732f323031372f30332f636f73696e652d6571756174696f6e2e706e67)  *which will be close to 1 keeping above values*

Head over to my [notebook](https://github.com/RheagalFire/Content_Based_Filtering/blob/master/Movie_Rec_eng.ipynb) to view in detail analysis of above given maths along with code.

 
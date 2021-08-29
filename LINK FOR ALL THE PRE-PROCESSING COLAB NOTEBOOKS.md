Here are the links for all the data preprocessing google colab notebooks used for preprocessing the data of the project.




Step 1: Clustering of movies(based on their genre):

Embedding vector of dimension 400 was created for each movie on the basis of genre of the movie using SGT(sequence graph transform) algorithm and then the dimension of the vector was reduced to 2 from 400 by using PCA(principal component analysis) algorithm. Then the movies were clustered using the kmeans algorithm on the 2 dimensional embedding vector for each movie using scikit learn kmeans module. Matplotlib library had been used to plot the clusters on the plot. To find the appropriate number of clusters to be formed, elbow method was used. 

Link: [clickhere](https://colab.research.google.com/drive/1RxSPhKid7Bqes8xZ8y8CL6hPlzmwnVTz?usp=sharing)


Step 2: RatedMatrix generation for each cluster:

Based on the clusters formed, unique rating matrices were formed for each cluster group where each matrix contained the ratings given by a user to a movie present in that particular cluster group. These was done using numpy library functions. 

Link: [clickhere](https://colab.research.google.com/drive/1rNL9N_03PBIDJPtrLDC-LovmGb_VglJL?usp=sharing)


Step 3: SVD DataMatrix for each cluster:

SVD (singular value decomposition) algorithm was used to produce SVD matrix for each cluster group. This matrix contain the data that how much relevant a genre is to a movie which is calculated based on the ratings given by users. These matrices are used in the final notebook where cosine similarity will is applied to the data of this matrix and top similar movies will be recommended. 

Link: [clickhere](https://colab.research.google.com/drive/1hLy2f-yIsJxSYkkLQoUpxnfWsvEs96pj?usp=sharing)

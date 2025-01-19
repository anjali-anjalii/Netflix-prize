# Netflix-prize
# Introduction 
In 2006, Netflix held the Netflix Prize completition open to all to find the best algorithm to predict user ratings for films. The prediction was based on the previous ratings from the users of Netflix's movies without any other information about the user or movie. 
The winning team BellKor, led by AT&T Research engineers won the 1 Million dollars prize for 10% improvement on Netflix's existing CineMatch algorithm. 
The Goal of this project is to build a Recommendation System to beat Netflix using sparse methods for recommendation systems. 

# Dataset 
* Movie ratings from 1 to 5 (Average- 3.6)
* 17K+ movies (Average movies seen- 206)
* 99M user ratings (Total 9B entries but only 99M were non-zero)
* 480K viewers

# Algorithms 
We will implement 3 different algorithms for this problem which are well suited for recommendation systems
## The SVD Algorithm
SVD states that any matrix A can be factorized as: A = U<sub>(mxm)</sub>S<sub>(mxn)</sub>Vᵀ<sub>(nxn)</sub>
where U and V are orthogonal matrices with orthonormal eigenvectors chosen from AAᵀ and AᵀA respectively. S is a diagonal matrix with r (rank) elements equal to the root of the positive eigenvalues of AAᵀ or Aᵀ A. 
The SVD algorithm consists of decomposing the user-item interaction matrix into the product of two lower-dimensionality rectangular matrices and then performing their product to predict the values of non-empty cells in the user-movie interaction matrix.

## The SVD++ Algorithm
It is n extension of SVD taking into account implicit ratings. Here, an implicit rating describes the fact that a user rated an item, regardless of the rating value.

## KNN
The KNN algorithm is a KNN based approach that looks at ratings of neighbors to make a prediction. We use cosine similarity for similarity which is efficient with sparse vectors.

# Results
The goal of this project was to study the approach used by the winners of the Netflix prize challenge. 

![image](https://github.com/user-attachments/assets/3d893048-dcdb-4981-ae06-6d574f7c3b6e)


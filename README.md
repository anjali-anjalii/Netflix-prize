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
# The SVD Algorithm
![image](https://github.com/user-attachments/assets/026a329b-c402-49ed-ac21-966936cdff51)
SVD states that any matrix A can be factorized as: A = USVᵀ
where U and V are orthogonal matrices with orthonormal eigenvectors chosen from AAᵀ and AᵀA respectively. S is a diagonal matrix with r (rank) elements equal to the root of the positive eigenvalues of AAᵀ or Aᵀ A. The diagonal elements are composed of singular values i.e. an m× n matrix can be factorized as: A<sub>(mxn)</sub> = U<sub>(mxm)</sub>S<sub>(mxn)</sub>Vᵀ<sub>(nxn)</sub>

# The SVD++ Algorithm

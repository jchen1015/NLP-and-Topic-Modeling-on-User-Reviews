# NLP-and-Topic-Modeling-on-User-Reviews

This an unsupervise learning project to clustered customer reviews into groups and discovered the latent semantic structure. The dataset is an e-commerce product data from http://s3.amazonaws.com/amazon-reviews-pds/readme.html.

## Steps of clustered customer reviews:
- Preprocessing review text by tokenization, stemming, removing stop words an extracted features by Term Frequency - Inverse Document Frequency.
- Training unsupervised learning models of K-means clustering and Latent Dirichlet Analysis. 
- Identifying latent topic and keywords of each review for clustering.

## K-means Clustering
Number of clusters is 10. 
- Cluster 0: band,look,leather,wrist,good,nice
- Cluster 1: great,look,price,comfort,product,work
- Cluster 2: work,look,time,use,day,good
- Cluster 3: good,product,price,love,big,qualiti
- Cluster 4: excel,product,price,fast,qualiti,good
- Cluster 5: like,look,work,face,nice,big
- Cluster 6: nice,price,look,realli,good,love
- Cluster 7: perfect,beauti,fit,wear,great,realli
- Cluster 8: love,wife,husband,look,color,gift
- Cluster 9: expect,clock,everyth,thank,nice,time

|     |Cluster|
|-----|-------|
|2    |429    |
|8    |97     |
|0    |91     |
|7    |77     |
|1    |70     |
|5    |64     |
|3    |63     |
|6    |55     |
|4    |30     |
|9    |24     |

Since number of review text between clusters is very different, I decide to move on to Latent Dirichlet Allocation. 

## Topic Modeling -- Latent Dirichlet Allocation


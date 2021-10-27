# NLP-and-Topic-Modeling-on-User-Reviews

This an unsupervise learning project to clustered customer reviews into groups and discovered the latent semantic structure. The dataset is an e-commerce product data from http://s3.amazonaws.com/amazon-reviews-pds/readme.html.

## Steps of clustered customer reviews:
- Preprocessing review text by tokenization, stemming, removing stop words an extracted features by Term Frequency - Inverse Document Frequency.
- Training unsupervised learning models of K-means clustering and Latent Dirichlet Analysis. 
- Identifying latent topic and keywords of each review for clustering.

## K-means Clustering
Number of clusters is 10. 
- Cluster 0: like, perfect, expect, qualiti, want, awesom
- Cluster 1: work, great, stop, use, good, batteri
- Cluster 2: great, look, price, product, love deal
- Cluster 3: excel, product, price, fast, good, qualiti
- Cluster 4: nice, price, look, love, money, like
- Cluster 5: look, nice, like, great, good, realli
- Cluster 6: good, product, price, qualiti, love, time
- Cluster 7: time, band, use, day, easi, read
- Cluster 8: beauti, love, great, wear, time, heavi
- Cluster 9: love, gift, wife, absolute, color, bought

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

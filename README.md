# NLP-and-Topic-Modeling-on-User-Reviews

This an unsupervise learning project to clustered customer reviews into groups and discovered the latent semantic structure. The dataset is an e-commerce product data from http://s3.amazonaws.com/amazon-reviews-pds/readme.html.

## Steps of clustered customer reviews:
- Preprocessing review text by tokenization, stemming, removing stop words an extracted features by Term Frequency - Inverse Document Frequency.
- Training unsupervised learning models of K-means clustering and Latent Dirichlet Analysis. 
- Identifying latent topic and keywords of each review for clustering.

## K-means Clustering
Number of clusters is 5. 
- Cluster 0: good,product,look,qualiti,price,recommend
- Cluster 1: love,gift,husband,beauti,wife,bought
- Cluster 2: great,look,price,love,work,product
- Cluster 3: nice,look,price,love,realli,like
- Cluster 4: look,like,time,band,work,love

|     |Cluster|
|-----|-------|
|4    |10587  |
|2    |1569   |
|1    |1022   |
|0    |975    |
|3    |847    |

Since number of review text between clusters is very different, I decide to move on to Latent Dirichlet Allocation. 

## Topic Modeling -- Latent Dirichlet Allocation

Split words into 5 topics.

|     |Topic  |
|-----|-------|
|2    |5105   |
|0    |3389   |
|4    |2537   |
|3    |2194   |
|1    |1775   |


|      |Word 0|	Word 1|	Word 2|	Word 3|	Word 4|	Word 5|	Word 6|	Word 7|	Word 8|	Word 9|	Word 10|	Word 11|	Word 12|	Word 13|	Word 14|
|------|------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|---------|---------|---------|---------|
|Topic 0|	great	|beauti	|look	|love	|awesom	|big	|compliment	|husband	|like	|pictur	|lot	|wrist	|watch	|bought	|happi|
|Topic 1|	perfect	|qualiti	|fit	|band	|recommend	|amaz	|small	|cute	|ok	|great	|look	|high	|good	|eleg	|wrist|
|Topic 2|	nice	|time	|band	|look	|like	|day	|wear	|use	|cheap	|strap	|realli	|face	|hand	|broke	|read
|Topic 3|	love	|good	|excel	|price	|gift	|like	|great	|look	|wife	|pretti	|nice	|stylish	|easi	|simpl	|durabl|
|Topic 4|	work	|product	|thank	|great	|batteri	|expect	|time	|arriv	|item	|fast	|cool	|ship	|money	|best	|valu|


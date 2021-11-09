# NLP-and-Topic-Modeling-on-User-Reviews

This an unsupervise learning project to clustered customer reviews into groups and discovered the latent semantic structure. The dataset is an e-commerce product data from http://s3.amazonaws.com/amazon-reviews-pds/readme.html.

## Steps of clustered customer reviews:
- Preprocessing review text by tokenization, stemming, removing stop words an extracted features by Term Frequency - Inverse Document Frequency.
- Training unsupervised learning models of K-means clustering and Latent Dirichlet Analysis. 
- Identifying latent topic and keywords of each review for clustering.

## K-means Clustering
Number of clusters is 7. 
- Cluster 0: love,gift,husband,bought,beauti,wife
- Cluster 1: time,work,beauti,love,look,use
- Cluster 2: great,look,price,love,work,time
- Cluster 3: excel,product,qualiti,recommend,price,good
- Cluster 4: nice,look,price,love,good,like
- Cluster 5: band,like,look,wrist,face,wear
- Cluster 6: good,product,look,qualiti,price,thank

|     |Cluster|
|-----|-------|
|1    |9600   |
|5    |4913   |
|2    |1947   |
|4    |1183   |
|0    |1091   |
|6    |807    |
|3    |459    |

Since number of review text between clusters is very different, I decide to move on to Latent Dirichlet Allocation. 

## Topic Modeling -- Latent Dirichlet Allocation

Split words into 7 topics.

|     |Topic  |
|-----|-------|
|3    |3893   |
|0    |3195   |
|5    |3181   |
|6    |2903   |
|4    |2712   |
|1    |2447   |
|2    |1669   |


|      |Word 0 |	Word 1|	Word 2|	Word 3|	Word 4|	Word 5|	Word 6|	Word 7|	Word 8|	Word 9|	Word 10|	Word 11|	Word 12|	Word 13|	Word 14|
|------|------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|---------|---------|---------|---------|
|Topic 0 |	nice	|price	|great	|look	|good	|qualiti	|product	|recommend	|buy	|like	|best	|high	|valu	|money	|love|
|Topic 1 |	good	|like	|big	|light	|look	|time	|read	|littl	|face	|cute	|easi	|wrist	|realli	|clock	|pretti|
|Topic 2 |	excel	|easi	|use	|casio	|time	|product	|color	|timex	|simpl	|display	|function	|great	|like	|read	|band|
|Topic 3 |	work	|batteri	|time	|band	|day	|return	|month	|year	|use	|broke	|replac	|week	|look	|stop	|set|
|Topic 4 |	band	|look	|strap	|wrist	|wear	|leather	|like	|ok	|small	|face	|great	|nice	|fit	|comfort	|love|
|Topic 5 |	look	|time	|watch	|like	|compliment	|wear	|hand	|great	|mani	|love	|face	|dial	|band	|day	|second|
|Topic 6 |	love	|great	|gift	|beauti	|bought	|thank	|husband	|perfect	|wife	|christma	|son	|happi	|look	|awesom	|friend|


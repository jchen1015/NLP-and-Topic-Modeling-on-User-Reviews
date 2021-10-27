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

Split words into 10 topics.

|     |Topic  |
|-----|-------|
|4    |209    |
|9    |182    |
|5    |112    |
|3    |105    |
|0    |101    |
|1    |86     |
|7    |65     |
|2    |56     |
|8    |54     |
|6    |30     |

|      |Word 0|	Word 1|	Word 2|	Word 3|	Word 4|	Word 5|	Word 6|	Word 7|	Word 8|	Word 9|	Word 10|	Word 11|	Word 12|	Word 13|	Word 14|
|------|------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|---------|---------|---------|---------|
|Topic 0|	beauti|	broke|	batteri|	week|	love|	arriv|	color|	band|	year|	water|	clock|	resist|	fell|	day|	anoth|
|Topic 1|	nice|	awesom|	thank|	amaz|	super|	fast|	price|	ship|	simpl|	set|	love|	look|	great|	instruct|	hard|
|Topic 2|	perfect|	wife|	gift|	love|	worth|	recommend|	happi|	quick|	buy|	alreadi|	movement|	gave|	look|	high|	nice|
|Topic 3|	good|	love|	like|	qualiti|	realli|	pretti|	price|	better|	person|	look|	pictur|	beauti|	time|	month|	came|
|Topic 4|	look|	band|	face|	like|	great|	pictur|	nice|	watch|	cheap|	leather|	feel|	make|	time|	design|	size|
|Topic 5|	great|	excel|	work|	product|	expect|	price|	look|	seller|	exact|	item|	everyth|	perfect|	fit|	valu|	good|
|Topic 6|	strap|	compliment|	invicta|	lot|	buy|	dress|	easili|	everi|	style|	think|	love|	sever|	short|	anoth|	watch|
|Topic 7|	husband|	love|	deliveri|	pleas|	big|	stylish|	heavi|	receiv|	got|	daughter|	look|	piec|	surpris|	beauti|	time|
|Topic 8|	absolut|	wear|	cool|	bought|	want|	love|	bad|	fine|	money|	time|	work|	reason|	swim|	tell|	beauti|
|Topic 9|	use	band|	look|	work|	comfort|	day|	great|	time|	far|	easi|	good|	light|	function|	deal|	like|

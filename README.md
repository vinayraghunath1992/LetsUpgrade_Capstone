# LetsUpgrade_Capstone : Social network Graph Link Prediction - Facebook Challenge
This repo contains Capstone project submitted as a part of LetsUpgrade PGP programme

<h2><b> Problem statement:</b></h2>
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph) <br>
<h2><b> Data Overview </b></h2>
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting data contains two columns source and destination eac edge in graph - Data columns (total 2 columns): - source_node int64 - destination_node int64
<h2><b> Mapping the problem into supervised learning problem: </b></h2>
- Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.<br>
<h3><b> Some reference papers and videos : </b></h3> 
- https://www.cs.cornell.edu/home/kleinber/link-pred.pdf <br>
- https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf<br>
- https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf<br>
- https://www.youtube.com/watch?v=2M77Hgy17cg
<h2><b> Business objectives and constraints:  </b></h2>
No low-latency requirement. <br>
Probability of prediction is useful to recommend highest probability links<br>
<br>
<h3><b>Performance metric for supervised learning:</h3></b>
Both precision and recall is important so F1 score is good choice - Confusion matrix

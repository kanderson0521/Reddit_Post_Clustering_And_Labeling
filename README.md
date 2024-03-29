# Comment Clustering And Labeling from an AskReddit Post

A topic modeling and labeling project aimed to label comments from an AskReddit post asking Redditors, “What is the best advice you can give someone?”. Utilized multiple topic modeling techniques to form topics but the topic results were not coherent. Instead of utilizing the results to label the comments I used them as a form of data exploration and was able to get some of the main ideas. I manually built a topic/keywords dictionary using the top words from the LDA (Latent dirichlet allocation) and NMF (non-negative matrix factorization) models and organized them manually into topics. The topics were: Physical health, Mental health, Interpersonal relationships, Love/Dating, Financial, and Life planning.

Applied labels to the comments with the help of word2vec embeddings and cosine similarity measure. Using word2vec embeddings allowed me to save time building a dictionary of all terms, instead I could measure word similarity of the input word and the keywords to assign the topic. 

<p align="center"> <b> Create topics using the top words from LDA/NMF    -->     Create keyword dict for topics     -->    Label comments based on similarity </b> </p>



## More Information

The data was collected using the Reddit API and PRAW (Python Reddit API Wrapper) to pull comments from a post, https://www.reddit.com/r/AskReddit/comments/pqftho/what_is_the_best_advice_you_can_give_someone/

The pickle files were included for download to avoid having to run some steps. To download Google's pretrained word2vec model used in this project, go here: 
https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?resourcekey=0-wjGZdNAUop6WykTtMip30g

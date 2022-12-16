# ics691B_project

This is the ICS691B Project. 

It's called the AskTheBible. It's a fun project which takes a user's query and returns 3 best hit Bible verses as output. 

This project uses the HuggingFace's all-mpnet-base-v2 sentence transformer (https://huggingface.co/sentence-transformers/all-mpnet-base-v2) to create embeddings of the Bible (King James Version). The program takes a query string as an input and generate 3 verses in the Bible which have the most cosine similarity with the input text's vector. 

The program uses the Kaggle's Bible Corpus's King James Version Bible as the dataset:
https://www.kaggle.com/datasets/oswinrh/bible

Since the Bible data is a big data, the embedding takes a long time to generate. After generating the embeddings, run the last block of code to avoid generating the embeddings again for the query's output. 

The program should show you 3 best hit Bible verses as an output that have the highest cosine similarities with the input text. 

In the program the default query is "How to be a good neighbor?" (which can be found in the last block of code) and the 3 verses are:

1) Romans
Chapter 15 Verse 1
We then that are strong ought to bear the infirmities of the weak, and not to please ourselves.

2) Isaiah
Chapter 41 Verse 5
The isles saw it, and feared; the ends of the earth were afraid, drew near, and came.

3) Exodus
Chapter 20 Verse 16
Thou shalt not bear false witness against thy neighbor.

This program can be improved in the future to answer questions we have in life, using the Bible as our source. It will help users to "get their prayers' answers" in the form of AI, and NLP. 

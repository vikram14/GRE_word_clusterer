# LEARN GRE WORDS EASILY  
When one begins preparation for the GRE (Graduate Record Examinations), one must learn at least 800-1500 words (depending one's own English proficiency). This at first seems like an insurmountable task; however, a large number of these words are related/synonymous. To prepare for my GRE, I thought to exploit this property to make my learning experience much easier.

Natural Language Processing has come a long way in the last 10 years. We no longer use word counts, co-occurrence matrices and tf-idf to represent words. Thanks to the rise of Neural Networks, we now have much more reliable vector representations. I used spacy's pre-trained GLOVE vectors and the cosine-similarity measure to find groups and synonyms in the popular [GregMat Word list](https://docs.google.com/spreadsheets/d/1jRATLVV34vATsL4Y67fZZXQc7qZPYc0c0Yk7Bykh4fw/edit#gid=0), which contains 840 words. Due to this grouping I was able to learn all 840 words in just 12 days. 

To Visualize this grouping, I used t-SNE to reduce the dimensionality of embeddings and then plotted them on a 2D graph to see if clusters exist. The image below was the result.

![Clusters](https://github.com/vikram14/GRE_word_clusterer/blob/master/tSNE-plot1.png)

It is difficult to identify clusters from this graph because 300 random words are projected on to it. Therefore, I decided to take a more organized approach and decided to plot clusters that were relevant. The images below depict the result.

![Clusters](https://github.com/vikram14/GRE_word_clusterer/blob/master/tSNE-plot1.png)

![Table](https://github.com/vikram14/GRE_word_clusterer/blob/master/table.png)

As we can see, the grouping is pretty accurate; However, there are instance when words that antonyms or similar sounding end up together. This happens because a lot of these words are used in the same context as the other. Despite of this drawback, with enough care one can drastically reduce the amount of time spent learning words and instead focus on answering actual questions.

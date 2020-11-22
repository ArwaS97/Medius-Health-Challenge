# Medius-Health-Challenge
Medius Health Data Science Challenge 

By Arwa Siddiqui

-------------------------------------------------------------------------------------------

#### Data Description: 
1. Dataset is provided in “data” folder. Each file in the data folder is considered as a document.
2. There are 300 documents.
3. Each document has some text information.

#### Task Description: Grouping documents with the same semantic description into clusters. 
1. Process the text data in each document/file using NLP, data processing, text mining.
3. Develop a model to partition the data into multiple clusters. It is required to develop the end-to-end model in python instead of using any data clustering libraries or pre-trained models.

The **outcome** of the model: 
1. Number of clusters and the data points in each cluster. 
2. Report the number of clusters found in the data.
3. Find out the topics of each cluster. (You can run any benchmark off-the-shelf topic modelling algorithm like Latent Dirichlet Allocation (LDA) or PLSA)
4. If possible, visualize the cluster.

---------------------------------------------------------------------------------------------

### To answer the challenge, the "Medius Health Challenge.ipynb" has analysis set-up as:
1. **Load imports/libraries**
2. **Process text files/documents to extract information**     
    * Extract files to make dataframe
    * Text mining, use NLTK to tokenize documents, remove stop-words, etc.   
    * Use Stemmer   
    * Use Frequency Dist to plot most common words 
    * Perform TF-IDF Vectorizer
3. **Building K-Means model, without clustering libraries (using sample numeric data)**
    * Create sample data as an example
    * Build K-Means algorithm from scratch 
    * Plot clusters of sample data
4. **Building K-Means model, with clustering libraries (using original text data from (2))**
    * Using *KMeans* from *sklearn* library to model document data
    * Find and plot optimal number of clusters, using Elbow Method  
5. **Perform LDA to find topics in clusters**
6. **Plot TSNE plot to visualise clusters**


Note: "requirements.txt" has also been added to the GitHub. 

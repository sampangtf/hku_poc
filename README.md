# Introducing Clustering to SG's News Digest System

Every day in SG, analysts from the risk department would generate a set of daily market digest, which consists of the most significant financial news based on different regions, including the charts of the day. The daily market digest can allow readers to quickly grasp the latest market information and is widely used by top management executives. However, on average, it normally takes 3-4 hours to produce those reports. Therefore, the risk department is seeking a solution to automate this process to spare more human resources. The Design and Digital Office (DDO) of SG designed and implemented natural language processing (NLP) algorithms inspired by the latest and most popular methodologies to automate the generation of the daily market digest. 

This project would explore the use of clustering algorithm with the latest word embedding methods, aiming to group similar incoming news into clusters. It would streamline the workflow and save analysts’ time, increase market news awareness, and provide better support for market activity monitoring and PNL validation.

# Demonstration
https://hkusg.herokuapp.com/

# Report
To be released

# Description
Here we listed the major parts of our project and where they are located in the github. To understand the implementation details behind them, please read our report.


1) Custom created dataset with 5 classes (Brexit, Cryptocurrency, Electric Vehicle, Hong Kong, US-China), 560 data in total
  
  Location: nlp_data_science/custom_dataset.csv
  
 <br> 
 
2) Evluated 4 word/sentence embeddings models (BERT, Word2Vec, TF-IDF, USE)
  
 Location: nlp_data_science/notebook_wordEmbeddingComparison.ipynb
  
 <br> 
 
3) Explored keyword extraction (Nouns, NERs) to explain different clusters. Merged clusters with recursive clustering approach
  
  Location: nlp_data_science/notebook_keywordExtraction_mergeCluster.ipynb
    
 <br> 
 
4) Output to JSON in NonSQL format
  
  Location: nlp_data_science/outputJSON.ipynb
    
 <br> 
 
5) Frontend Presentation and result evaluation

Location: web/
  
"python app.py" to start the server, localhost:5000 to visit the website locally
 <br> 
 

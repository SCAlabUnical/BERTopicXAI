# Interpreting User Opinions: A Multidimensional Approach Leveraging Explainable AI and Generative Models

## BERTopicXAI

**BERTopicXAI** is an explainable AI methodology that enhances interpretability of BERTopic model by creating visual explanations of a document’s related topics using topic's representative words. This is useful in opinion statements since the statement may talk about multiple aspects. Steps of BERTopicXAI is as follows:

- Identification of top topics related to a document
- Extracting c-TF-IDF scores of the words relative to the topics
- Highlight the representative words of each topic based on their c-tf-idf scores

**Necessary Files**
- A saved BERTopic model
- Dataset used for topic modeling
- A title file including titles of the topics (preferable with a column named "title")
- Optionally a file for selected reviews to create visual interpretation of the top topics



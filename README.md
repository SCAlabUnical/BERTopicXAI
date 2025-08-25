# BERTopicXAI

**BERTopicXAI** is an Explainable AI (XAI) methodology that enhances the interpretability of the BERTopic model by providing visual explanations of documents and their associated topics. Its goal is to bridge the interpretability gap in unsupervised topic modeling methods by offering clear insights into why a document belongs to specific topics.

## 🚀 Key Features

BERTopicXAI has been developed to:
- Identify the main topics of a document based on the probabilities assigned by the BERTopic model.
- Extract the c-TF-IDF scores of the most representative words for each topic.
- Visually highlight the most significant words in analyzed texts, providing a transparent interpretation of topic assignments.

## 📌 Method Flow

The **BERTopicXAI** process consists of three main steps:

1. **Top Topic Identification**: BERTopicXAI calculates the probability of topics for each document using the saved BERTopic model. Topics are ranked by probability and selected based on different coverage methods:
   - Percentile Cut-off
   - Value Cut-off

2. **c-TF-IDF Score Calculation**: The c-TF-IDF matrix is extracted from the BERTopic model, and word scores are normalized to identify the most representative words for each topic.

3. **XAI Representation Generation**: Words in documents are highlighted based on their topic association, with opacity proportional to their relevance.

![motodologiaxai](https://github.com/user-attachments/assets/8efa0f20-5ce1-45d0-824e-600d60450abb)

## 📂 Required Files

To run BERTopicXAI, the following files are required:
- **Saved BERTopic Model**: A pre-trained model used for topic assignment.
- **Dataset**: The documents used for analysis.
- **Titles File**: A file assigning a title to each topic, preferably with a column named `title`.
- **Selected Reviews File** *(optional)*: A file containing a set of documents for which visual explanations will be generated.

### Repository Files:
The following files are included in this repository:

- **`BertopicXAI.ipynb`**: Jupyter Notebook containing the implementation of BERTopicXAI.
- **`hotel_revs_topic_model.csv`**: Dataset containing hotel reviews and their associated topics.
- **`selected_reviews77_initial_probs-dimensions-interpretability.csv`**: A dataset with preprocessed selected reviews, including initial topic probabilities and interpretability scores.
- **`titles_df10.csv`**: A file mapping topic numbers to their respective titles.
- **`Bertopic_implementation.ipynb`** Jupyter Notebook containing the implementation of BERTopic with selected parameters.

## 📊 Example Output

The output of BERTopicXAI is a textual visualization where the most significant words are highlighted in different colors, representing the topics they belong to.

![esempio1](https://github.com/user-attachments/assets/f41966d7-940f-4e1b-8d8e-6befce04d925)


## 📖 Reference Papers

BERTopicXAI was introduced in the following paper:

> **Cosentino, C., Gündüz-Cüre, M., Marozzo, F., & Öztürk-Birim, Ş. (2024)**, *Exploiting Large Language Models for Enhanced Review Classification Explanations Through Interpretable and Multidimensional Analysis*, International Conference on Discovery Science, Springer.

This work is currently under review:

> **Cosentino, C., Gündüz-Cüre, M., Marozzo, F., & Öztürk-Birim, Ş. (2025)**, *Interpreting User Opinions: A Multidimensional Approach Leveraging Explainable AI and Generative Models.*

## 📌 Citation
If you use BERTopicXAI in your research, please cite our paper:

```bibtex
@inproceedings{cosentino2024exploiting,
  title={Exploiting Large Language Models for Enhanced Review Classification Explanations Through Interpretable and Multidimensional Analysis},
  author={Cosentino, Cristian and G{"u}nd{"u}z-C{"u}re, Merve and Marozzo, Fabrizio and {"O}zt{"u}rk-Birim, {\c{S}}ule},
  booktitle={International Conference on Discovery Science},
  pages={3--18},
  year={2024},
  organization={Springer}
}
```

## 📜 License
BERTopicXAI is released under the MIT license. Feel free to contribute and improve the project!

---

If you have any questions or suggestions, open an issue in the repository or contact us by e-mail cristian.cosentino@unical.it ! 🚀

# **Book Recommendation Systems 📚**
## **Introduction:** 
Recommendation systems have become a powerful tool for guiding users through the extensive world of digital content. In this research, we will focus on a content-based approach, where the system finds the attributes related to the product that the user liked and uses this information to recommend other products with similar features. 
We will focus on book plot summaries, using NLP methods to extract meaningful features. The primary objective of this research is to develop three book recommendation algorithms and address their strengths and limitations.

## **Dataset:** 
We used the CMU Book Summary Dataset from Kaggle (https://www.kaggle.com/datasets/ymaricar/cmu-book-summary-dataset). It contains plot summaries for 16 559 books extracted from Wikipedia and their metadata.

## **Three Recommendation Algorithms:**
- **Cosine Similarity of Plots**:
This approach represents each book's plot numerically using TF-IDF and calculates cosine similarity between them to recommend books with similar themes or plots.
- **Named Entities in Plots**:
This approach is focused on extracting named entities (e.g., characters, locations, events) mentioned in the plots and using them to establish similarities between books.
- **Topic Modeling using Latent Dirichlet Allocation (LDA)**:
This approach applies Latent Dirichlet Allocation (LDA) to identify underlying topics in book plots, representing each book's plot as a distribution over these topics.

## **Dependencies**:
### The codes **plot_similarity_Tfidf** and **NER_similarity** have the following dependencies:
- NumPy (np)
- Pandas (pd)
- SpaCy 
- Regular Expressions (re)
- CSV (csv)
- TQDM (tqdm)
- Matplotlib (matplotlib.pyplot)
### The code **LDA_based** has the following dependencies:
- NumPy (np)
- Pandas (pd)
- SpaCy
- Regular Expressions (re)
- CSV (csv)
- TQDM (tqdm)
- pyLDAvis
- Gensim
- Matplotlib

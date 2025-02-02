# **Book Recommendation Systems 📚**

## Overview
This project uses NLP techniques to develop content-based book recommendation systems using plot summaries. We aim to develop three distinct book recommendation algorithms and analyze their strengths and limitations.

## Dataset
**CMU Book Summary Dataset from Kaggle**
The dataset includes plot summaries for 16,559 books along with their metadata extracted from Wikipedia. 
[View Dataset](https://www.kaggle.com/datasets/ymaricar/cmu-book-summary-dataset)

## Recommendation Algorithms
### 1. Cosine Similarity of Plots
- **Description**: Uses TF-IDF to numerically represent each book's plot and calculates cosine similarity between them to identify books with similar themes or plots.
- **Notebook**: [Plot Similarity TF-IDF](plot_similarity_Tfidf.ipynb)

### 2. Named Entities in Plots
- **Description**: Extracts named entities such as characters, locations, and events from the plots, using these to establish similarities between books.
- **Notebook**: [NER Similarity](NER_similarity.ipynb)

### 3. Topic Modeling using LDA
- **Description**: Applies Latent Dirichlet Allocation (LDA) to uncover underlying topics within book plots, representing each plot as a distribution over these topics.
- **Notebook**: [LDA Based](LDA_based.ipynb)

## Material and Method
### TF-IDF and Cosine Similarity
- **Process**: Text data is tokenized, lemmatized, and stripped of non-alphabetic tokens. We employ `scikit-learn`'s `TfidfVectorizer` to transform plot summaries into TF-IDF vectors and compute cosine similarity between them.

### Named Entity Recognition (NER)
- **Tools**: Uses `spaCy` for text preprocessing and entity extraction. Filters named entities based on specific labels to improve the relevance of recommendations.

### LDA and Cosine Similarity
- **Preprocessing**: Text cleaning involves removing stopwords, special characters, and lemmatization. We utilize `Gensim`'s `Phrases` module to detect common phrases and `doc2bow` for creating a bag of words representation for each document.

## Results
Our three book recommendation systems demonstrate varied strengths:
- **Cosine Similarity of Plots**: Effective in identifying thematic similarities and broader themes.
- **Named Entities in Plots**: Excellently identifies and recommends sequels or related books based on character and location entities.
- **Topic Modeling using LDA**: Captures deep thematic consistencies, adept at recommending sequels and thematically related books beyond obvious genre constraints.

## Conclusion
This research highlights the potential of NLP to enhance recommendation systems, particularly effective in addressing the "cold start" problem where little data is available.

# Word2Vec Model with Preprocessing

This project demonstrates the use of Word2Vec for generating word embeddings, along with essential preprocessing steps for text data.

## Preprocessing Steps

1. **Tokenization:**
   - Converts text into individual words (tokens) using NLTK's `word_tokenize`.
   - Lowercases the text for uniformity.
   - Example: "I love NLP" -> ["i", "love", "nlp"]

2. **Lemmatization:**
   - Reduces words to their base form using NLTK's `WordNetLemmatizer`.
   - Groups similar words together.
   - Example: "running" -> "run"

3. **Stop Words Removal:**
   - Eliminates common words (e.g., "the", "a", "is") using NLTK's `stopwords`.
   - Focuses on meaningful words.
   - Example: "The cat is on the mat" -> ["cat", "mat"]

## Word2Vec Model

- Trains a Word2Vec model using Gensim's `Word2Vec` class.
- Learns vector representations (embeddings) for words in the vocabulary.
- Access embeddings using `model.wv[word]`.
- Example:

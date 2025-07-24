# Amazon Customer Review Sentiment Analysis (NLP + Semantic Web)

This project combines Natural Language Processing (NLP) techniques and Semantic Web principles to analyze Amazon customer reviews. The goal is to classify reviews as **positive** or **negative**, extract meaningful entities, and explore relationships between sentiment, product categories, and customer experience.

## 🎯 Objectives

- Analyze unstructured customer reviews from Amazon.
- Classify each review's **sentiment polarity** (positive/negative).
- Apply Semantic Web techniques to enrich the text and link it to structured knowledge.
- Extract key opinionated phrases and insights from customers.

## 🛒 Dataset

- **Source**: Amazon Product Reviews Dataset
- **Fields used**:
  - `ReviewText`
  - `Rating`
  - `Product Category`
  - `Review Title`
  - `Timestamp`

## 🔍 NLP Techniques Used

- Text Cleaning & Tokenization
- Lemmatization / Stopword Removal
- Sentiment Analysis using:
  - TextBlob
  - VADER (Valence Aware Dictionary)
  - Custom Logistic Regression classifier
- Named Entity Recognition (NER)
- Word Clouds & Frequency Analysis
- BERT embeddings (optional advanced layer)

## 🌐 Semantic Web Integration

- Mapping product categories and review content to semantic concepts using:
  - RDF triples (`<Product> hasSentiment <Positive>`)
  - Named Entities as URIs
  - Linking keywords to DBpedia/Wikidata (e.g., `Headphones` → `http://dbpedia.org/resource/Headphones`)
- Building a knowledge graph of reviews and associated metadata.

## 📈 Key Insights

- Products in categories like **Electronics** and **Beauty** tend to have stronger sentiment swings (very positive or very negative).
- Customers who mention **delivery**, **packaging**, or **support** are more likely to leave a **negative** review.
- High-rated reviews (4–5 stars) often contain words like “amazing,” “perfect,” “recommended.”
- Semantic enrichment allows grouping and querying reviews by concepts, not just raw keywords.

## 🧪 Model Evaluation

- Accuracy: ~87%  
- Precision / Recall / F1-Score evaluated using test data
- Confusion Matrix and ROC Curve included

## 📁 Files Included

- `amazon_sentiment_nlp.ipynb` – NLP pipeline and sentiment classification
- `semantic_mapping.ttl` – RDF triples (Turtle format) of enriched data
- `visualizations/` – Word clouds, sentiment distribution charts
- `dataset/` – Raw and preprocessed reviews

## 🧠 What I Learned

- Building an end-to-end NLP pipeline on real-world text data
- Leveraging semantic annotation to add structure to unstructured data
- How sentiment links to business insights (e.g., product improvement, customer satisfaction)
- Creating a foundation for ontology-based recommendation systems

---

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/Amazon-Review-Sentiment-Analysis-NLP.git
cd Amazon-Review-Sentiment-Analysis-NLP
open amazon_sentiment_nlp.ipynb

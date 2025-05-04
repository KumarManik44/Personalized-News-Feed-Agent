# Personalized News Feed Agent

## Overview

This project is an AI-powered **Personalized News Feed Agent** designed to recommend news articles tailored to individual user preferences. It blends **collaborative filtering** with **fine-tuned BERT embeddings** to deliver personalized news recommendations that adapt based on user interactions.

✅ **Key Features:**
- Suggests relevant news articles based on user interaction data (simulated likes, clicks, etc.).
- Extracts deep semantic features using Natural Language Processing (NLP).
- Fine-tunes the BERT model to enhance content-based filtering.
- Combines collaborative filtering and content-based approaches.
- Continuously adapts to user preference changes over time.
- Outputs a personalized feed of top 5–10 recommended articles with summaries.

---

## Project Structure

├── Data/
│ ├── data.csv # Original raw dataset
│ ├── sampled_data.csv # Sample of 1000 cleaned articles for quick testing
│ └── (cleaned_data.csv not uploaded due to file size limits)
├── Notebooks/
│ ├── AI_Agent_1.ipynb # Exploratory Data Analysis & Cleaning
│ ├── AI_Agent_2.ipynb # Fine-tuning BERT embeddings
│ └── AI_Agent_3.ipynb # Generating recommendations
├── README.md
├── requirements.txt

---

## Notebooks Overview

**AI_Agent_1.ipynb**
- Loads and explores the dataset.
- Performs data cleaning (removing nulls, duplicates, etc.).
- Visualizes trends like article categories and length distributions.
- Exports the cleaned dataset for later stages.

**AI_Agent_2.ipynb**
- Fine-tunes the `bert-base-uncased` model using the cleaned dataset.
- Handles tokenization and model training.
- Saves the fine-tuned model for later inference.
- *Note: The trained model is not uploaded to the repo due to file size restrictions.*

**AI_Agent_3.ipynb**
- Loads user profiles and article data.
- Uses collaborative filtering and BERT embeddings to recommend articles.
- Outputs top 5–10 personalized article recommendations per user.

---

## Dataset Info

- **Contents:**
    - `data.csv`: Original raw dataset (uploaded).
    - `sampled_data.csv`: 1000-row sample of the cleaned dataset (uploaded for testing).
    - `cleaned_data.csv`: Full cleaned dataset (not uploaded due to file size limits).

You can recreate the full cleaned dataset by running `AI_Agent_1.ipynb`.

---

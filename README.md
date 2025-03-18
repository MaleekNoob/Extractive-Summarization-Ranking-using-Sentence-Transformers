# YouTube Transcript Ranker
## Overview
This Python package provides a system for semantically ranking and highlighting segments of YouTube video transcripts based on user queries. It uses state-of-the-art sentence embeddings and semantic search to find the most relevant parts of a transcript that match a user's query.

## Features
- ### Semantic Search:
  Finds transcript segments that are conceptually related to the query, not just exact keyword matches.
- ### Diversity Algorithm:
  Uses Maximal Marginal Relevance (MMR) to ensure diverse results
- ### Sentence Ranking:
  Ranks sentences by relevance to the query
- ### Context Highlighting:
  Provides surrounding context for each highlighted sentence
- ### FAISS Integration:
  Leverages FAISS for efficient vector similarity search

## How It Works
- ### Transcript Processing:
  Splits transcript into sentences and generates embeddings using SentenceTransformer
- ### Vector Indexing:
  Stores embeddings in FAISS for fast retrieval
- ### Query Processing:
  Converts user query to an embedding vector
- ### Similarity Searc:
   Finds the most similar transcript segments

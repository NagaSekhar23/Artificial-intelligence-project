# AI Assignment 9: Genetic Algorithms and RAG Systems

This repository contains a Jupyter Notebook implementing two key AI concepts: a Genetic Algorithm for optimization and a Retrieval-Augmented Generation (RAG) system for querying salary data.

## Overview

- **Ai Assignment 9.ipynb**  
  Explores evolutionary computation with a Genetic Algorithm (GA) for the MAX-ONE problem and builds a simple RAG pipeline using embeddings, FAISS retrieval, and Google's Gemini model for natural language queries on a data scientist salary dataset.

## Assignment Details

### Problem 1: Genetic Algorithm for MAX-ONE
- Implements a GA to evolve binary strings toward the optimal solution (all 1s).
- Key components:
  - Fitness function: Count of 1s in the binary string.
  - Selection: Tournament selection.
  - Crossover: One-point crossover.
  - Mutation: Bit-flip with probability.
- Runs for a fixed number of generations or until an optimal solution is found.
- Parameters: String length (L=50), Population size (20), Generations (100), Mutation prob (0.01).
- Outputs progress per generation and final best individual.

### Problem 2: RAG Pipeline for Salary Data Queries
- Builds a Retrieval-Augmented Generation system on a filtered dataset of data scientist salaries (from Stack Overflow survey).
- Key features:
  - Data loading and filtering: Focus on data scientists with valid salary/experience data.
  - Embeddings: Uses Sentence Transformers for vectorizing job descriptions, countries, etc.
  - Retriever: FAISS-based vector search with keyword bonuses for relevance.
  - Generator: Integrates Google's Gemini model to answer queries based on retrieved context.
- Context formatting: Includes averages, ranges, top countries, and sample records.
- Test queries: Demonstrates with homework-style questions (e.g., average salary by experience, top locations).
- Prompt engineering: Strict instructions to use only provided data for accurate, concise responses.

## Requirements

```bash
Python >= 3.8
numpy
pandas
faiss-cpu  # Or faiss-gpu if available
sentence-transformers
google-generativeai  # For Gemini API

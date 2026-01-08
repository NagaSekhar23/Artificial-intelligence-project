# AI Homework 8: Masked Language Modeling and Gemini Chatbot

This repository contains a Jupyter Notebook implementing a simple Masked Language Modeling (MLM) task using PyTorch on a custom dataset, along with integration of Google's Gemini API for a conversational chatbot.

## Overview

- **Ai Homework 8.ipynb**  
  Builds and trains a basic feedforward neural network for MLM on sentences related to the University of Alabama at Birmingham (UAB). It also includes a chatbot powered by Google's Gemini model that maintains conversation history and generates summaries.

## Assignment Details

### Part 1: Masked Language Modeling (MLM) with PyTorch
- **Dataset**: Custom sentences about UAB, professors, students, doctors, and nurses.
- **Preprocessing**: Tokenization, vocabulary building (including 'mask' token), one-hot encoding.
- **MLM Examples**: Generates 1000 masked training examples by randomly masking words in sentences.
- **Model**: Simple Feedforward Neural Network (FFN) with linear layers and ReLU activations.
- **Training**: Uses CrossEntropyLoss and Adam optimizer; processes sentences as matrices of one-hot vectors.
- **Testing**: Predicts masked words in predefined test sentences (e.g., filling "professor", "student", "birmingham").
- **Vocabulary Size**: 36 words.

### Part 2: Gemini-Powered Chatbot
- Integrates Google's Gemini API for natural language responses.
- Maintains conversation history and generates brief summaries after each exchange.
- Handles user inputs in a loop until 'exit' or 'quit'.
- Example usage: Query about UAB-related topics or general conversation.

## Requirements

```bash
Python >= 3.8
torch
numpy
random
google-generativeai  # For Gemini API

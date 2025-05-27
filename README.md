# Chaingram Visualization Tool

This Python project analyzes and visualizes relationships between n-grams within a collection of texts. It constructs a graph showing how phrases (n-grams) overlap and embed within longer ones, offering insights into language structure and semantic chaining.

## 🔍 Features

- Tokenizes input texts and identifies occurrences of given n-grams
- Detects overlapping sub-phrases and their frequency context
- Builds a directed graph (nodes = n-grams, edges = subgram-to-supergram)
- Reduces the graph using transitive reduction
- Visualizes the graph using PyVis (HTML interactive graph)
- Allows filtering by root phrases and pruning least important nodes via PageRank

## 📦 Dependencies

Install the required libraries with:

```bash
pip install nltk numpy pandas scipy scikit-learn networkx pyvis tqdm matplotlib
import nltk
nltk.download('punkt')

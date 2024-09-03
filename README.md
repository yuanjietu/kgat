# KGAT for Movie Recommendation

## Project Overview

This project implements a Knowledge Graph Attention Network (KGAT) for movie recommendations using the MovieLens dataset. The project involves building a knowledge graph from the dataset, training the KGAT model, and visualizing the knowledge graph.

## Dataset Information

### MovieLens Dataset

The MovieLens dataset is a widely used benchmark dataset in the recommendation systems community. The dataset used in this project includes information about users, movies, ratings, and additional metadata.

- MovieLens 100k: Contains 100,000 ratings from 943 users on 1,682 movies.
- MovieLens 1M: Contains 1 million ratings from 6,000 users on 4,000 movies.

### Knowledge Graph CSV Files

- knowledge_graph_movies_100k.csv: Knowledge graph built from the MovieLens 100k dataset.
- knowledge_graph_movies_1m.csv: Knowledge graph built from the MovieLens 1M dataset.

## Installation

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook

### Install Dependencies

```bash
pip install -r requirements.txt

```

## Code Explanation

### 1. kg_building.ipynb

This notebook is responsible for building the knowledge graph from the MovieLens dataset. It extracts relationships such as user-movie interactions, movie-genre associations, and more. The output is saved as CSV files (knowledge_graph_movies_100k.csv and knowledge_graph_movies_1m.csv).

### 2. kgat_attention_smoothndcg_embedding.ipynb

This notebook implements the KGAT model. It includes the following steps:

- **Embedding Initialization:** Initializes the embeddings for entities and relations.
- **Multi-Head Attention:** Implements the attention mechanism used in KGAT.
- **Training and Evaluation:** Trains the model using the training data and evaluates it on the test set.

### 3. visualize_kg.ipynb

This notebook provides visualization of the knowledge graph, helping to understand the structure and relationships within the data.

## How to Run

- Build the Knowledge Graph: Run the kg_building.ipynb notebook to generate the knowledge graph CSV files.
- Train the KGAT Model: Run the kgat_attention_smoothndcg_embedding.ipynb notebook to train the KGAT model on the knowledge graph data.
- Visualize the Knowledge Graph: Run the visualize_kg.ipynb notebook to visualize the knowledge graph.

## Results

The KGAT model is evaluated using metrics such as Mean HR and Mean NDCG. The results are displayed at the end of the kgat_attention_smoothndcg_embedding.ipynb notebook.

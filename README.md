# Portfolio

Here you can find links to my most relevant projects. Click on a project's name to open it.

## Table of Contents

1. [Machine Learning Research & LLMs](#i-machine-learning-research--llms)
2. [Deep Learning & Machine Learning](#ii-deep-learning--machine-learning)
3. [Distributed Systems & Data Engineering](#iii-distributed-systems--data-engineering)
4. [Backend & Software Engineering](#iv-backend--software-engineering)

## I. Machine Learning Research & LLMs

**[CARF: Cardinality-Aware Reranking for Knowledge Graph Completion](https://github.com/Cosminius/kgc-reranker-cardinality)** (paper submitted to ICAAR 2026)

Code for my paper with Gheorghe Cosmin Silaghi. A BERT cross-encoder reranks the top 50 answers of a SimKGC bi-encoder, and the two scores are combined with one weight per cardinality bin. It improves MRR on all three benchmarks, for example from 67.1 to 73.9 on WN18RR.

**Oscar RAG: Graph RAG vs. Text RAG** (link not public yet)

A local app that answers questions about the 2026 Oscars in two ways: a local LLM writes SPARQL queries over a knowledge graph, or the app searches text with Weaviate and a reranker. It refuses to answer when it finds nothing relevant.

**[Sneaker Reseller Knowledge Graph](https://github.com/Cosminius/SNEAKER-Reseller-KG)**

A GraphDB knowledge graph with about 100,000 sneakers, orders, regions and brands, built from legacy data, an ADOxx model and OWL and SPARQL reasoning rules. You can query it in plain English.

## II. Deep Learning & Machine Learning

**[AI-Generated Image Detector](https://github.com/Cosminius/AI_images_Detector)**

A Flask app that tells real photos from AI-generated ones. A first model decides if the image shows a person or an object, then a model trained for that type gives the answer.

From my work through *Hands-On Machine Learning with Scikit-Learn and PyTorch* (Aurélien Géron), with the end-of-chapter exercises:

**[Time Series Forecasting with RNNs and CNNs](https://github.com/Cosminius/Processing_Seqeunces_with_RNNs_and_CNNs)**

Predicts daily bus and train ridership in Chicago, from naive and SARIMA baselines to LSTM, GRU and WaveNet-style models. Also includes sketch recognition and a "yes"/"no" classifier on my own audio recordings.

**[NLP with RNNs and Attention](https://github.com/Cosminius/NLP_with_RNN_and_Attention)**

Text generation, sentiment analysis, English to Spanish translation with attention, and a date converter built from scratch.

**[Convolutional Neural Networks](https://github.com/Cosminius/ConvolutionalNeuralNets)**

Computer vision with CNNs in PyTorch and torchvision.

**[End-to-End ML Flow](https://github.com/Cosminius/End-to-End-ML-Flow)**

The full scikit-learn workflow on housing and used car prices: data exploration, feature engineering, Random Forest and hyperparameter search.

Other chapters: [Neural Networks](https://github.com/Cosminius/NeuralNets-and-DeepLearning) · [Classification](https://github.com/Cosminius/ml-classification-fundamentals) · [Training Models](https://github.com/Cosminius/ml-training-models) · [Decision Trees](https://github.com/Cosminius/ml_decision-trees) · [Ensemble Methods](https://github.com/Cosminius/ml-ensemble-methods) · [Dimensionality Reduction](https://github.com/Cosminius/Dimensionality-Reduction) · [Unsupervised Learning](https://github.com/Cosminius/Unsupervised_learning)

## III. Distributed Systems & Data Engineering

**[Distributed Monte Carlo Value-at-Risk](https://github.com/Cosminius/distributed-montecarlo-var)**

Computes the risk of a stock portfolio with 480 million Monte Carlo scenarios, split across four funcX (Globus Compute) nodes running in Docker. Reaches a 2.3x speed-up on 3 nodes.

**[RDF Bridge](https://github.com/Cosminius/RDF-Bridge)**

Turns RDF graphs stored in RDF4J into JSON and exposes them through a GraphQL API, with a Flask backend and a JavaScript frontend.

## IV. Backend & Software Engineering

**[Restaurant Ordering App](https://github.com/Cosminius/Proiect_Comenzi_Restaurant)** and **[Restaurant Mobile App](https://github.com/Cosminius/MobileAppRestaurant)**

A restaurant ordering web app in ASP.NET and its mobile version in .NET MAUI.

## Contact

[LinkedIn](https://linkedin.com/in/rosculet-cosmin)

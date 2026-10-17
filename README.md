# Portfolio

I'm a master's student at Babeș-Bolyai University in Cluj-Napoca, working on LLMs, retrieval-augmented generation and knowledge graphs. Below are my most relevant projects; click on a project's name to open it.

## Table of Contents

1. [Machine Learning Research & LLMs](#i-machine-learning-research--llms)
2. [Deep Learning & Machine Learning](#ii-deep-learning--machine-learning)
3. [Distributed Systems & Data Engineering](#iii-distributed-systems--data-engineering)
4. [Backend & Software Engineering](#iv-backend--software-engineering)

## I. Machine Learning Research & LLMs

**[CARF: Cardinality-Aware Reranking for Knowledge Graph Completion](https://github.com/Cosminius/kgc-reranker-cardinality)** (paper submitted to ICAAR 2026)

Implements my paper with Gheorghe Cosmin Silaghi. Reranks the top 50 answers of a SimKGC bi-encoder with a BERT cross-encoder, then combines the two scores with one weight per cardinality bin. Improves MRR on all three benchmarks, for example from 67.1 to 73.9 on WN18RR.

**[Oscar RAG: Graph RAG vs. Text RAG](https://github.com/grnln/OscarRAG)**

Compares structured and unstructured retrieval on the same domain, the 2026 Academy Awards. Splits the data on purpose: the knowledge graph holds only the results and the text only the Academy's history, so every question shows which kind of retrieval suits it. Runs both pipelines on one local LLM (Qwen 2.5 Coder 7B via Ollama), so nothing leaves the machine.

- **Graph RAG:** Turns each question into a SPARQL query over an RDF knowledge graph in GraphDB (LangChain), guided by few-shot examples, and shows the query so you can check the answer.
- **Text RAG:** Searches the text with MiniLM embeddings in Weaviate, reranks the results with a cross-encoder and cites its sources. Refuses to answer when nothing relevant is found.

## II. Deep Learning & Machine Learning

**[AI-Generated Image Detector](https://github.com/Cosminius/AI_images_Detector)**

Tells real photos from AI-generated ones in a Flask app. First decides whether the image shows a person or an object, then passes it to a model trained for that type.

From my work through *Hands-On Machine Learning with Scikit-Learn and PyTorch* (Aurélien Géron), with the end-of-chapter exercises:

**[Transformers for NLP and Chatbots](https://github.com/Cosminius/Transformers-for-NLP-and-Chatbots)**

Covers the main Transformer families in PyTorch and Hugging Face:

- **Transformer from scratch:** Builds attention and the full encoder-decoder by hand, then trains it for English to Spanish translation.
- **BERT from scratch:** Pretrains an encoder-only model with masked language modeling on WikiText-2.
- **Fine-tuning:** Fine-tunes DistilBERT for IMDb sentiment analysis and GPT-2 on Shakespeare.
- **Alignment:** Aligns GPT-2 with TRL, first with SFT on Alpaca, then with DPO on Anthropic HH-RLHF.
- **Movie-expert chatbot with RAG:** Retrieves similar plots from 35,000 Wikipedia movies with SBERT and lets Qwen recommend films based on them.

**[Time Series Forecasting with RNNs and CNNs](https://github.com/Cosminius/Processing_Seqeunces_with_RNNs_and_CNNs)**

Predicts daily bus and train ridership in Chicago, from naive and SARIMA baselines to LSTM, GRU and WaveNet-style models. Also includes sketch recognition and a "yes"/"no" classifier on my own audio recordings.

Other chapters: [NLP with RNNs and Attention](https://github.com/Cosminius/NLP_with_RNN_and_Attention) · [Convolutional Neural Networks](https://github.com/Cosminius/ConvolutionalNeuralNets) · [End-to-End ML Flow](https://github.com/Cosminius/End-to-End-ML-Flow) · [Neural Networks](https://github.com/Cosminius/NeuralNets-and-DeepLearning) · [Classification](https://github.com/Cosminius/ml-classification-fundamentals) · [Training Models](https://github.com/Cosminius/ml-training-models) · [Decision Trees](https://github.com/Cosminius/ml_decision-trees) · [Ensemble Methods](https://github.com/Cosminius/ml-ensemble-methods) · [Dimensionality Reduction](https://github.com/Cosminius/Dimensionality-Reduction) · [Unsupervised Learning](https://github.com/Cosminius/Unsupervised_learning)

## III. Distributed Systems & Data Engineering

**[Distributed Monte Carlo Value-at-Risk](https://github.com/Cosminius/distributed-montecarlo-var)**

Computes the risk of a stock portfolio with 480 million Monte Carlo scenarios, split across four funcX (Globus Compute) nodes running in Docker. Reaches a 2.3x speed-up on 3 nodes.

**[RDF Bridge](https://github.com/Cosminius/RDF-Bridge)**

Turns RDF graphs stored in RDF4J into JSON and exposes them through a GraphQL API, with a Flask backend and a JavaScript frontend.

## IV. Backend & Software Engineering

**[Restaurant Ordering App](https://github.com/Cosminius/Proiect_Comenzi_Restaurant)** and **[Restaurant Mobile App](https://github.com/Cosminius/MobileAppRestaurant)**

Takes restaurant orders on the web (ASP.NET) and on mobile (.NET MAUI).

## Contact

[GitHub](https://github.com/Cosminius) · [LinkedIn](https://linkedin.com/in/rosculet-cosmin)

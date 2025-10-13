🧠 TextMorph: Advanced Text Summarization and Model Comparison
Project Overview

TextMorph Milestone 2 focuses on advanced text summarization using both abstractive and extractive techniques.
It extends the first milestone by integrating multiple transformer-based models, adding interactive Google Colab UIs, and visualizing evaluation metrics to identify which model performs best.

The project demonstrates:

Generation of concise, accurate summaries from diverse text domains

Metric-based comparison of multiple models

Visualization of performance to support model selection

Models Used

TinyLlama (Abstractive)
Version: TinyLlama/TinyLlama-1.1B-Chat-v1.0
Lightweight chat model offering fast summarization while preserving meaning.

Phi 2 (Abstractive)
Version: microsoft/phi-2
Compact reasoning-based model providing efficient and coherent summaries.

BART-Large-CNN (Abstractive)
Version: facebook/bart-large-cnn
Classic transformer fine-tuned for high-quality summarization.

Gemma 2B-IT (Abstractive)
Version: google/gemma-2b-it
Google’s instruction-tuned model delivering fluent, human-like summaries.

TextRank (Extractive)
Algorithm: Graph-based ranking using PageRank on sentence embeddings (all-MiniLM-L6-v2).

Why These Models Were Used

TinyLlama: Fast and efficient summarization for limited resources.

Phi 2: Reasoning-based outputs with strong semantic accuracy.

BART: Reliable baseline for abstractive summarization.

Gemma: High-quality summaries through instruction tuning.

TextRank: Non-neural extractive benchmark for comparison.

Stepwise Workflow

Install Dependencies – Set up required libraries like transformers, torch, datasets, and ipywidgets.

Import Modules – Load APIs, metrics, and visualization tools.

Hugging Face Setup – Create account, accept Gemma license, add token as HF_TOKEN in Colab.

Model Initialization – Load TinyLlama, Phi, BART, Gemma, and TextRank with GPU optimization.

Data Preparation – Use 10 sample texts from various domains for testing.

Summarization – Generate summaries from all models on the same inputs.

TextRank (Extractive) – Apply embeddings and PageRank for extractive summaries.

Evaluation Metrics – Compute ROUGE, semantic similarity, and readability scores.

Interactive UIs – Use Colab widgets to compare or select models for summarization.

Visualization – Plot graphs comparing model performance across metrics.

Execution and Runtime Details

Runtime: Designed for Google Colab GPU environment.

Precision: Uses torch.bfloat16 for efficient memory usage.

Device Mapping: Automatically assigns models to CPU/GPU.

Error Handling: Managed token and memory issues with safe exception blocks.

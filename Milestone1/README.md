# TextMorph: Text Summarization and Paraphrasing Comparison

## Project Overview
**TextMorph** is an NLP project aimed at **comparing the performance of three popular transformer models—T5, BART, and PEGASUS—for both text summarization and paraphrasing**. Using publicly available texts, the project evaluates each model’s outputs based on:

- How well it preserves the original content  
- The length and conciseness of summaries  
- The quality and diversity of paraphrased outputs  

This analysis helps identify which model is best suited for different **language generation tasks**.

---

## Models Used

- **T5 (Text-to-Text Transfer Transformer)**: A versatile model capable of handling both summarization and paraphrasing tasks.  
- **BART (Bidirectional and Auto-Regressive Transformer)**: Designed for sequence generation, effective for summarization and paraphrasing.  
- **PEGASUS (Pre-training with Extracted Gap-sentences for Abstractive Summarization)**: Specialized for abstractive summarization tasks.  
- **SentenceTransformer (all-MiniLM-L6-v2)**: Used to compute sentence embeddings for measuring similarity between generated text and original input.

---

## Stepwise Workflow

1. **Install Dependencies**: Python libraries for transformer models, evaluation metrics, embeddings, and plotting.  
2. **Import Modules**: Hugging Face pipelines, sentence transformers, cosine similarity, and text processing utilities.  
3. **Load Pre-trained Models**: Summarization and paraphrasing models loaded on CPU by default.  
4. **Data Preparation**: Fetch and preprocess input texts by cleaning and trimming for efficient processing.  
5. **Summarization**: Generate summaries using each model, applying chunking to handle large inputs.  
6. **Paraphrasing**: Perform paraphrasing on summaries with each model, managing exceptions for stability.  
7. **Analysis**: Compute cosine similarities between original and generated text embeddings.  
8. **Visualization**: Compare output length distributions and similarity scores through charts.  
9. **Sample Outputs**: Display examples for manual and qualitative assessment.

---

## Execution and Runtime Details

- **CPU Limitation**: Initial execution on CPU was slow due to large model sizes and text volume.  
- **GPU Acceleration**: Switching to GPU (e.g., on Google Colab) significantly improved inference speed.  
- **Memory Management**: Chunked input texts and dynamic device allocation prevented memory overflow.  
- **Error Handling**: Implemented exception handling to address PEGASUS warnings and ensure smooth operation.

---

## Challenges Faced and Solutions

- **Large Model Sizes**: Split input data into smaller chunks to avoid memory issues.  
- **Slow CPU Processing**: Transitioned to GPU for faster computation.  
- **Model Warnings/Errors**: Added exception handling for PEGASUS to improve stability.  
- **Device Compatibility**: Adapted code to detect CPU/GPU automatically for portability.

---

## Conclusion on Model Suitability

- **BART**: Best for **summarization** where accuracy and content preservation are priorities. Produces summaries that closely match the original text.  
- **T5**: Ideal for **paraphrasing** where similarity to the original is important but variation is desired.  
- **PEGASUS**: Performs well for **summarization**, but paraphrased outputs are more abstract, suitable for creative or novel paraphrasing needs.

**Summary Recommendations**:

| Task              | Recommended Model | Reason |
|------------------|-----------------|--------|
| Summarization     | BART            | High similarity and content preservation |
| Paraphrasing      | T5              | Balanced similarity and diversity |
| Creative Paraphrasing | PEGASUS     | Produces abstract or novel outputs |

These conclusions are supported by similarity metrics and output length analyses visualized in the project charts.

---

## Repository Purpose

This repository is intended to **showcase milestones, projects, and achievements** from the TextMorph project. It highlights **technical skills, model evaluation, and implementation experience**, serving as a record of **growth and learning in NLP and AI-focused text generation tasks**.


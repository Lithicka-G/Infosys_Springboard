# TextMorph: Advanced Text Summarization and Model Comparison

## Project Overview
**TextMorph Milestone 2** focuses on **advanced text summarization** using both *abstractive* and *extractive* techniques.  
It extends the first milestone by integrating multiple transformer-based models, adding **interactive Google Colab UIs**, and visualizing **evaluation metrics** to identify which model performs best.

The project demonstrates:
- Generation of concise, accurate summaries from diverse text domains  
- Metric-based comparison of multiple models  
- Visualization of performance to support model selection

---

### What Are Abstractive and Extractive Models?
- **Abstractive Models:** Generate new text to summarize content meaningfully, often rewording and compressing information like a human would.
- **Extractive Models:** Select and combine the most important sentences from the source text without rewriting them.  

---

## Models Used

### Abstractive Models:

#### 1. TinyLlama  
- **Version:** `TinyLlama/TinyLlama-1.1B-Chat-v1.0`  
- Lightweight chat model offering fast summarization while preserving meaning.

#### 2. Phi 2  
- **Version:** `microsoft/phi-2`  
- Compact reasoning-based model providing efficient and coherent summaries.

#### 3. BART-Large-CNN  
- **Version:** `facebook/bart-large-cnn`  
- Classic transformer fine-tuned for high-quality summarization.

#### 4. Gemma 2B-IT  
- **Version:** `google/gemma-2b-it`  
- Google’s instruction-tuned model delivering fluent, human-like summaries.

### Extractive Models:

#### 1. TextRank  
- **Algorithm:** Graph-based ranking using PageRank on sentence embeddings (`all-MiniLM-L6-v2`).  
- Produces summaries by selecting key sentences from the input text.

---

## Why These Models Were Used
- **TinyLlama:** Fast and efficient summarization for limited resources.  
- **Phi 2:** Reasoning-based outputs with strong semantic accuracy.  
- **BART:** Reliable baseline for abstractive summarization.  
- **Gemma:** High-quality summaries through instruction tuning.  
- **TextRank:** Non-neural extractive benchmark for comparison.  

---

## 10 Sample Texts From Different Domains:
1. Nature
2. Climate Change
3. Artificial Intelligence
4. Stock Market
5. Pollution
6. Life in Japan
7. Afterlife
8. Pollution
9. Cybersecurity
10. Anime

## Stepwise Workflow

1. **Install Dependencies** – Set up required libraries like `transformers`, `torch`, `datasets`, and `ipywidgets`.  
2. **Import Modules** – Load APIs, metrics, and visualization tools.  
3. **Hugging Face Setup** – Create account, accept Gemma license, add token as `HF_TOKEN` in Colab.  
4. **Model Initialization** – Load TinyLlama, Phi, BART, Gemma, and TextRank with GPU optimization.  
5. **Data Preparation** – Use 10 sample texts from various domains for testing.  
6. **Summarization** – Generate summaries from all models on the same inputs.  
7. **TextRank (Extractive)** – Apply embeddings and PageRank for extractive summaries.  
8. **Evaluation Metrics** – Compute ROUGE, semantic similarity, and readability scores.  
9. **Interactive UIs** – Use Colab widgets to compare or select models for summarization.  
10. **Visualization** – Plot graphs comparing model performance across metrics.  

---

## Execution and Runtime Details
- **Runtime:** Designed for **Google Colab GPU** environment.  
- **Precision:** Uses `torch.bfloat16` for efficient memory usage.  
- **Device Mapping:** Automatically assigns models to CPU/GPU.  
- **Error Handling:** Managed token and memory issues with safe exception blocks.  

---

## Challenges Faced and Solutions

| Challenge | Solution |
|------------|-----------|
| Large model memory usage | Used `torch.bfloat16` and `device_map="auto"`. |
| Gemma authorization errors | Added Hugging Face token and license acceptance. |
| Slow inference on CPU | Switched to GPU runtime in Colab. |
| Inconsistent summary lengths | Applied uniform decoding and length limits. |

---

## Results and Analysis

| Model | ROUGE-L (↑) | Semantic Similarity (↑) | Readability (↑) | Summary Length (↓) |
|--------|--------------|--------------------------|------------------|--------------------|
| **Gemma 2B-IT** | Highest | High | Balanced | Medium |
| **BART-Large-CNN** | High | Moderate | Good | Medium |
| **Phi 2** | Medium | High | Excellent | Short |
| **TinyLlama** | Moderate | Moderate | High | Very Short |
| **TextRank** | Lowest | Low | Good | Short |

- **Gemma 2B-IT** produced the most coherent and human-like summaries.  
- **BART** remained a consistent baseline.  
- **Phi 2** achieved good performance with low resource use.  
- **TinyLlama** offered fast, concise summaries.  
- **TextRank** provided a transparent extractive comparison.



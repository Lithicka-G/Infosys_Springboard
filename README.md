# Infosys_Springboard / Milestone1

**Project Description**
This repository contains Milestone 1 for Text Summarization & Paraphrasing. The goal is to compare pretrained transformer models for summarization (T5, BART, Pegasus-XSum) and paraphrasing (T5, Pegasus, BART variants). This deliverable includes an analysis notebook, code, and visual comparisons to help pick models for real projects.

## What I did:

I created a Colab notebook that:

* Loads two `.txt` files as inputs (you can replace with your own).
* Produces summaries with T5, BART, and Pegasus-XSum.
* Produces paraphrases using fine-tuned paraphrase variants of T5/Pegasus/BART.
* Computes ROUGE scores for summarization and BLEU scores for paraphrases (length, lexical overlap).
* Generates plots comparing models so you can easily see which is better for short/long text.

## Repo structure:

```
Infosys_Springboard/
└── Milestone1/
    ├── README.md            # (this file)
    ├── code/
    │   └── Milestone1_notebook.ipynb   # Colab-ready notebook (final .ipynb)
    ├── data/
    │   ├── input1.txt       # sample input text 1
    │   └── input2.txt       # sample input text 2
```

## Notes on models:

* **T5 (t5-base)** — versatile; you need to provide `task: summarization:` style prompts in some code. Good balance of speed/quality.
* **BART (facebook/bart-large-cnn)** — strong summarizer on news-like text. I suggest `bart-large-cnn` for better summaries than `bart-base`.
* **Pegasus (google/pegasus-xsum)** — trained specifically for extreme summarization; great for short, punchy summaries.
* **Paraphrase models** — many fine-tuned checkpoints exist. I provide example model IDs and code where you can swap in any HF model.

# Financial Sentiment Analyzer using BERT

## Project Overview
This Natural Language Processing (NLP) project leverages a fine-tuned Large Language Model (LLM) to analyze and classify the sentiment of financial news headlines. By automating the extraction of market sentiment (Positive, Negative, Neutral), this tool can assist financial analysts and trading algorithms in processing massive streams of news data in real-time.

## Tools & Technologies
* **Language:** Python
* **Machine Learning Framework:** PyTorch
* **NLP & LLMs:** Hugging Face `transformers`, `datasets`
* **Model:** Pre-trained `bert-base-uncased`
* **Data Manipulation:** Pandas

## Methodology
1. **Data Acquisition:** Utilized the Financial PhraseBank dataset, consisting of thousands of financial sentences labeled by industry experts.
2. **Preprocessing & Tokenization:** Employed the BERT Tokenizer to convert text data into machine-readable formats, managing padding and truncation for uniform sequence lengths. Set up custom PyTorch Datasets for optimized data loading.
3. **Fine-Tuning:** Fine-tuned the `bert-base-uncased` transformer model using Google Colab (T4 GPU). 
4. **Evaluation:** Achieved a highly accurate baseline classification score after just two epochs, demonstrating the model's strong contextual understanding of financial terminology.

## Key Capabilities
* **Contextual Understanding:** Goes beyond simple keyword matching (e.g., understanding that "drop in profits" is negative, but "drop in expenses" is positive).
* **Scalable Pipeline:** The prediction engine is built to rapidly ingest and classify new, unseen text data on demand.

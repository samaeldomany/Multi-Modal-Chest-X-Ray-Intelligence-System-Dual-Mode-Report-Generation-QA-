# Multi-Modal-Chest-X-Ray-Intelligence-System-Dual-Mode-Report-Generation-QA-

## Overview
This repository contains a dual-mode medical AI system that integrates vision-language retrieval (ColPali) and instruction-tuned generation (MedGemma) to analyze Chest X-Rays. 

### Features
1. **Mode 1: Report Generation:** Upload an X-ray, retrieve visually similar historical cases via Qdrant, and generate a structured medical report using MedGemma.
2. **Mode 2: Clinical QA (RAG):** Ask text-based clinical questions, retrieve relevant historical context, and generate grounded answers.

### Model Architecture
* **Retriever:** `vidore/colpali-v1.3`
* **Generator:** `google/gemma-2b-it` (4-bit Quantized)


## How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Add your Hugging Face Token as an environment variable: `export HF_TOKEN="your_token_here"`
3. Launch the UI: `python app.py`

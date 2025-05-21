# Legal Document Analysis with LLaMA 3

This project leverages Meta's LLaMA 3 model to classify legal documents using a fine-tuned language model approach. It is designed to work with preprocessed document metadata and demonstrates the end-to-end pipeline for classifying legal documents into predefined categories.

## Project Structure

- `Llama_3_2_Calssify_docs.ipynb` – Main notebook that loads the model, processes input metadata, and performs classification.
- `Convert_pdf_to_text_and_clean.ipynb` – Utility for converting PDFs to cleaned text.
- `Post_processing.ipynb` – Handles post-processing of classification results.
- `MD_splits.zip` – Contains splits used for training/testing.
- `instruction.txt` – Prompt engineeried instructions.
- `LICENSE` – License information for the project.

## Setup Instructions

1. **Install dependencies** (from the main notebook):

```bash
pip install --upgrade pip
pip install datasets transformers bitsandbytes>=0.39.0 accelerate>=0.20.0 optimum>=1.20.0 gdown packaging ninja flash-attn
````

2. **Download required files**:
   The notebook uses `gdown` to fetch a folder of preprocessed data from Google Drive. Ensure you have access to the linked dataset.

3. **Run the main notebook**:
   Open `Llama_3_2_Calssify_docs.ipynb` in Jupyter or Colab and execute the cells sequentially.

## Usage

This project is intended for legal document analysis tasks, particularly:

* Document type classification
* AI-assisted legal data triage
* Evaluation of LLaMA 3 model performance on domain-specific content

## Requirements

* Python 3.8+
* GPU (recommended for model inference)
* Jupyter Notebook

## License

This repository is licensed under the terms of the LICENSE file.

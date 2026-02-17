# Synthetic Data Forge

AI-powered synthetic data generation tool using Qwen-2.5-7B-Instruct.

## Description

Synthetic Data Forge is a tool designed to generate high-quality synthetic data for various business niches. It leverages the power of the **Qwen/Qwen2.5-7B-Instruct** Large Language Model (LLM) to create realistic datasets. The tool features a user-friendly Gradio interface, allowing users to specify a business niche and the number of rows to generate. The generated data can be viewed directly in the browser and downloaded as a CSV file.

## Features

-   **AI-Powered Generation:** Uses Qwen-2.5-7B-Instruct for intelligent and context-aware data generation.
-   **Gradio Interface:** Simple web-based UI for easy interaction.
-   **Customizable:** Generate data for any business niche (e.g., Hospital, E-commerce, Finance) by providing a prompt.
-   **Realistic Data:** Integrates `Faker` library for realistic names, addresses, and dates, combined with LLM-generated logic for consistency.
-   **Export:** Download generated datasets as CSV files.
-   **GPU Accelerated:** Optimized for running on GPU (CUDA) for faster generation.

## Prerequisites

To run this notebook, you need the following Python libraries:

-   `torch`
-   `transformers`
-   `accelerate`
-   `bitsandbytes` (for 4-bit quantization)
-   `gradio`
-   `faker`
-   `pandas`
-   `huggingface_hub`

You can install them using pip:

```bash
pip install torch transformers accelerate bitsandbytes gradio faker pandas huggingface_hub
```

## Usage

1.  **Open the Notebook:** Open `DATAGEN.ipynb` in Google Colab or a Jupyter environment with GPU support.
2.  **Install Dependencies:** Run the first few cells to install the necessary libraries.
3.  **Hugging Face Login:** You will need a Hugging Face token to access the model. authentiate using `notebook_login()` or set the `HF_TOKEN` secret in Colab.
4.  **Run the Generator:** Execute the cells to load the model and define the generation functions.
5.  **Launch Interface:** Run the final cell to launch the Gradio interface.
6.  **Generate Data:**
    -   Enter a business niche prompt (e.g., "Retail store inventory").
    -   Specify the number of rows.
    -   Click "Submit".
    -   Download the generated CSV.

## Files

-   `DATAGEN.ipynb`: The main Jupyter Notebook containing the code.
-   `README.md`: This file.

## License

[MIT](https://choosealicense.com/licenses/mit/)

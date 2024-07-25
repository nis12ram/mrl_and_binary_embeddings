# Jupyter Notebooks for Movie Embedding and Retrieval

This subfolder contains Jupyter notebooks that demonstrate various methods for embedding movie data and performing retrieval tasks. Below are the key features and points covered in this subfolder.

## Key Features

1. **Embedding Model**
    - **Model Used:** [nomic-embed-text-v1.5-GGUF](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5-GGUF)
    - This model is used to convert movie names, types, and descriptions into embedding vectors.

2. **Dataset**
    - **Dataset Used:** [IMDB Movies Dataset Based on Genre](https://www.kaggle.com/datasets/rajugc/imdb-movies-dataset-based-on-genre)
    - This dataset is used to train and test the embedding and retrieval systems.

## Jupyter Notebooks

1. **in_Memory.ipynb**
    - This notebook demonstrates how to use FAISS to store and retrieve binary vectors in-memory. The vectors are not stored permanently.

2. **persistent_memory.ipynb**
    - This notebook demonstrates how to use FAISS for storing and retrieving binary vectors but in a persistant .

3. **scratch_ar_mrl_bin.ipynb**
    - This notebook details the process of storing and retrieving binary vectors without using FAISS.

## How to Use

1. **Download the Embedding Model**
    - Download the embedding model from [Hugging Face](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5-GGUF) and place it in the appropriate directory.

2. **Download the Dataset**
    - Download the dataset from [Kaggle](https://www.kaggle.com/datasets/rajugc/imdb-movies-dataset-based-on-genre) and place it in the data directory.

3. **Run the Notebooks**
    - Open each Jupyter notebook and follow the instructions to see how to implement embedding and retrieval using different methods.

## Requirements

- Python 3.5+
- pandas
- faiss-cpu
- llama-cpp-python[server]
- numpy
- [nomic-embed-text-v1.5-GGUF](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5-GGUF)
- [IMDB Movies Dataset](https://www.kaggle.com/datasets/rajugc/imdb-movies-dataset-based-on-genre)


![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Embeddings


## Introduction

A digital bank receives thousands of support messages a day, and most of them have been asked, and answered, many times before. In this lab you build the tool that finds them: a semantic search that takes a new customer message and returns the most similar past messages and their category. You compare sentences with an embedding model, index 10,000 real customer messages, write the search function, build a TF-IDF search to compare with, measure both on 3,080 new messages, and check whether the embeddings can discover the categories on their own. In the extra task, you teach the tool to say *I'm not sure*.

The lab follows the **Embeddings and Semantic Search** lesson step by step.


## Getting Started

Open the `main.ipynb` file in the `your-code` directory. Follow the instructions, add your code, and answer the questions in the markdown cells. Each challenge ends with a checkpoint that tells you what you should see. The data is in the `data` folder: `banking_train.csv` has the past messages and `banking_test.csv` the new ones, both with the columns `text` and `category`.

The lab needs the `sentence-transformers` library (`pip install sentence-transformers`). The first run downloads the `all-MiniLM-L6-v2` model, about 90 MB, so you need an internet connection. Everything else runs on your own computer, with no account and no API key.

## Deliverables

- `main.ipynb` with your code, its outputs, and your answers.

## Submission

Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.

## Resources

- [Sentence Transformers examples: Semantic search](https://github.com/huggingface/sentence-transformers/tree/main/examples/sentence_transformer/applications/semantic-search)
- [Sentence Transformers examples: Clustering](https://github.com/huggingface/sentence-transformers/tree/main/examples/sentence_transformer/applications/clustering)
- [scikit-learn user guide: Clustering performance evaluation](https://scikit-learn.org/stable/modules/clustering.html#clustering-performance-evaluation)

## Data

The Banking77 dataset was created by PolyAI and published in [Efficient Intent Detection with Dual Sentence Encoders](https://arxiv.org/abs/2003.04807) (Casanueva et al., 2020). It is available at [PolyAI-LDN/task-specific-datasets](https://github.com/PolyAI-LDN/task-specific-datasets) under the [Creative Commons Attribution 4.0 licence](https://creativecommons.org/licenses/by/4.0/). The files in `data` are the original `train.csv` and `test.csv`, renamed, with no other change.

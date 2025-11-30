This project is a from-scratch implementation of a Transformer-based language model, closely following the architecture of GPT-2 and the seminal paper, "Attention Is All You Need".

This is the pretrain model, So it is trained on the TinyStories dataset to perform the task of Next Word Prediction (NWP), learning to generate coherent, story-like text.

# Features
Decoder-Only Architecture: Implements a GPT-2 style decoder stack.\
Multi-Head Self-Attention: The core mechanism allowing the model to weigh the importance of different words in the input sequence.\
Positional Encoding: Injects information about the position of tokens in the sequence.\
Text Generation: Uses Top-k sampling with temperature scaling for diverse and controlled text generation.

Paramters:
No. of heads - 12
No. of layer - 12
Embd. dim - 768
Context length - 1024

# Evaluation
The model was evaluated on its Next Word Prediction capabilities on a held-out test set from the TinyStories dataset. The performance was measured using several standard NLP metrics.

Metric	Score\
BLEU:	0.834\
ROUGE-L:	0.915\
BERTScore (F1):	0.970\
Perplexity: 279.810

# Tech Stack Used
Python 3.10\
PyTorch\
Hugging Face Transformers\
NumPy


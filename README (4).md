# NLP Homework 4  
# Sharath Chandra Seriyala (700776646)

## Overview

This repository showcases implementations of fundamental Natural Language Processing (NLP) models, including:  
- Character-Level RNN  
- Mini Transformer Encoder  
- Scaled Dot-Product Attention  

---

## Q1: Character-Level RNN

### Model Architecture

Embedding → RNN → Fully Connected Layer → Softmax  

### Training Performance

The model’s loss steadily decreased from approximately 0.65 to around 0.11, indicating successful learning over epochs.

### Text Generation Behavior

- Temperature 0.7: Produces more consistent and repetitive text  
- Temperature 1.0: Generates balanced and readable output  
- Temperature 1.2: Produces more diverse but less stable text  

### Observations

- Lower temperature values result in more predictable and structured text  
- Higher temperature values increase creativity but introduce noise  

---

## Q2: Mini Transformer Encoder

### Key Components

- Tokenization  
- Embedding Layer  
- Positional Encoding  
- Self-Attention Mechanism  
- Multi-Head Attention  
- Feedforward Network with Layer Normalization  

### Output

- Produces contextualized word embeddings  
- Attention visualizations illustrate relationships between words in a sequence  

---

## Q3: Scaled Dot-Product Attention

### Formula

Attention(Q, K, V) = softmax(QKᵀ / √dₖ) V  

### Results

- Raw attention scores are computed using QKᵀ  
- Scaling factor improves numerical stability of softmax  
- Attention weights emphasize the most relevant tokens  

### Key Insight

Applying scaling prevents excessively large values, ensuring stable gradients during training  

---

## Conclusion

- RNNs are effective for capturing sequential patterns  
- Transformers provide improved context understanding  
- Attention mechanisms enable efficient modeling of relationships within text  

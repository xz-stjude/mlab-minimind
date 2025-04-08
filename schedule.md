This educational seminar series guides participants through the complete process of training a small, efficient language model from scratch, based on the MiniMind project. Participants will learn both theoretical foundations and practical implementation skills for building their own LLMs with minimal resources.

---

### Session 1: Introduction to LLMs and the MiniMind Project

- **Introduction to Large Language Models**
  - Evolution of language models and the transformer architecture
  - Current landscape of LLMs and their applications
  - Challenges with large models: cost, resources, and accessibility
- **The MiniMind Project Overview**
  - Project goals: training a 26M parameter model in 2 hours for ~3 RMB
  - Technical architecture and design choices
  - Model variants: Dense vs MoE implementations
- **Development Environment Setup**
  - Installing required libraries and dependencies
  - Setting up GPU environments for training
  - Code structure walkthrough and project organization
- **Hands-on**: Setting up the MiniMind codebase and exploration of model architecture

---

### Session 2: Tokenization and Vocabulary

- **Understanding Tokenization in LLMs**
  - Role of tokenizers in language models
  - Different tokenization approaches and algorithms
  - Vocabulary size considerations and tradeoffs
- **MiniMind Tokenizer Design**
  - Small vocabulary (6,400 tokens) vs larger tokenizers
  - Performance implications of vocabulary size
  - Training data selection for tokenization
- **Implementation Details**
  - Training a tokenizer from scratch using custom data
  - Using pre-existing tokenizers vs building custom ones
- **Hands-on**: Training a small custom tokenizer and implementing tokenization pipeline

---

### Session 3: Dataset Collection and Processing

- **Types of Datasets for LLM Training**
  - Pretraining data: formats, sources, and quality considerations
  - SFT data: instruction-tuning formats and conversation structures
  - RLHF data: preference pairs and quality benchmarks
- **Data Cleaning and Preprocessing**
  - Text extraction, cleaning, and normalization
  - Deduplication and quality filtering strategies
  - Length considerations and chunking approaches
- **Efficient Data Pipelines**
  - Converting raw text to tokenized training data
  - Building efficient data loaders and batching strategies
- **Hands-on**: Preparing and processing datasets for pretraining and fine-tuning

---

### Session 4: Model Architecture Design

- **Deep Dive into Transformer Architecture**
  - Attention mechanisms and multi-head attention
  - Feed-forward networks and activation functions
  - Pre-normalization and layer structures
- **MiniMind Model Variations**
  - Dense models: balancing layers and width
  - Mixture of Experts (MoE): shared experts implementation
  - Parameter scaling strategies for small models
- **Positional Encoding**
  - RoPE (Rotary Position Embedding) implementation
  - Position embedding considerations for small models
- **Hands-on**: Implementing a simple transformer decoder block

---

### Session 5: Pretraining Fundamentals

- **Pretraining Objectives**
  - Next token prediction (causal language modeling)
  - Loss functions and optimization strategies
- **Training Hyperparameters**
  - Learning rates, batch sizes, and sequence lengths
  - Gradient accumulation and mixed precision training
- **Training Infrastructure**
  - Single GPU vs multi-GPU training
  - DDP and DeepSpeed integration
- **Monitoring and Debugging**
  - Loss curves interpretation and optimization
  - Common issues and troubleshooting strategies
- **Hands-on**: Pretraining a tiny model on a small dataset

---

### Session 6: Supervised Fine-Tuning (SFT)

- **Instruction Tuning Fundamentals**
  - Converting a pretrained model to instruction-following
  - Chat formatting and templates
  - SFT dataset preparation and quality considerations
- **Implementation Approaches**
  - Full parameter fine-tuning methodology
  - Hyperparameter considerations for fine-tuning
  - GPU memory optimization techniques
- **Conversation and Response Format**
  - Implementing conversation templates
  - Managing context windows efficiently
- **Hands-on**: Fine-tuning a pretrained model for instruction following

---

### Session 7: Parameter-Efficient Fine-Tuning

- **Introduction to PEFT Methods**
  - Overview of parameter-efficient fine-tuning approaches
  - Understanding adapter-based methods
- **Low-Rank Adaptation (LoRA)**
  - Mathematical foundations of LoRA
  - Implementation from scratch without external libraries
  - Rank selection and hyperparameter tuning
- **Domain Adaptation**
  - Specializing models for specific domains (medical, code, etc.)
  - Balancing domain knowledge with general capabilities
- **Hands-on**: Implementing LoRA fine-tuning for domain specialization

---

### Session 8: Reinforcement Learning from Human Feedback

- **Introduction to RLHF**
  - Aligning models with human preferences
  - RLHF pipeline overview: reward modeling and RL training
- **Direct Preference Optimization (DPO)**
  - Mathematical foundations of DPO
  - Advantages over traditional PPO approaches
  - Preference dataset preparation and quality
- **Implementation Details**
  - Building the DPO training loop from scratch
  - Balancing preference learning with maintaining capabilities
- **Hands-on**: Training a model with DPO on a small preference dataset

---

### Session 9: Knowledge Distillation and Model Optimization

- **Knowledge Distillation Techniques**
  - Teacher-student model framework
  - White-box vs black-box distillation approaches
  - Loss functions for effective knowledge transfer
- **Reasoning Model Distillation**
  - Distilling reasoning capabilities from larger models
  - Training with intermediate thinking steps
  - MiniMind-Reason implementation details
- **Model Optimization Techniques**
  - KV-cache implementation for efficient inference
  - Quantization approaches for small models
- **Hands-on**: Implementing a distillation pipeline for a reasoning model

---

### Session 10: Evaluation, Deployment and Future Directions

- **Model Evaluation**
  - Benchmark testing (C-Eval, CMMLU, etc.)
  - Qualitative evaluation approaches
  - Performance comparison with other small models
- **Serving and Deployment**
  - Building an OpenAI-compatible API server
  - WebUI implementation with streamlit
  - Inference optimization techniques
- **Future Directions**
  - Scaling to larger models
  - Multimodal extensions (MiniMind-V)
  - Research frontiers for small efficient models
- **Final Project Showcase**
  - Participants demonstrate their trained models
  - Q&A and community discussion
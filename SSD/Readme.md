# Fast Machine Unlearning Without Retraining Through Selective Synaptic Dampening - Jack Foster, Stefan Schoepf, Alexandra Brintrup - AAAI 2024

Welcome to my implementation of **Selective Synaptic Dampening (SSD)** — a technique for selective forgetting in neural networks. This repository reproduces the core ideas from the AAAI 2024 paper:

> **Fast Machine Unlearning Without Retraining Through Selective Synaptic Dampening**  
> *Jack Foster et al.*  
> [Paper Link](https://arxiv.org/abs/2308.07707) 

---

## 📌 What is SSD?

**Selective Synaptic Dampening (SSD)** is a lightweight Post Hoc and efficient method for **machine unlearning**. It selectively scales down (dampens) model parameters most responsible for a given forget data subset, while preserving model performance on retained data.

Unlike retraining or adversarial unlearning, SSD performs *targeted, in-place parameter dampening*, guided by Fisher Information  importance scores.

---

## 📊 Features

- ✅ Compute Fisher Information Matrix (diagonal approximation)
- ✅ Measure importance of parameters for both forget and retain data
- ✅ Apply SSD update rule to selectively dampen parameters
- ✅ Track fraction of weights affected
- ✅ Compare retain and forget set performance pre- and post-unlearning


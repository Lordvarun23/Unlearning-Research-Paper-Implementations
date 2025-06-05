# Unlearning-Research-Paper-Implementations
A collection of reproducible implementations of state-of-the-art research papers in **machine unlearning**. This repository provides clean, modular, and well-documented codebases for various unlearning algorithms, enabling benchmarking, experimentation, and further research in privacy-preserving AI.

---

## Overview

Machine unlearning is an emerging area focused on enabling models to selectively forget specific data points without the need for full retraining. This capability is increasingly important for complying with privacy regulations such as GDPR and CCPA, and for improving data lifecycle management in AI systems.

## Papers Implemented ✅

- [x] **Can Bad Teaching Induce Forgetting? Unlearning in Deep Networks using an Incompetent Teacher**  - Chundawat et al. - AAAI 2023
- [ ] Amnesiac Unlearning  
- [ ] UNSIR  
- [x] **Fast Machine Unlearning Without Retraining Through Selective Synaptic Dampening (SSD)**  - Jack Foster et al. - AAAI 2024
- [ ] (Add more here...)

---
## 📊 Benchmark Results [Unlearning Rocket Subclass in CIFAR20 Dataset with ResNet18 Model]

| Unlearning Method                                      | Retain Accuracy (%) | Forget Accuracy (%) | Time Taken for Unlearning (s) |
|:-------------------------------------------------------|:--------------------|:--------------------|:------------------------------|
| Trained Model                                          | 80.2                | 82.5                | NA                            |
| BadTeacher                                             | 81.7                | 3.2                 | 40                            |
| SSD                                                    | 79.2                | 0.02                | 110                           |
| Amnesiac Unlearning                                    | -                   | -                   | -                             |
| UNSIR                                                  | -                   | -                   | -                             |

### 📌 Notes:
- **Retain Accuracy**: Accuracy on the retained test set (data the model should remember)
- **Forget Accuracy**: Accuracy on the forget set (data the model should forget — lower is better)
- **Time Taken**: Total time (in seconds) for the unlearning process only (excluding initial training)


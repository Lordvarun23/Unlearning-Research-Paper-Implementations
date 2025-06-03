# Bad Teaching Unlearning on CIFAR-Super20

This repository contains my implementation of the **"Can Bad Teaching Induce Forgetting? Unlearning in Deep Networks using an Incompetent Teacher"** paper (AAAI 2023) applied on the **CIFAR-Super20 dataset**.

The work introduces a novel machine unlearning framework where an *incompetent teacher* model guides a student to forget specific data while retaining knowledge from a *competent teacher*. This implementation focuses on evaluating the impact of bad teaching on **retain and forget accuracy**.

---

## 📌 Paper Reference

> **Can Bad Teaching Induce Forgetting? Unlearning in Deep Networks using an Incompetent Teacher**  
> Vikram S. Chundawat, Ayush K. Tarun, Murari Mandal, Mohan Kankanhalli  
> [AAAI 2023 Paper](https://arxiv.org/abs/2205.08096)

---

## 📊 Results (Sub Class Forgetting-Rocket)

| Phase                       | Retain Accuracy | Forget Accuracy       |
|:----------------------------|:----------------|:----------------------|
| Trained Model               |  **77%**         |  **69%**              |
| After Unlearning            |  **76.8%**         | **5%** (↓ clear drop) |




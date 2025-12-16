# Semantic and Structural Fusion for Code Smell Detection

Code smell detection using **CodeBERT embeddings** + **Random Forest / MLP** on the **SmellyCode++** dataset.

This project is my **CS 298 Master’s Project** at **San José State University**.

---

## Overview

- Use **CodeBERT (`microsoft/codebert-base`)** to embed Java code into **768-dimensional vectors**
- Train **Random Forest** and **MLP** on those embeddings for **binary classification**: `smelly` vs `clean`
- Experiments done on a **balanced 5K subset** of SmellyCode++ (2.5K smelly, 2.5K clean)
- Both models achieve around **78% accuracy** using embeddings alone (no handcrafted metrics)

---

## Repo Structure

```text
.
├─ 
├─ presentationDeck.pptx               # Presentation
├─ 298-final-report.pdf            # Final report
├─ code_smell_detection.ipynb   # Main experiment notebook
└─ data/
    └─ smellycodepp/        #  SmellyCode++ dataset

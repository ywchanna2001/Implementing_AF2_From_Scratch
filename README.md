# AlphaFold2 From Scratch

A research-oriented reimplementation of the AlphaFold2 architecture with the goal of understanding and reproducing the core algorithmic components of modern protein structure prediction systems.

This repository focuses on implementing the major modules of AlphaFold2 step-by-step from first principles, with an emphasis on clarity, modularity, mathematical correctness, and reproducibility rather than production-scale inference speed.

---

## Project Goals

- Reproduce the core architectural components of AlphaFold2
- Develop an in-depth understanding of geometric deep learning for proteins
- Implement the mathematical foundations behind structure prediction
- Build modular and well-documented components for experimentation
- Explore the relationship between attention mechanisms, evolutionary information, and 3D protein structure generation

---

## Planned / Implemented Components

### Input & Embedding
- Input embedding pipeline
- Multiple Sequence Alignment (MSA) representation
- Pair representation initialization
- Positional and relative encodings

### Evoformer
- MSA row attention
- MSA column attention
- MSA transition
- Outer product mean
- Triangle multiplication (incoming/outgoing)
- Triangle attention (starting/ending node)
- Pair transition

### Structure Module
- Invariant Point Attention (IPA)
- Backbone frame generation
- Torsion angle prediction
- Atom coordinate reconstruction

### Training & Optimization
- Recycling mechanism
- Loss functions
  - FAPE loss
  - Distogram loss
  - Torsion angle loss
  - Confidence prediction losses
- Training and inference utilities

---

## Technical Focus

This implementation emphasizes:

- PyTorch-based modular design
- Mathematical transparency of each operation
- Clean tensor-level implementations
- Geometric reasoning in 3D space
- Reproducible experiments
- Educational value for researchers and students

---

## Repository Objectives

The main objective of this repository is not only to reproduce AlphaFold2, but also to deeply understand:

- Why Evoformer works
- How geometric inductive biases are integrated into transformers
- The role of evolutionary information in protein folding
- Rotation and translation equivariance in structural biology models
- Efficient tensor operations used in large-scale protein models

---

## Disclaimer

This project is an independent educational and research implementation inspired by the AlphaFold2 architecture described by DeepMind and related publications.

It is **not** an official implementation and is **not intended** to replicate the full-scale training pipeline, datasets, or proprietary optimizations used in the original system.

---

## References

- AlphaFold2 papers and supplementary materials
- DeepMind publications
- OpenFold
- Protein Data Bank (PDB)
- "Attention Is All You Need"

---

## Tagline

> A modular PyTorch reimplementation of AlphaFold2 focused on understanding Evoformer, IPA, and geometric protein structure prediction from first principles.

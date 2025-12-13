## DCGAN — From-Scratch Implementation (PyTorch)

A research-driven reproduction of Deep Convolutional Generative Adversarial Networks, grounded in the theory of the original GAN paper.

## Overview

This project implements DCGAN (Radford et al., 2015) from scratch in PyTorch, after a deep theoretical study of the original GAN (Goodfellow et al., 2014).
The goal is to understand why DCGAN training is stable, what architectural decisions matter, and how the generator and discriminator co-evolve during training.

## Theory Background

### Original GAN (2014) 

*Minimax objective

*Why non-saturating loss is preferred

*JS divergence and training instability

*Why generator & discriminator gradients often conflict

*Source of mode collapse

### DCGAN (2015)

*DCGAN stabilizes GANs by enforcing:

*No fully connected layers

*Use of strided convolutions

BatchNorm in both G and D

*ReLU activations in G, LeakyReLU in D

*Tanh output for G

*Normal weight initialization

**This repository follows these design principles precisely.**

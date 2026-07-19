---
layout: page
title: Projects
navigation: true
logo: 'assets/images/fairy.jpg'
current: projects
permalink: /projects/
show_layout_title: false
---

{% include section-header.html %}

My work is available primarily through the  <a href="https://github.com/JenWei0312" target="_blank" rel="noopener noreferrer"><img src="/assets/images/github_icon.png" alt="GitHub Icon" width="32" height="32" style="display: inline-block;"> and 🤗 [Hugging Face Hub](https://huggingface.co/bird-of-paradise). These projects range from first-principles implementations of modern AI systems to original research on optimization, memory, and training dynamics.

## Muon-Based Optimization for GRPO

I am developing a Muon-based optimizer variant for GRPO-style reinforcement learning. The project examines whether Muon’s matrix-aware updates can improve stability and optimization behavior in reinforcement-learning settings, where noisy rewards and long-horizon generation create dynamics very different from pretraining.

The work includes optimizer design, integration into the training loop, instrumentation of gradient behavior, and controlled comparisons against conventional optimization baselines.

[View the repo](https://huggingface.co/bird-of-paradise/Llama-Hopper-Reasoning-v1)

## Engram Conditional Memory in `olmo-core`

I extended `olmo-core` with Engram conditional memory to study how external memory interacts with attention-based and hybrid architectures.

The project became a broader investigation of architecture-specific learning dynamics. I traced anomalous loss and gradient behavior to implementation defects, corrected the integration, and reran the experiments to separate genuine memory effects from artifacts of the original code.

[View the repo](https://github.com/JenWei0312/OLMo-core/tree/feature/engram-poc)

## Distributed Muon

A reverse-engineered and annotated implementation of Moonshot AI’s distributed Muon optimizer, with an emphasis on multi-node communication, CPU offloading, and the systems decisions that make Muon practical at scale.

[View the project](https://huggingface.co/datasets/bird-of-paradise/muon-distributed)

## Understanding the Muon Optimizer

A theory-to-code guide to Muon, covering Newton–Schulz orthogonalization, matrix-shaped parameter updates, and the differences between Muon and conventional adaptive optimizers.

[View the tutorial](https://huggingface.co/datasets/bird-of-paradise/muon-tutorial)

## Reinforcement Learning for Tool Use

A hands-on implementation of ReTool, exploring how reinforcement learning can teach language models when and how to invoke external tools across multi-step reasoning trajectories.

[View the implementation](https://huggingface.co/spaces/bird-of-paradise/ReTool-Implementation)

## Model Architecture from First Principles

Implementations of DeepSeek’s Multi-Head Latent Attention and Mixture-of-Experts architectures, along with a complete Transformer-from-scratch tutorial.

* [Multi-Head Latent Attention](https://huggingface.co/bird-of-paradise/deepseek-mla)
* [Mixture-of-Experts](https://huggingface.co/bird-of-paradise/deepseek-moe)
* [Transformer from Scratch](https://huggingface.co/datasets/bird-of-paradise/transformer-from-scratch-tutorial)

## Post-Training Methods, Visualized

An interactive guide to distillation, preference optimization, RLHF, DPO, and related post-training methods.

[View the guide](https://huggingface.co/spaces/bird-of-paradise/post-training-techniques-guide)
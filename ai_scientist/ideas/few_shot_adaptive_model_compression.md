# I Can't Believe It's Not Better: Few-Shot Adaptive Model Compression

## Keywords
model compression, few-shot learning, adaptive pruning, meta-distillation, parameter efficiency

## TL;DR
AdaCompact enables dynamic model compression for few-shot learning scenarios through task-conditioned pruning and gradient-aware distillation.

## Abstract
Model compression techniques are essential for deploying deep learning in resource-constrained environments but face significant challenges in dynamic few-shot learning scenarios. We introduce AdaCompact, a novel framework combining dynamic magnitude pruning with task-conditioned threshold adaptation and gradient-aware knowledge distillation. Our approach features task-aware compression policies that automatically adjust pruning strategies based on target task requirements, coupled with distillation objectives that prioritize transferable feature representations. Experimental results on few-shot benchmarks show AdaCompact achieves 93% of original model performance at 30% parameter count, outperforming static compression baselines by 12.7% accuracy while maintaining comparable few-shot adaptation capabilities.

## Introduction
- Contrast static vs dynamic compression requirements in few-shot learning
- Limitations of current pruning/distillation in meta-learning scenarios

## Methodology
- Task-conditioned pruning threshold adaptation
- Gradient-sensitive knowledge distillation
- Meta-learning compression policies

## Innovations
- Dynamic pruning strategy adapts to task embeddings
- Distillation loss preserves gradient directions critical for few-shot adaptation
- Unified framework for compression-aware meta-learning

## Experiments
- Benchmarks: Mini-ImageNet (5-way 1/5-shot), Omniglot
- Comparison against magnitude/random pruning baselines
- Ablation on distillation components

## Key Innovations
1. First integration of dynamic pruning with meta-learning
2. Task-aware distillation preserving few-shot gradients
3. Compression ratio adaptation based on task complexity
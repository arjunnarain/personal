---
title: "Attention Is All You Need"
date: 2025-08-31
draft: false
tags: ["transformer", "attention", "nlp", "deep-learning"]
categories: ["research-papers"]
author: "Vaswani et al."
journal: "NeurIPS"
year: "2017"
doi: "10.5555/3295222.3295349"
paper_url: "https://arxiv.org/abs/1706.03762"
drive_link: "#"
summary: "The seminal paper that introduced the Transformer architecture, revolutionizing natural language processing by relying entirely on attention mechanisms."
reading_status: "read-notes"
ShowToc: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowShareButtons: true
---

## Abstract

The dominant sequence transduction models are based on complex recurrent or convolutional neural networks that include an encoder and a decoder. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely.

## Key Contributions

- Introduced the Transformer architecture based entirely on self-attention
- Eliminated the need for recurrent and convolutional layers
- Achieved state-of-the-art results on machine translation tasks
- Enabled much better parallelization during training
- Laid the foundation for modern large language models

## My Notes

### Main Findings

This paper fundamentally changed how we think about sequence modeling. The key insight is that attention mechanisms alone, without recurrence or convolution, can achieve superior performance on sequence transduction tasks.

### Methodology

The Transformer uses:
- **Multi-head self-attention**: Allows the model to attend to different representation subspaces
- **Position encodings**: Since there's no recurrence, positional information is added via sinusoidal encodings
- **Feed-forward networks**: Applied to each position separately
- **Layer normalization and residual connections**: For training stability

### Strengths

- Much faster training due to parallelization
- Better long-range dependency modeling
- Cleaner, more interpretable architecture
- Strong empirical results on translation tasks

### Limitations

- Quadratic complexity with sequence length
- Requires more data compared to RNNs for shorter sequences
- Position encoding scheme may not be optimal for all tasks

### Questions/Future Work

- How can we reduce the quadratic complexity?
- Can attention patterns be made more sparse?
- What other tasks can benefit from this architecture?

## Related Work

- Builds on attention mechanisms from Bahdanau et al. (2015)
- Improves upon seq2seq models with attention
- Influenced by convolutional sequence-to-sequence learning

## Citation

```bibtex
@article{vaswani2017attention,
  title={Attention is all you need},
  author={Vaswani, Ashish and Shazeer, Noam and Parmar, Niki and Uszkoreit, Jakob and Jones, Llion and Gomez, Aidan N and Kaiser, {\L}ukasz and Polosukhin, Illia},
  journal={Advances in neural information processing systems},
  volume={30},
  year={2017}
}
```

## Links

- [📄 Original Paper](https://arxiv.org/abs/1706.03762)
- [📝 Annotated PDF](#) <!-- Replace with your Google Drive link -->
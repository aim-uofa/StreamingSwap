# StreamingSwap

**From Short Clips to Real-Time Streams: Identity-Aware Supervision and Context-Efficient Generation for Video Face Swapping**

Zekai Luo*, Yuwei Liang*, Ruiqi Ma, Haoyu Huang, Xuehao Wang, Huanyi Zheng, Mingyu Liu, Linhao Zhong, Chenchen Jing, Yuling Xi†, Hao Chen†  
Zhejiang University · Zhejiang University of Technology  
*Equal contribution · †Corresponding authors

**[Project page](https://aim-uofa.github.io/StreamingSwap/)** · Paper: link to be added · Code and checkpoints: coming soon

## Teaser

<p align="center">
  <img src="https://raw.githubusercontent.com/aim-uofa/aim-uofa.github.io/refs/heads/master/StreamingSwap/assets/teaser.png" alt="StreamingSwap teaser showing professional film, live streaming, and AI-generated drama face-swapping examples" width="900">
</p>

## Abstract

Video face swapping transfers the reference identity to a target video while preserving its other attributes and motion. Despite recent progress in reference-guided flow-based methods, jointly achieving faithful identity transfer, high fidelity, and real-time generation over long video streams remains challenging. To address this challenge, we rethink the task-specific structure of reference-guided video face swapping. First, face swapping changes only identity while preserving most visual content, yet flow-matching supervision is weakly sensitive to these changes. We therefore develop Joint Rec-ID Loss, which balances explicit identity supervision and latent reconstruction according to the noise level. Second, the target video already provides non-edited attributes and temporal dynamics, enabling generation with fewer spatial tokens and shorter temporal contexts through Face-RoI Generation and Short-Context Rollout Training. By integrating these designs, we propose StreamingSwap, a reference-guided flow-matching framework for real-time streaming video face swapping. We also introduce HumanFaceVid, comprising 1,000 hours of cinematic training data and evaluation sets of 200 short and 200 long videos. Experiments demonstrate that our method achieves competitive identity transfer and visual quality at 20 FPS on a single NVIDIA RTX 4090 GPU, with stable generation over videos up to 10 minutes long.

## Highlights

- **Identity-aware supervision:** Joint Rec-ID Loss combines identity and reconstruction objectives according to the noise level.
- **Context-efficient generation:** Face-RoI Generation and Short-Context Rollout Training reduce the spatial and temporal context needed for streaming.
- **Real-time, long-video results:** The final streaming model reaches 21.174 FPS on one NVIDIA RTX 4090 and supports videos up to 10 minutes long.
- **HumanFaceVid:** 1,000 hours of cinematic training data, with evaluation sets of 200 short and 200 long videos.

## Release status

This repository is being prepared for the official code release. Source code, checkpoints, and usage instructions will be added here when available.

## Citation

BibTeX will be added when the paper's publication details are available.

<p align="center">
  <img src="https://aim-uofa.github.io/StreamingSwap/assets/streamingswap-logo-white.svg" alt="StreamingSwap" width="480">
</p>

<h3 align="center">From Short Clips to Real-Time Streams: Identity-Aware Supervision and Context-Efficient Generation for Video Face Swapping</h3>

<p align="center">
  Zekai Luo*, Yuwei Liang*, Ruiqi Ma, Haoyu Huang, Xuehao Wang, Huanyi Zheng, Mingyu Liu, Linhao Zhong, Chenchen Jing, Yuling Xi†, Hao Chen†<br>
  Zhejiang University · Zhejiang University of Technology<br>
  *Equal contribution · †Corresponding authors
</p>

<p align="center">
  <a href="https://arxiv.org/abs/2610.26681"><img src="https://aim-uofa.github.io/StreamingSwap/assets/readme-paper-badge.svg?v=5" alt="Paper on arXiv" height="30"></a>
  <a href="https://aim-uofa.github.io/StreamingSwap/"><img src="https://aim-uofa.github.io/StreamingSwap/assets/readme-project-badge.svg" alt="Project Page" height="30"></a>
  <img src="https://aim-uofa.github.io/StreamingSwap/assets/readme-dataset-badge.svg?v=4" alt="Dataset on ModelScope: coming soon" height="30">
</p>

<p align="center">Reference-guided face swapping for real-time video streams, preserving target attributes and motion.</p>

<p align="center">
  <img src="https://aim-uofa.github.io/StreamingSwap/assets/teaser.png" alt="StreamingSwap teaser showing professional film, live streaming, and AI-generated drama face-swapping examples" width="900">
</p>

## Highlights

- **Identity-aware supervision:** Joint Rec-ID Loss combines identity and reconstruction objectives according to the noise level.
- **Context-efficient generation:** Face-RoI Generation and Short-Context Rollout Training reduce the spatial and temporal context needed for streaming.
- **Real-time, long-video results:** The final streaming model reaches 21.174 FPS on one NVIDIA RTX 4090 and supports videos up to 10 minutes long.
- **HumanFaceVid:** 1,000 hours of cinematic training data, with evaluation sets of 200 short and 200 long videos.

## Method

<p align="center">
  <img src="https://aim-uofa.github.io/StreamingSwap/assets/method.png" alt="StreamingSwap method: identity-aware Face-RoI training followed by self-rollout training" width="900">
</p>

In Phase I, Face-RoI Generation focuses computation on the face region, while Joint Rec-ID Loss balances identity and reconstruction supervision according to the noise level. In Phase II, Short-Context Rollout Training uses generated history to reduce error accumulation during streaming.

## Data Construction

<p align="center">
  <img src="https://aim-uofa.github.io/StreamingSwap/assets/data-construction.png" alt="HumanFaceVid data construction and reverse-paired training" width="900">
</p>

Built from OpenHumanVid, HumanFaceVid provides 1,000 hours of training data and evaluation sets of 200 short and 200 long videos. Reverse-paired training uses synthetic face-swapped inputs and the original real videos as ground truth.

## Release Plan

We are preparing the following releases:

- [ ] Inference code
- [ ] Evaluation code and data
- [ ] Training code
- [ ] Data construction code and training data

## Citation

```bibtex
@misc{luo2026streamingswap,
  title={From Short Clips to Real-Time Streams: Identity-Aware Supervision and Context-Efficient Generation for Video Face Swapping},
  author={Zekai Luo and Yuwei Liang and Ruiqi Ma and Haoyu Huang and Xuehao Wang and Huanyi Zheng and Mingyu Liu and Linhao Zhong and Chenchen Jing and Yuling Xi and Hao Chen},
  year={2026},
  eprint={2610.26681},
  archivePrefix={arXiv},
  primaryClass={cs.CV},
  url={https://arxiv.org/abs/2610.26681}
}
```

# Awesome Self-Forcing for Video Diffusion [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of papers, code, and resources about **Self-Forcing-style autoregressive video diffusion**.

This repo focuses on the research line around:
- train-test gap in autoregressive video generation
- long-horizon stability
- streaming / real-time inference
- distillation and ODE initialization strategies

---

## Table of Contents
- [Awesome Self-Forcing for Video Diffusion ](#awesome-self-forcing-for-video-diffusion-)
  - [Table of Contents](#table-of-contents)
  - [What is this list](#what-is-this-list)
  - [Papers](#papers)
  - [Contributing](#contributing)
  - [Citation](#citation)

---

## What is this list

Self-Forcing family methods aim to reduce the mismatch between:
- **training-time inputs** (often teacher-forced or clean context), and
- **inference-time rollout** (model-generated context with accumulated errors).

This repository tracks papers and implementations that directly address this issue for autoregressive video diffusion.

---

## Papers

| Year | Title | Paper | Code / Project | Notes |
|---|---|---|---|---|
| 2025 | **Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion** | [arXiv:2506.08009](https://arxiv.org/abs/2506.08009) | [Project](https://self-forcing.github.io/) | Starting point of the self-forcing line |
| 2025 | **Rolling Forcing: Autoregressive Long Video Diffusion in Real Time** | [arXiv:2509.25161](https://arxiv.org/abs/2509.25161) | [Code](https://github.com/TencentARC/RollingForcing) · [Project](https://kunhao-liu.github.io/Rolling_Forcing_Webpage/) | Rolling/chunk-style long-horizon generation |
| 2025 | **Reward Forcing: Efficient Streaming Video Generation with Rewarded Distribution Matching Distillation** | [arXiv:2512.04678](https://arxiv.org/abs/2512.04678) | [Code](https://github.com/JaydenLyh/Reward-Forcing) | Reward-weighted distillation for streaming quality |
| 2025 | **Self-Forcing++: Towards Minute-Scale High-Quality Video Generation** | [arXiv:2510.02283](https://arxiv.org/abs/2510.02283) | - | Minute-scale long video extension |
| 2025 | **End-to-End Training for Autoregressive Video Diffusion via Self-Resampling** | [arXiv:2512.15702](https://arxiv.org/abs/2512.15702) | - | End-to-end AR training and stabilization |
| 2026 | **Causal Forcing: Autoregressive Diffusion Distillation Done Right for High-Quality Real-Time Interactive Video Generation** | [arXiv:2602.02214](https://arxiv.org/abs/2602.02214) | [Code](https://github.com/thu-ml/Causal-Forcing) · [Project](https://thu-ml.github.io/CausalForcing.github.io/) | AR teacher + ODE init + causal distillation |

---

## Contributing

Contributions are welcome.

Please open a PR and add entries with the following format:

- Title
- Year
- Paper link
- Code link (optional)
- Project page (optional)
- 2-5 keywords
- One-line relevance to self-forcing

---

## Citation

If this repository helps your research, please consider citing:

```bibtex
@misc{awesome_self_forcing_video_diffusion,
  title={Awesome Self-Forcing for Video Diffusion},
  author={Community Contributors},
  year={2026},
  howpublished={\url{https://github.com/ealicesora/awesome-video-forcing}}
}
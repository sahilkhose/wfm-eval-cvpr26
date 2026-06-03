# WFM-Eval: An Evaluation Framework for Video World Models in Robotic Manipulation

[**Project page**](https://sahilkhose.github.io/wfm-eval-cvpr26/) · [**Paper (PDF)**](assets/wfm-eval-paper.pdf) · [**Poster (PDF)**](assets/wfm-eval-poster.pdf)

[Sahil Khose](https://sahilkhose.github.io/)¹, Mengqi Zhang¹, Prithvijit Chattopadhyay², Judy Hoffman¹
&nbsp;&nbsp;|&nbsp;&nbsp; ¹UC Irvine &nbsp;·&nbsp; ²NVIDIA

> Accepted at the **1st Workshop on Video World Models (VWM)** and the **2nd Workshop on Foundation Models Meet Embodied Agents (FMEA)**, CVPR 2026.

> **Code coming soon.** The WFM-Eval toolkit (evaluation pipeline, metrics, and scripts) will be released in this repository soon. In the meantime, this repo hosts the [project page](https://sahilkhose.github.io/wfm-eval-cvpr26/).

WFM-Eval is a multi-dimensional evaluation framework for video world models in
robot manipulation. It decomposes video quality into three axes (**task
completion**, **object hallucination**, and **temporal consistency**) with
structured, object-level diagnostics scored by an automated VLM-grounding
pipeline that bypasses unreliable holistic judgment.

**Key findings**

1. Object hallucination is the dominant model-discriminative failure mode.
2. Model rankings reverse across datasets, so single-dataset benchmarks mislead.
3. The framework's hallucination ranking predicts downstream policy success on
   LIBERO (Predict2 beats Predict2.5 by +8.75 points).

## This repository

A static project page served via GitHub Pages.

```
index.html        the project page
stylesheet.css    styling (Inter + JetBrains Mono, light/dark)
favicon.svg
assets/
  poster.png            rendered poster (2400px)
  wfm-eval-poster.pdf   full-resolution poster
  wfm-eval-paper.pdf    camera-ready paper
  fig-radar.png         Figure 1: VLM-judge accuracy
  fig-taxonomy.png      Figure 2: error taxonomy
  fig-failure.png       Figure 3: failure modes
  fig-severity.png      Figure 4: severity distributions
```

To preview locally: open `index.html`, or run `python3 -m http.server` and
visit <http://localhost:8000>.

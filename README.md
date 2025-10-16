# 🛰️ RareFlow: Physics-Aware Flow-Matching for Cross-Sensor Super-Resolution of Rare-Earth Features

<p align="left">
  <!-- TODO: Update links/IDs or remove badges you don't want -->
  <a href="https://arxiv.org/abs/2402.05195">
    <img alt="arXiv" src="https://img.shields.io/static/v1?label=ArXiv&message=2402.05195&color=B31B1B&logo=arxiv">
  </a>
  <img alt="Status: Under review" src="https://img.shields.io/badge/status-under_review-ffaa00">
  <a href="./LICENSE">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-informational">
  </a>
  <a href="https://github.com/USER/rareflow/actions">
    <img alt="CI" src="https://img.shields.io/badge/CI-coming_soon-lightgrey">
  </a>
</p>

> **TL;DR**: RareFlow is a physics-aware, dual-conditioned flow-matching framework for cross-sensor super-resolution (SR) of rare geomorphic features.  
---

## 🗞️ News
- **TBA** — public release of code & weights after paper acceptance. Watch ⭐ the repo to get notified.

---

## ⭐ Highlights
- **Dual-conditioning with gated ControlNet** to balance LR structure vs. semantic priors.
- **Physics-aware objective:** FFT-magnitude alignment + CIELAB radiometric consistency + LPIPS.
- **Uncertainty-aware control:** MC-dropout drives per-block gates to reduce prior “creativity” on OOD inputs.
- **Unified SR + harmonization:** Cross-sensor style transfer while preserving geometry.
- **Benchmark results:** Strong perceptual quality (e.g., ~40% FID reduction) with competitive fidelity. <!-- TODO: Confirm/adjust numbers -->

---

## 🛰️ Datasets & Task

- **Input:** 10 m Sentinel-2 RGB tiles (12-bit → normalized).  
- **Target:** 2 m Maxar RGB tiles; cross-sensor and cross-temporal pairs with small spatial/temporal misalignments.  
- **Focus:** Rare geomorphic features (e.g., **retrogressive thaw slumps (RTS)**) in Arctic regions.  
- **Notes:** Strong domain shift, small crop sizes, non-standard dynamic range.

> We will release pre-processing & normalization utilities (percentile and fixed-range) and pairing scripts **upon acceptance**.

<p align="center">
  <img src="assets/data_challenges.png" alt="Data challenges: radiometry, misalignment, crop size (placeholder)" width="80%">
</p>

---

## 🗺️ Roadmap

- [ ] Release training & evaluation code
- [ ] Upload pretrained weights for target sensor styles
- [ ] Publish data preparation & pairing scripts
- [ ] Add model card & responsible-use guidance
- [ ] Provide reproducibility scripts and exact env (`environment.yml`)
- [ ] Colab / demo notebook

---

## 🧑‍⚖️ Model Card & Responsible Use (Coming Soon)

---

## 📝 Citation

If you find RareFlow useful, please cite:

```bibtex
@inreview{fallah2026rareflow,
  title   = {RareFlow: Physics-Aware Flow-Matching for Cross-Sensor Super-Resolution of Rare-Earth Features},
  author  = {Fallah, Forouzan and Li, Wenwen and Hsu, Chia-Yu and Lee, Hyunho and Yang, Yezhou},
  year    = {2026},
  note    = {Under review},
}
```

## ✉️ Contact & Acknowledgments

- **Contact:** ffallah@asu.edu
- We thank collaborators and domain experts who contributed to evaluation and feedback.


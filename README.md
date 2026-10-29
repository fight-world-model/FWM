<h1 align="center">Fight World Model</h1>

<p align="center"><b>Customizable Combat through Visual Interaction Proxies</b></p>

<p align="center">
  <a href="https://fight-world-model.github.io/"><img src="https://img.shields.io/badge/Project-Page-blue" alt="Project page"></a>
  <a href="https://fight-world-model.github.io/media/paper.pdf"><img src="https://img.shields.io/badge/Paper-PDF-red" alt="Paper PDF"></a>
</p>

<p align="center">
  <img src="assets/teaser.png" width="100%" alt="Fight World Model overview: character and arena customization, executable combat rules, and controllable skills">
</p>

<p align="center">
  <i>Execute the rules. Render the fight.</i>
</p>

> Fight World Model (FWM) connects executable combat rules to video generation through a visual interaction proxy. An engine resolves interactions and maintains state; a deterministic compiler aligns actions and their consequences with fighter identities and video frames; a video model renders the resulting fight with character and arena references.

A protected fighter can react to a hit without losing health, while lifesteal damages the recipient and heals the attacker. FWM renders these outcomes under edited rules without retraining the renderer. Changing a character or arena reference preserves the prescribed interaction, and identity binding keeps appearances associated with the intended fighters across side switches.

## 📰 News

- **[2026-10]** The [project page](https://fight-world-model.github.io/) and [paper](https://fight-world-model.github.io/media/paper.pdf) are available.

## 🚀 Release roadmap

- [x] Project page
- [x] Technical report: [PDF](https://fight-world-model.github.io/media/paper.pdf)
- [ ] Inference code
- [ ] Pretrained weights

## Method

<p align="center">
  <img src="assets/framework.png" width="100%" alt="FWM architecture: an executable proxy engine, interaction proxy compilation, a video renderer, and appearance and identity binding">
</p>

The interaction proxy separately encodes attempted actions, brief hit reactions, and persistent health on a shared canvas and timeline. This separation lets the engine specify damage scaling, limited-hit immunity, lifesteal, and multi-stage skill mechanisms through the same conditioning format.




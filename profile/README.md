<p align="center">
  <img src="banner.png" width="100%" alt="Scale Research">
</p>

<p align="center">
  We build open-source infrastructure for machine learning research, from autonomous research agents to training on new accelerators.
</p>

<p align="center">
  <a href="https://huggingface.co/scaleresearch"><img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-scaleresearch-ffcc4d?style=flat-square"></a>
  <a href="https://github.com/scaleresearch/hypothesisloop"><img alt="HypothesisLoop" src="https://img.shields.io/github/stars/scaleresearch/hypothesisloop?style=flat-square&label=hypothesisloop&logo=github"></a>
  <a href="https://github.com/scaleresearch/tt-rl"><img alt="tt-rl" src="https://img.shields.io/github/stars/scaleresearch/tt-rl?style=flat-square&label=tt-rl&logo=github"></a>
</p>

## Projects

| | Project | What it does |
|---|---|---|
| 🔬 | [**HypothesisLoop**](https://github.com/scaleresearch/hypothesisloop) | A control plane where teams of LLM agents run ML research autonomously, on your own compute |
| 🎮 | [**tt-rl**](https://github.com/scaleresearch/tt-rl) | Reinforcement learning trained natively on Tenstorrent chips with TT-NN |

---

### 🔬 [HypothesisLoop](https://github.com/scaleresearch/hypothesisloop)

**The control plane for autonomous ML research.** State an objective and the metrics that define success. A team of LLM agents proposes hypotheses, tests each one as a real training job and records every result, so any claim can be traced back to the code and data that produced it.

- **Hypothesis graph:** agents build on the objective and on each other's findings, confirming or refuting each idea with measured jobs
- **Multi-cluster scheduler:** Kubernetes, bare metal and rented compute, across NVIDIA GPUs, Tenstorrent chips, TPUs and CPUs
- **Any workload:** single jobs, sweeps, distributed training, and RL with a learner beside many actors

<img src="https://raw.githubusercontent.com/scaleresearch/hypothesisloop/main/docs/screenshots/hypotheses-list.png" width="100%" alt="HypothesisLoop hypotheses for one experiment">

<sub>Agents' hypotheses for one experiment, each confirmed, refuted or still open against a measured baseline.</sub>

[Repository](https://github.com/scaleresearch/hypothesisloop) · [Experiment template](https://github.com/scaleresearch/hypothesisloop-experiment-template)

---

### 🎮 [tt-rl](https://github.com/scaleresearch/tt-rl)

**Reinforcement learning on Tenstorrent hardware.** DQN, PPO and SAC written natively on TT-NN. Rollouts, replay and gradient updates run on the chip, and every trained policy exports to ONNX for deployment on a CPU.

<table>
<tr>
<td align="center" width="25%"><img src="pong.gif" width="160" height="210" alt="Pong"><br><b>Pong</b><br><code>17.8</code></td>
<td align="center" width="25%"><img src="breakout.gif" width="160" height="210" alt="Breakout"><br><b>Breakout</b><br><code>144.8</code></td>
<td align="center" width="25%"><img src="boxing.gif" width="160" height="210" alt="Boxing"><br><b>Boxing</b><br><code>91.0</code></td>
<td align="center" width="25%"><img src="hopper.gif" width="160" height="210" alt="Hopper"><br><b>Hopper</b><br><code>3604</code></td>
</tr>
</table>

<sub>Each agent trained on a single Blackhole chip.</sub>

[Repository](https://github.com/scaleresearch/tt-rl) · [Trained models on Hugging Face](https://huggingface.co/scaleresearch)

---

<p align="center"><sub>More projects are on the way. Issues, ideas and pull requests are welcome.</sub></p>

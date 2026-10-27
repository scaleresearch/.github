<h1 align="center">Scale Research</h1>

<p align="center">
  Open-source tools for machine learning research: a platform where LLM agents run ML research autonomously, and reinforcement learning on Tenstorrent accelerators.
</p>

<p align="center">
  <a href="https://huggingface.co/scaleresearch"><img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-scaleresearch-ffcc4d"></a>
  <a href="https://github.com/scaleresearch/tt-rl/blob/master/LICENSE"><img alt="MIT" src="https://img.shields.io/badge/license-MIT-blue"></a>
</p>

---

## [HypothesisLoop](https://github.com/scaleresearch/hypothesisloop)

The control plane for autonomous ML research. State an objective and the metrics that define success, and a team of LLM agents proposes hypotheses, tests them as real jobs on your compute and records every result, so each claim can be traced and rerun.

<img src="https://raw.githubusercontent.com/scaleresearch/hypothesisloop/main/docs/screenshots/hypothesis-graph.png" width="100%" alt="HypothesisLoop hypothesis graph">

Its scheduler spans Kubernetes clusters, bare-metal nodes and rented compute, across NVIDIA GPUs, Tenstorrent chips, TPUs and CPUs. New experiments start from [hypothesisloop-experiment-template](https://github.com/scaleresearch/hypothesisloop-experiment-template).

## [tt-rl](https://github.com/scaleresearch/tt-rl)

Reinforcement learning on Tenstorrent hardware. DQN, PPO and SAC written natively on TT-NN, with rollouts, replay and gradient updates on the chip, and every trained policy exportable to ONNX.

<table>
<tr>
<td align="center"><img src="https://raw.githubusercontent.com/scaleresearch/tt-rl/master/assets/pong.gif" width="160" alt="Pong"><br><b>Pong</b><br>17.8</td>
<td align="center"><img src="https://raw.githubusercontent.com/scaleresearch/tt-rl/master/assets/breakout.gif" width="160" alt="Breakout"><br><b>Breakout</b><br>144.8</td>
<td align="center"><img src="https://raw.githubusercontent.com/scaleresearch/tt-rl/master/assets/boxing.gif" width="160" alt="Boxing"><br><b>Boxing</b><br>91.0</td>
<td align="center"><img src="https://raw.githubusercontent.com/scaleresearch/tt-rl/master/assets/hopper.gif" width="160" alt="Hopper"><br><b>Hopper</b><br>3604</td>
</tr>
</table>

Each agent was trained on a single Blackhole chip. The weights are on [Hugging Face](https://huggingface.co/scaleresearch).

---

<p align="center"><sub>Issues, ideas and pull requests are welcome on every project.</sub></p>

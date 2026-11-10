## Arkytas

Physical AI lab, Ravensburg. We co-design embodiment, data and policy for learned manipulation: imitation learning from teleoperated demonstrations, RL post-training in sim, and a reliability layer that closes the gap between VLA success rates in the literature and what a production cell needs.

### Stack

- **Embodiments:** open-hardware, 3D-printed arms, swappable end effectors, leader–follower teleop rigs for demonstration capture.
- **Data:** LeRobot-format episodes with QC and per-episode metadata. Sources: teleop, sim rollouts, later deployment logs.
- **Policies:** ACT, Diffusion Policy and SmolVLA benchmarked on identical tasks. Next: specialist models for failure detection, cross-embodiment action mapping and high-precision placement.
- **Sim:** arm and task twin for RL fine-tuning and sim-to-real transfer.

### Eval protocol

- n ≥ 20 rollouts per condition
- Success reported as k/n, never a bare percentage
- Interventions and cycle time logged per rollout
- In-distribution and OOD conditions never pooled

### Status

Phase 1: data pipeline on an SO-101. Repos go public as components stabilise.

Datasets and checkpoints: [huggingface.co/Arkytas](https://huggingface.co/Arkytas)

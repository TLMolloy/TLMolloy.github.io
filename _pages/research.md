---
layout: page
permalink: /research/
title: Research
description: Learning, decision-making, and control under uncertainty for robots and autonomous systems.
nav: true
nav_order: 2
---

My research is on **learning, decision-making, and control under uncertainty for robots and autonomous systems**.

Robots and autonomous systems are increasingly expected to work alongside people and other agents, in environments they cannot fully observe, and with objectives that are rarely known in advance.
My work develops approaches to let them [learn](#learning) from the behaviour of others, [decide](#decision-making) what to sense and when to act with incomplete and changing information, and [control](#control) their interactions with other agents safely.

---
## Current Grants {#grants}
- ARC Discovery Project DP250100112, _"Seeing through Space and Time: Spatio-Temporal Event Processing for Robots"_ (AUD 673k).
- ARC Discovery Project DP250101763, _"Control at What Cost? One-Shot Real-Time Dual Inverse Optimal Control"_ (AUD 340k).
- US Air Force Research Laboratory, Asian Office of Aerospace Research and Development (AOARD), _"Solution Concepts and Performance Guarantees in Partial Information Multi-Player Games"_ (USD 390k).

---

## Learning: Objectives, Intent, and Skills from Behaviour {#learning}

Inverse optimal control (or inverse reinforcement learning) is the problem of inferring the underlying objectives of agents or decision-makers by observing their actions or the consequences of their actions.
Applications include learning reward functions from human demonstrations, modelling bird mid-air collision avoidance, and inferring intent for aircraft collision avoidance.

<div style="display: flex; gap: 1rem; justify-content: center; align-items: center; margin: 2rem 0; flex-wrap: wrap;">
  <div style="text-align: center; flex: 1 1 280px;">
    <img src="{{ site.baseurl }}/assets/img/book_cover.jpg" alt="Inverse Optimal Control and Inverse Noncooperative Dynamic Game Theory book cover" style="height: 340px; width: auto; max-width: 100%; box-shadow: 0 2px 8px rgba(0,0,0,0.15);">
  </div>
  <div style="text-align: center; flex: 1 1 280px;">
    <video height="340" style="width: auto; max-width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
      <source src="{{ site.baseurl }}/assets/videos/ioc_rocket.mp4" type="video/mp4">
    </video>
  </div>
</div>

Selected Papers:

- M. Xu, **T. L. Molloy**, S. Gould. _Revisiting Implicit Differentiation for Learning Problems in Optimal Control._ NeurIPS, 2023. [[link](https://arxiv.org/abs/2310.14468)]
- **T. L. Molloy**, J. Inga, S. Hohmann, T. Perez. _Inverse Optimal Control and Inverse Noncooperative Dynamic Game Theory._ Springer Nature, 2022. [[link](https://link.springer.com/book/10.1007/978-3-030-93317-3)]
- **T. L. Molloy**, J. J. Ford, T. Perez. _Finite-Horizon Inverse Optimal Control for Discrete-Time Nonlinear Systems._ Automatica, 2018. [[link](https://eprints.qut.edu.au/223233/)]
- **T. L. Molloy**, J. J. Ford, T. Perez. _Online Inverse Optimal Control for Control-Constrained Discrete-Time Systems on Finite and Infinite Horizons._ Automatica, 2020. [[link](https://arxiv.org/abs/2005.06153)]
- T. Zhao, **T. L. Molloy**. _Extended Kalman Filtering for Recursive Online Discrete-Time Inverse Optimal Control._ ACC, 2024.
- O. Dry, **T. L. Molloy**, W. Jin, I. Shames. _ZORMS-LfD: Learning from Demonstrations with Zeroth-Order Random Matrix Search._ IEEE Robotics and Automation Letters, 2025. [[link](https://arxiv.org/abs/2507.17096)]

---

## Decision-Making: What to Sense and When to Act {#decision-making}

How should an autonomous system act when it cannot see everything, its sensors are noisy, and the world may change without warning?
My work in this theme develops methods for deciding what information to acquire and how to act on it, for detecting as quickly as possible when the situation has changed, and for sensing and perceiving fast enough to make this possible in dynamic environments.

### Event-Based Sensing and Perception {#event-cameras}

Event cameras are neuromorphic sensors that output asynchronous per-pixel brightness changes, enabling high-speed, low-latency perception.
Applications include high-speed object detection and tracking for robot perception in low-light and dynamic environments.

<div style="text-align: center; margin: 2rem 0;">
  <video width="480" height="360" style="max-width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
    <source src="{{ site.baseurl }}/assets/videos/event_fast.mp4" type="video/mp4">
  </video>
</div>

Selected Papers:

- A. Apps, Z. Wang, V. Perejogin, **T. L. Molloy**, R. Mahony. _Asynchronous Multi-Object Tracking with an Event Camera._ ICRA, 2025. [[link](https://arxiv.org/abs/2505.08126)]
- Z. Wang, **T. L. Molloy**, P. van Goor, R. Mahony. _Asynchronous Blob Tracker for Event Cameras._ IEEE Transactions on Robotics, 2024. [[link](https://arxiv.org/abs/2307.10593)]

### Partially Observed Markov Decision Processes (POMDPs) {#pomdps}

POMDPs are a stochastic control framework for sequential decision-making when the system state is not fully observable.
Applications include autonomous robot exploration, covert navigation, privacy, and cybersecurity.

<div style="display: flex; gap: 2rem; justify-content: center; margin: 2rem 0; flex-wrap: wrap;">
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <p style="font-weight: 600; margin-bottom: 0.5rem;">Standard POMDP</p>
    <video width="100%" height="auto" style="max-width: 350px; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
      <source src="{{ site.baseurl }}/assets/videos/standard_pomdp.mp4" type="video/mp4">
    </video>
  </div>
  <div style="flex: 1; min-width: 300px; text-align: center;">
    <p style="font-weight: 600; margin-bottom: 0.5rem;">Uncertainty-Aware POMDP</p>
    <video width="100%" height="auto" style="max-width: 350px; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
      <source src="{{ site.baseurl }}/assets/videos/uncertainty_aware_pomdp.mp4" type="video/mp4">
    </video>
  </div>
</div>

Selected Papers:

- **T. L. Molloy**. _ISC-POMDPs: Partially Observed Markov Decision Processes with Initial-State Dependent Costs._ IEEE Control Systems Letters, 2025. [[link](https://arxiv.org/abs/2503.05030)]
- **T. L. Molloy**, G. N. Nair. _Entropy-Regularized Partially Observed Markov Decision Processes._ IEEE Transactions on Automatic Control, 2024. [[link](https://arxiv.org/abs/2112.12255)]
- **T. L. Molloy**, G. N. Nair. _Smoother Entropy for Active State Trajectory Estimation and Obfuscation in POMDPs._ IEEE Transactions on Automatic Control, 2023. [[link](https://arxiv.org/abs/2108.10227)]

### Quickest Change Detection {#change-detection}

Quickest change detection is the problem of detecting an abrupt change in a stochastic process as quickly as possible after it occurs while avoiding false alarms.
Applications include vision-based aircraft detection and fault diagnosis.

<div style="text-align: center; margin: 2rem 0;">
  <video width="480" height="360" style="max-width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
    <source src="{{ site.baseurl }}/assets/videos/Detection of Aircraft Below The Horizon_trim.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

Selected Papers:

- **T. L. Molloy**. _Misspecified and Asymptotically Minimax Robust Quickest Change Diagnosis._ IEEE Transactions on Automatic Control, 2021. [[link](https://arxiv.org/abs/2004.09748)]
- **T. L. Molloy**, J. J. Ford. _Minimax Robust Quickest Change Detection in Systems and Signals with Unknown Transients._ IEEE Transactions on Automatic Control, 2019. [[link](https://eprints.qut.edu.au/121741/)]
- **T. L. Molloy**, J. J. Ford. _Misspecified and Asymptotically Minimax Robust Quickest Change Detection._ IEEE Transactions on Signal Processing, 2017. [[link](https://eprints.qut.edu.au/110110/)]

---

## Control: Safe Interaction with Other Agents {#control}

### Dynamic and Differential Game Theory {#game-theory}

Dynamic and differential game theory studies multi-agent systems in which each agent optimises its own objective, knowing that others do likewise.
Applications include autonomous collision avoidance and human–machine teaming.

<div style="text-align: center; margin: 2rem 0;">
  <video width="480" height="360" style="max-width: 100%; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.15);" autoplay loop muted playsinline controls>
    <source src="{{ site.baseurl }}/assets/videos/aiaa_prying_pedestriantrajectory_C.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

Selected Papers:

- P. Braun, **T. L. Molloy**, I. Shames. _Prying Pedestrian Surveillance-Evasion: Minimum-Time Evasion from an Agile Pursuer._ Journal of Guidance, Control, and Dynamics, 2025. [[link](https://arxiv.org/abs/2411.19376)]
- Y. Chen, **T. L. Molloy**, I. Shames. _Two-Player Dynamic Potential LQ Games with Sequentially Revealed Costs._ CDC, 2025. [[link](https://arxiv.org/abs/2503.20234)]
- **T. L. Molloy**, T. Perez, B. P. Williams. _Optimal Bearing-Only-Information Strategy for Unmanned Aircraft Collision Avoidance._ Journal of Guidance, Control, and Dynamics, 2020. [[link](https://arxiv.org/abs/2004.09744)]

### Optimal Control {#optimal-control}

Optimal control is the problem of choosing control inputs that minimise a cost, such as time, energy, or tracking error, subject to a system's dynamics and constraints.
Applications include minimum-time escape and evasion manoeuvres for marine, aerial, and ground robots, and online control of systems whose objectives are revealed only as they operate.

Selected Papers:

- Y. Chen, **T. L. Molloy**, T. Summers, I. Shames. _Regret Analysis of Online LQ Control Using Trajectory Prediction and Tracking._ IEEE Transactions on Automatic Control, 2026. [[link](https://arxiv.org/abs/2302.10411)]
- **T. L. Molloy**, I. Shames. _Minimum-Time Escape from a Circular Region for a Dubins Car._ NOLCOS, 2023. [[link](https://arxiv.org/abs/2211.01706)]


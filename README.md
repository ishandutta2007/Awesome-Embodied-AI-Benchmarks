# Awesome-Embodied-AI-Benchmarks

## Top Embodied AI Benchmarks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Robotic Manipulation, Navigation & Long-Horizon Task Evaluation*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Embodied AI Benchmarks**. These tools provide standardized simulation environments, task suites, and evaluation metrics for training and assessing embodied agents—robots that perceive, reason, and act in physical or simulated worlds.



**Examples** include BEHAVIOR-1K, Habitat-Sim, RLBench, RoboSuite, ManiSkill, ALFRED, VirtualHome, AI2-THOR, ARNOLD, and Colosseum (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, GPU-parallelized simulation, and open task generation—ideal for robotics researchers, embodied AI engineers, and developers seeking transparent, vendor-independent evaluation infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Embodied AI and physics simulation software market is estimated at **$3.2B – $3.9B in 2025–2026**, growing at a CAGR of ~16–18% driven by multimodal Foundation/VLA models and synthetic data demand. The sector displays a hybrid structure: it is **highly concentrated at the core foundational simulator and cloud compute infrastructure tier** (dominated by tech giants like Meta, NVIDIA, and Google), while remaining **moderately to highly fragmented across specialized application domains and robotics hardware form-factors**.

## SaaS/Hosted Platforms

| Platform | Organization / Backer | Organization Size (Revenue / Valuation) | Description | Pricing | Free Tier Limits |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[Habitat Challenge](https://aihabitat.org/challenge/)** | Meta Platforms | ~$1.8T - $2.0T Market Cap (~$160B+ Rev) | Annual challenge and evaluation service evaluating uploaded embodied agents in unseen simulated environments via automated code execution. | $0 / Free (Research Platform) | Free forever; unlimited challenge phase submissions subject to EvalAI rate limit of 3–5 submissions/day per team |
| **[BEHAVIOR Challenge](https://behavior.stanford.edu/)** | Stanford University | $40.8B Endowment ($8.2B+ Op Budget) | Annual benchmark competition grounded in 1,000 human-surveyed daily activities evaluating long-horizon mobile manipulation tasks. | $0 / Free (Academic Benchmark) | Free forever; unrestricted public registration with EvalAI evaluation cap of 2 daily test submissions during challenge periods |
| **[AI2-THOR Cloud](https://ai2thor.allenai.org/)** | Allen Institute for AI (Ai2) | $150M - $205M Annual Inflows / Grants | Cloud-hosted photorealistic indoor simulation platform and benchmark suite for teams training embodied agents without dedicated local GPU clusters. | $0 / Free (501(c)(3) Open Research) | Free forever; open-source access and free cloud Colab/demo runner instances with standard 12h runtime limits |



## Open-Source GitHub Projects



- **[BEHAVIOR-1K](https://behavior.stanford.edu/)**  

  **The first human-centered embodied AI benchmark** with 1,000 realistic household activities. Grounded in surveys of what people actually want robots to do. Features long-horizon mobile manipulation in realistic environments. **The most comprehensive benchmark for human-centric robot assistance** .



- **[Habitat-Sim](https://github.com/facebookresearch/habitat-sim)**  

  **High-performance 3D simulator for embodied AI research** (MIT). Thousands of frames per second—orders of magnitude faster than prior simulators. Features configurable agents, sensor suites (RGB, depth, semantic segmentation, surface normals, optical flow), and scene dataset ingestion API. Supports Habitat 1.0 (navigation), Habitat 2.0 (rearrangement), and Habitat 3.0 (co-habitat with humans and avatars). Installation via Conda, PIP, Docker, or source .



- **[RLBench](https://github.com/stepjam/RLBench)**  

  **100 completely unique, hand-designed manipulation tasks** ranging from simple target reaching and door opening to long multi-stage tasks (e.g., opening an oven and placing a tray in it). Provides proprioceptive and visual observations. **The most widely used benchmark for robot learning from demonstrations** .



- **[RoboSuite](https://robosuite.ai/)**  

  **Modular simulation framework and benchmark for robot learning** powered by MuJoCo. Standardized manipulation tasks, procedural generation of new environments, diverse robot embodiments (including humanoids), composite controllers (joint-space velocity, inverse kinematics, operational space, whole body), teleoperation devices (keyboard, SpaceMouse, DualSense), multi-modal sensors, and photorealistic rendering via NVIDIA Isaac Sim. Part of the ARISE Initiative .



- **[ManiSkill3](https://github.com/haosulab/ManiSkill)**  

  **GPU-parallelized robotics simulation and rendering for generalizable embodied AI**. Collect RGBD + segmentation data at **30,000+ FPS with a 4090 GPU**. Supports heterogeneous simulation (every parallel environment has different scene/objects). Task coverage: table-top, drawing/cleaning, dexterous manipulation across humanoids, mobile manipulators, and single-arm robots. Includes tuned RL (PPO, SAC, TD-MPC2), imitation learning (BC, Diffusion Policy), and VLA (Octo, RDT-1B, RT-x) baselines. RSS 2025 paper .



- **[ALFRED](https://askforalfred.com/)**  

  **Action Learning From Realistic Environments and Directives**—instruction following benchmark built on AI2-THOR. Features 382,065 training samples with action understanding, object recognition, and task planning evaluations. **The standard benchmark for vision-language navigation and interaction** .



- **[VirtualHome](http://virtual-home.org/)**  

  **Multi-agent household activity simulation platform**. Features crowdsourced 2,821 ActivityPrograms spanning 75 atomic actions and 308 objects. Scratch-style interface with 77 block types for program authoring. **The most accessible platform for long-horizon embodied planning research** .



- **[AI2-THOR](https://ai2thor.allenai.org/)**  

  **Near-photorealistic interactive indoor scenes** with rich object properties and affordances. Supports procedural scene generation and embodied manipulation. Foundation for ALFRED, ALFWorld, and many other benchmarks. **The most widely used indoor simulation platform** .



- **[ARNOLD](https://github.com/arnold-benchmark/arnold)**  

  **Benchmark for language-grounded task learning with continuous states in realistic 3D scenes**. Features high-fidelity rendering, continuous object states, and language diversity. Dataset on Zenodo includes trained model checkpoints and benchmark results (3.8 GB). **The most focused benchmark for continuous-state manipulation** .



- **[Colosseum V2](https://github.com/colosseum-benchmark/colosseum)**  

  **Benchmark for vision-language-action model generalization**. Builds on RLBench with **28 tasks across single-arm and bimanual configurations**. Tests robustness to visual and physical perturbations (camera viewpoints, scene geometry, object configurations). Evaluates ACT and π0.5 baselines in **11.5 hours on single RTX 4090**. Validates sim-to-real transfer. **The most focused benchmark for VLA generalization** .



### Additional Strong Open-Source Options



- **[LIBERO](https://github.com/Lifelong-Robot-Learning/LIBERO)** — Lifelong robot learning benchmark with four fixed-base manipulation suites (Spatial, Object, Goal, Long). Ten tasks per suite. LIBERO-Plus adds perturbations to camera, robot state, language, and lighting .

- **[ManiSkill-HAB](https://github.com/haosulang/ManiSkill-HAB)** — Low-level mobile manipulation benchmark with Fetch robot. SetTable (bowl from drawer, apple from refrigerator), TidyHouse, PrepareGroceries. Covers picking, placement, refrigerator/drawer opening .

- Community **n8n** workflows for benchmark evaluation automation and leaderboard tracking.



**Frameworks for building custom systems**: Combine **ManiSkill3** for GPU-parallelized simulation with **Habitat-Sim** for high-fidelity navigation, **RoboSuite** for modular manipulation tasks, **BEHAVIOR-1K** for human-centric long-horizon tasks, and **Colosseum V2** for VLA generalization testing—creating a comprehensive embodied AI evaluation stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Embodied AI benchmarks are research tools. Performance on benchmarks does not guarantee real-world robot success—sim-to-real gap remains a critical challenge.

- **Open-source embodied AI benchmarks are mature and production-grade.** Habitat-Sim, ManiSkill3, RoboSuite, and RLBench are actively maintained and widely adopted in academic and industrial research .

- **Benchmark design matters more than benchmark size.** BEHAVIOR-1K's human-centric grounding (surveys of what people actually want) distinguishes it from arbitrary task collections . Colosseum V2's structured generalization tests (visual and physical perturbations) reveal robustness gaps that in-distribution evaluation misses .

- **Evaluation metrics vary by benchmark.** Success rate is primary, but Goal-Condition Success (GCS) provides finer granularity and Success weighted by Path Length (SPL) rewards efficiency . Choose metrics matching your research questions.

- **Sim-to-real transfer is validated but not guaranteed.** Colosseum V2 demonstrates that "performance trends in simulation reliably reflect real-world generalization behavior" . However, absolute performance may still degrade on physical hardware.

- Self-hosted open-source solutions require proper GPU provisioning (ManiSkill3 achieves 30,000+ FPS on 4090), storage for scene datasets, and ongoing maintenance. Benchmark versions evolve—cite specific versions in publications.



---



**Made for robotics researchers, embodied AI engineers, and developers building transparent evaluation infrastructure.**

Let's make Embodied AI Benchmarks more open, data-driven, and human-centered.

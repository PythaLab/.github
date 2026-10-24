<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/banner-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/banner-light.svg">
    <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/banner-light.svg" alt="PythaLab: research lab at Yildiz Technical University, Istanbul. Learning-based control, UAV systems, mechatronics, rigorous AI research." width="100%">
  </picture>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Yildiz_Technical_University-Istanbul-57318a?style=flat-square" alt="Yildiz Technical University, Istanbul">
  <img src="https://img.shields.io/badge/focus-learning--based_control-d98e04?style=flat-square" alt="Focus: learning-based control">
  <img src="https://img.shields.io/badge/focus-UAV_systems-d98e04?style=flat-square" alt="Focus: UAV systems">
  <img src="https://img.shields.io/badge/focus-rigorous_AI_research-d98e04?style=flat-square" alt="Focus: rigorous AI research">
  <br>
  <img src="https://img.shields.io/badge/Python-3b4a78?style=flat-square" alt="Python">
  <img src="https://img.shields.io/badge/PyTorch-3b4a78?style=flat-square" alt="PyTorch">
  <img src="https://img.shields.io/badge/C%2FC%2B%2B-3b4a78?style=flat-square" alt="C/C++">
  <img src="https://img.shields.io/badge/MATLAB-3b4a78?style=flat-square" alt="MATLAB">
  <img src="https://img.shields.io/badge/arXiv_preprints-9-b31b1b?style=flat-square" alt="9 arXiv preprints">
</p>

**PythaLab** turns theory into algorithms, algorithms into reliable software, software into simulations
and experiments, and findings into academic outputs. Claims are tested before they are believed:
reproducible code, fair baselines, and honest reporting of what works and what does not.

## Research themes

<table>
  <tr>
    <td width="50%" valign="top">
      <b>✈️ Learning-based flight control for UAVs</b><br>
      Reinforcement learning grounded in HJB/Bellman optimal control for fixed-wing and VTOL aircraft,
      with 6-DOF digital twins and validation from simulation through SIL/HIL to flight.
    </td>
    <td width="50%" valign="top">
      <b>🛡️ Safe and nonlinear control</b><br>
      Safety filters that preserve a baseline autopilot, approximate dynamic programming, MPC, and
      adaptive and robust control with Lyapunov (ISS/UUB) analysis.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b>📡 Estimation and embedded systems</b><br>
      Kalman filtering and sensor fusion, real-time control on microcontrollers, mechatronic test rigs
      and actuator systems.
    </td>
    <td width="50%" valign="top">
      <b>🔬 Rigorous evaluation of AI systems</b><br>
      Preregistered, placebo-controlled studies of LLM coding agents and small local models, including
      falsification-based self-repair and risk-controlled claim checking.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <b>🧰 AI research infrastructure</b><br>
      Local-first research workspaces, multi-agent workflows for software and science, and literature
      pipelines that turn papers into searchable, structured knowledge.
    </td>
    <td width="50%" valign="top">
      <b>🧬 Physics-informed generative modelling</b><br>
      Generative models constrained by physics, with applications such as biosignal synthesis for
      prosthetic control.
    </td>
  </tr>
</table>

## Research pipeline

```mermaid
flowchart TD
    T["Theory<br/>HJB/Bellman, Lyapunov"] --> A["Algorithm"]
    A --> S["Research software<br/>tested, reproducible"]
    S --> D["Simulation and digital twin"]
    D --> H["SIL / HIL"]
    H --> F["Flight and lab experiments"]
    F --> P["Publication and open code"]
    F -.->|"feedback"| T

    classDef step fill:none,stroke:#888,stroke-width:1.5px
    class T,A,S,D,H,F,P step
```

## Preprints

Preprints on arXiv; see each listing for status.

**UAV control**

| Title | Year |
| --- | --- |
| [Autopilot-Preserving Residual Q-Learning with HJB-Inspired Finite-Action Risk Filtering for Fixed-Wing UAV Command Supervision](https://arxiv.org/abs/2606.01397) | 2026, with B. Temiz |

**AI systems: rigorous evaluation and engineering use**

| Title | Year |
| --- | --- |
| [Requirement-Bound Verified Commissioning: A Frozen Four-Billion-Parameter Local Model as a Candidate Generator under an External Acceptance Layer with Verification and Release Authority](https://arxiv.org/abs/2609.30219) | 2026 |
| [Form, Not Content? A Preregistered, Placebo-Controlled Evaluation of Learned Error-Conditioned Self-Repair Through Prompts and Weights in Frozen Small Code Models](https://arxiv.org/abs/2607.12962) | 2026 |
| [Falsification, Not Exposure: An Internally Preregistered Placebo-Controlled Decomposition of Self-Repair Feedback in Frozen Small Code Models](https://arxiv.org/abs/2606.31511) | 2026 |
| [Selection Without Signal, Recovery Through Expression: A Measurement Study of Post-Hoc Falsification Operators for Frozen Small Code Models](https://arxiv.org/abs/2606.16999) | 2026 |
| [Scaffold, Not Vocabulary? A Controlled, Two-Tier, Pre-Registered Study of a Popperian Code-Generation Skill](https://arxiv.org/abs/2606.06454) | 2026 |
| [PYTHALAB-MERA: Validation-Grounded Memory, Retrieval, and Acceptance Control for Frozen-LLM Coding Agents](https://arxiv.org/abs/2605.08468) | 2026 |
| [Feedback-Normalized Developer Memory for Reinforcement-Learning Coding Agents: A Safety-Gated MCP Architecture](https://arxiv.org/abs/2605.01567) | 2026 |
| [Learning When to Remember: Risk-Sensitive Contextual Bandits for Abstention-Aware Memory Retrieval in LLM-Based Coding Agents](https://arxiv.org/abs/2604.27283) | 2026 |

## Research showcase

<table>
  <tr>
    <td colspan="2" align="center">
      <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/showcase/uav-architecture.png" alt="Block diagram of autopilot-preserving residual command supervision: mission reference, residual command supervisor, command projection, classical autopilot and fixed-wing UAV plant, with the internal decision logic (feature extraction, finite candidate residuals, Q/HJB critic, Hamiltonian advantage, CLF/CBF-style safety filter, select or fallback)" width="100%"><br>
      <sub>Autopilot-preserving residual command supervision: a learned supervisor above an unchanged classical autopilot, with a value-guided critic and a safety filter (<a href="https://arxiv.org/abs/2606.01397">arXiv:2606.01397</a>)</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top" align="center">
      <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/showcase/uav-crosswind-timeseries.png" alt="Time series of a representative low-altitude crosswind and turbulence orbit: baseline, Q residual and HJB residual controllers" width="100%"><br>
      <sub>Representative low-altitude crosswind/turbulence orbit, baseline versus residual controllers (<a href="https://arxiv.org/abs/2606.01397">arXiv:2606.01397</a>)</sub>
    </td>
    <td width="50%" valign="top" align="center">
      <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/showcase/uav-rms-benchmark.png" alt="Bar chart of full-duration RMS spatial reference and path tracking error for baseline, Q residual and HJB residual" width="100%"><br>
      <sub>Mean RMS path error over a 20-scenario simulation benchmark (<a href="https://arxiv.org/abs/2606.01397">arXiv:2606.01397</a>)</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top" align="center">
      <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/showcase/mera-benchmark.png" alt="Phase 1c hard RL benchmark: strict validation success, mean repair attempts and mean wall-clock duration for three methods" width="100%"><br>
      <sub>Strict-validation success on a 3-task RL coding benchmark, 3 repetitions (<a href="https://arxiv.org/abs/2605.08468">arXiv:2605.08468</a>)</sub>
    </td>
    <td width="50%" valign="top" align="center">
      <img src="https://raw.githubusercontent.com/PythaLab/.github/main/profile/assets/showcase/teaching-rl-lab.gif" alt="Screen recording of a browser-based reinforcement learning laboratory: overview page, k-armed bandit module and finite MDP editor" width="100%"><br>
      <sub>Browser-based RL laboratory used in teaching</sub>
    </td>
  </tr>
</table>

## Teaching

Courses in Python programming, artificial intelligence, a reinforcement learning control laboratory,
applied nonlinear control and capstone design, at undergraduate and graduate level; a graduate course
on large language models is in preparation. Browser-based interactive laboratories let students run
simulations and train policies without installing anything.

## Students

The lab supervises MSc research and is launching an undergraduate research programme. Each student works in a private,
supervised repository with a common structure; progress is tracked through weekly reports,
assignments with evidence-based solutions, and written reviews.

## Open work

Selected public repositories on the supervisor's account, [PhiniteLab](https://github.com/PhiniteLab):

| Area | Repositories |
| --- | --- |
| Safe control | [residual-shield](https://github.com/PhiniteLab/residual-shield) · [ReinforcementLearningControl](https://github.com/PhiniteLab/ReinforcementLearningControl) · [IntelligentNonlinearControl](https://github.com/PhiniteLab/IntelligentNonlinearControl) |
| Embedded control and estimation | [control-library-for-embedded-systems](https://github.com/PhiniteLab/control-library-for-embedded-systems) · [fast-kalman-filter](https://github.com/PhiniteLab/fast-kalman-filter) · [system-dynamic-library](https://github.com/PhiniteLab/system-dynamic-library) |
| Neural network toolboxes | Levenberg–Marquardt training in [C](https://github.com/PhiniteLab/levenberg-marquardt-nn-C-toolbox) · [C++](https://github.com/PhiniteLab/levenberg-marquardt-nn-Cpp-toolbox) · [MATLAB](https://github.com/PhiniteLab/levenberg-marquardt-nn-matlab-toolbox) |
| AI research tooling | [scaffold-skill](https://github.com/PhiniteLab/scaffold-skill) · [rl-developer-memory](https://github.com/PhiniteLab/rl-developer-memory) · [cortexmark](https://github.com/PhiniteLab/cortexmark) |

## Supervisor

Asst. Prof. Dr. Mehmet İşcan — [github.com/PhiniteLab](https://github.com/PhiniteLab) ·
phinitelab@gmail.com

---

<p align="center">
  <sub>Toolchain: Python, PyTorch, C/C++, MATLAB, FastAPI, React, SQLite, Ollama, uv · Student repositories are private.</sub>
</p>

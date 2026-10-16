---
hide_table_of_contents: false
pagination_prev: null
pagination_next: null
---

# Research Program

## A theory of identification and generation in stochastic differential equations

---

## Overview

From data observed as trajectories or snapshots, we **identify** the generator (drift or potential) that drives a stochastic process — the inverse problem. From the identified stochastic differential equation (SDE), we **generate** target distributions — the forward problem. This program aims to develop the theories of both on a common mathematical foundation.

---

## Background

The **inverse problem** for stochastic processes (identification of the generator: inverse stochastic control and drift estimation) and the **forward problem** (error analysis of generative models) have developed in separate research communities. Yet their mathematical core is the same: both operate in the common language of **Schrödinger bridges, h-path processes, Doob transforms, and forward–backward stochastic differential equations (FBSDEs)**.

Working in this common language, our group has obtained results on both the inverse side (inverse stochastic control) and the forward side (convergence analysis of diffusion generative models). The program develops the two around a single object: the identified SDE.

---

## Three topics

1. **Transport** — Establish the relationship between inverse stochastic control and (stochastic) optimal transport and the Schrödinger problem as a general framework that contains the classical cases as special instances.
2. **Generation** — Establish an error analysis of sampling (diffusion-model-type generation) that uses the identified SDE as the forward process, extending DDPM-type convergence theory to general drifts.
3. **Coupling** — Establish an **error-propagation principle from identification to generation**, in which the output of identification quantitatively governs the error guarantees of generation. This is the central topic of the program.

The methodological core is to formulate constraints on distributions as **distances in a reproducing kernel Hilbert space (RKHS)** and to solve them from samples via **unbiased estimators**. A distinguishing feature of the program is that its methods come with **finite-sample guarantees and convergence rates** (well-posedness, suboptimality-gap bounds, almost-sure convergence) that deep-learning approaches lack. As a validation of the theory, we identify Langevin equations from public ecological data (animal movement trajectories) and test the whole pipeline from identification to generation.

---

## Selected results

**Identification (inverse problem)**

- Well-posedness and numerical methods for inverse stochastic optimal control — [Automatica 149 (2023), 110831](https://doi.org/10.1016/j.automatica.2022.110831)
- Inverse stochastic control via generalized Schrödinger problems — [Systems & Control Letters 218 (2026), 106614](https://doi.org/10.1016/j.sysconle.2026.106614)
- Drift-potential identification free of time-step bias — [arXiv:2610.04268](https://arxiv.org/abs/2610.04268) [[code](https://github.com/yumiharu-nakano/inverse-drift-potential)]

**Transport**

- A kernel-based method for Schrödinger bridges — Jpn. J. Ind. Appl. Math. 43 (2026), 46 [[arXiv:2310.14522](https://arxiv.org/abs/2310.14522)] [[code](https://github.com/yumiharu-nakano/kernelSB)]
- Multi-marginal optimal transport via Hilbert space embeddings — Statist. Comput. 36 (2026), 118 [[arXiv:2412.03478](https://arxiv.org/abs/2412.03478)] [[code](https://github.com/yumiharu-nakano/kernelMMOT)]
- Continuum-marginal optimal transport: a mesh-free kernel method — [arXiv:2604.24226](https://arxiv.org/abs/2604.24226) [[code](https://github.com/yumiharu-nakano/alltimeOT)]

**Generation (forward problem)**

- Structural and convergence analysis of discrete-time DDPMs — [arXiv:2406.01320](https://arxiv.org/abs/2406.01320)
- Kernel-based potential mean-field games with unbiased random Fourier U-statistics — [arXiv:2605.29371](https://arxiv.org/abs/2605.29371) [[code](https://github.com/yumiharu-nakano/kernelMFG-RFU)]

**Foundations (numerical analysis)**

- Convergence of meshfree collocation methods for fully nonlinear parabolic equations — Numer. Math. 136 (2017), 703–723
- Convergence of kernel and neural-network methods for HJB equations on unbounded domains — [arXiv:2610.09299](https://arxiv.org/abs/2610.09299) [[code](https://github.com/yumiharu-nakano/hjb-residual-methods)]

See the [top page](/) for the full list of publications.

---

## Research tree

The research tree visualizes the overall course of the research and how each area converges into the integrated program.

👉 [**View the research tree**](https://yumiharu-nakano.github.io/nakano-lab/tree-en.html)

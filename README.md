# DecAEvolve

**Decompose, Adapt, and Evolve, or, Three Pillars of Effective LLM-based Scientific Equation Discovery**

Pouya Behzadifar\*, Parshin Shojaee\*, Sanchit Kabra\*, Kazem Meidani, Chandan K. Reddy
*<sup>\*</sup>Equal contribution.*

Sharif University of Technology · Virginia Tech · Capital One · Carnegie Mellon University

📍 **ICML 2026 — Seoul, South Korea**

[Paper](static/pdfs/decaevolve.pdf) · [arXiv](https://arxiv.org/abs/0000.00000) · [Project Page](https://radical-p.github.io/DecAEvolve/) · [Code](https://github.com/decaevolve/decaevolve)

---

## Abstract

Discovering compact mathematical expressions that approximate an unknown target function from observed data is a foundational problem in physics, biology, and materials science. Recent LLM-based symbolic regression methods leverage scientific priors to navigate the combinatorial hypothesis space, but they share two limitations: the LLM is treated as a *static* hypothesis generator whose weights never see the target system, and the only feedback returned to it is a *scalar* reward that hides which symbolic components actually drove a hit or a miss.

**DecAEvolve** reframes equation discovery as a closed-loop process built on three coupled mechanisms:

- **Decompose** — parse each generated program into an abstract syntax tree, isolate atomic symbolic terms, and quantify single-term and pairwise contributions via re-optimized ablations.
- **Adapt** — distill the observed system into the policy at test time using Group-Relative Policy Optimization (GRPO) with LoRA adapters and a KL anchor to a frozen reference model.
- **Evolve** — thread decomposition annotations back into a multi-island experience buffer, so subsequent prompts carry not just successful hypotheses but the structural reasons they succeeded.

On four scientific benchmarks (two nonlinear oscillators, *E. coli* growth, aluminum stress–strain) and six open-source backbones (1.5B–8B), DecAEvolve reduces OOD normalized MSE by up to two orders of magnitude over LLM-SR and classical/neural symbolic regression baselines.

## Citation

```bibtex
@inproceedings{behzadifar2026decaevolve,
  title     = {DecAEvolve: Decompose, Adapt, and Evolve, or, Three Pillars
               of Effective LLM-based Scientific Equation Discovery},
  author    = {Behzadifar, Pouya and Shojaee, Parshin and Kabra, Sanchit
               and Meidani, Kazem and Reddy, Chandan K.},
  booktitle = {Proceedings of the 43rd International Conference on Machine Learning},
  address   = {Seoul, South Korea},
  publisher = {PMLR},
  volume    = {306},
  year      = {2026}
}
```

## License

Paper © 2026 the authors. Released under the conference's standard license.

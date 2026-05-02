# DecAEvolve Project Page

This repository hosts the project page for:

**DecAEvolve: Decompose, Adapt, and Evolve, or, Three Pillars of Effective LLM-based Scientific Equation Discovery**

Accepted to **ICML 2026**.

Authors: Pouya Behzadifar*, Parshin Shojaee*, Sanchit Kabra*, Kazem Meidani, and Chandan K Reddy.

`*` Equal contribution.

Project page: https://radical-p.github.io/DecAEvolve/

Paper PDF: [`static/pdfs/decaevolve.pdf`](static/pdfs/decaevolve.pdf)

## Overview

DecAEvolve is a framework for LLM-based scientific equation discovery. It combines:

- **Decompose:** parse candidate equations into symbolic terms and estimate which terms contribute to accuracy.
- **Adapt:** fine-tune the LLM at test time with GRPO using data-driven rewards.
- **Evolve:** maintain an evolving population of high-scoring, annotated equation programs that guide future search.

The project page is a static HTML/CSS site adapted from the Academic Project Page Template and deployed with GitHub Pages.

## BibTeX

```bibtex
@inproceedings{behzadifar2026decaevolve,
  title={DecAEvolve: Decompose, Adapt, and Evolve, or, Three Pillars of Effective LLM-based Scientific Equation Discovery},
  author={Behzadifar, Pouya and Shojaee, Parshin and Kabra, Sanchit and Meidani, Kazem and Reddy, Chandan K},
  booktitle={Proceedings of the 43rd International Conference on Machine Learning},
  address={Seoul, South Korea},
  publisher={PMLR},
  volume={306},
  year={2026}
}
```

# EMSC2010 – Week 7 Lectorial 1: Bayesian Inference

This repository contains the template Jupyter notebooks for **Week 7 Lectorial 1** of *EMSC2010: Data Science for Earth System Scientists* at the Australian National University.

The session introduces **Bayesian inference** — how to update beliefs about uncertain quantities in light of data — progressing from foundational probability concepts through to probabilistic programming with PyMC.

---

## Notebooks

### Notebook 1 – Normal Distributions and Probability (`NB1`)

**Scenario:** You find a lost penguin in a dark Antarctic snowstorm. You can measure its height (71 cm) but cannot identify the species. Should you direct it towards the Emperor colony or the Adélie colony?

Using known population statistics for each species (mean and standard deviation of height), this notebook demonstrates how to use the normal distribution to calculate probabilities and make principled decisions under uncertainty.

**Key concepts:** Normal (Gaussian) distributions, probability density functions, `scipy.stats.norm`

**Libraries:** `numpy`, `matplotlib`, `scipy`

---

### Notebook 2 – Bayesian Inference and the Posterior Distribution (`NB2`)

**Scenario:** Probes are launched at random locations above a planet's surface. Some land in ocean, some on land. What proportion of the surface is covered by ocean?

This notebook applies **Bayes' theorem** with a Beta-Binomial conjugate model to calculate a posterior distribution for the ocean fraction. It also explores the effect of different priors — starting from a uniform (non-informative) prior and then encoding domain knowledge via an informed Beta prior.

**Key concepts:** Bayes' theorem, prior and posterior distributions, Beta-Binomial conjugacy, credible intervals

**Libraries:** `numpy`, `matplotlib`, `scipy`

---

### Notebook 3 – Probabilistic Programming with PyMC (`NB3`)

Using student height data collected in Week 5, this notebook estimates the posterior distribution of the population mean height in two ways:

1. **Analytically** — deriving the posterior as a *t*-distribution using non-informative (Jeffreys) priors for μ and σ.
2. **Via probabilistic programming** — using **PyMC** and Markov chain Monte Carlo (MCMC) sampling to approximate the same posterior numerically, then extending to an informative prior.

The notebook demonstrates that the two approaches agree, and highlights how probabilistic programming makes it straightforward to incorporate prior knowledge and tackle problems where an analytical posterior is intractable.

**Key concepts:** Analytical posteriors, Markov chain Monte Carlo, probabilistic programming, informative vs non-informative priors, posterior predictive checks

**Libraries:** `numpy`, `matplotlib`, `scipy`, `pymc`, `arviz`

---

## Getting Started

This is a **template repository**. To begin working on the notebooks:

1. Click **"Use this template"** at the top of this page to create a copy of the repository in your own GitHub account.
2. Open any notebook from your copy of the repository and click the **"Open in Colab"** badge at the top of the notebook to launch it in Google Colab.
3. Before submitting, replace the `uXXXXXXX` placeholder in the filename with your ANU student UID.

---

## Repository Structure

```
EMSC2010-W7-L1/
├── EMSC2010_W7_L1_NB1_uXXXXXXX.ipynb   # Normal distributions & probability
├── EMSC2010_W7_L1_NB2_uXXXXXXX.ipynb   # Bayesian inference with Beta-Binomial model
├── EMSC2010_W7_L1_NB3_uXXXXXXX.ipynb   # Probabilistic programming with PyMC
├── LICENSE
└── README.md
```

---

## Course Information

| | |
|---|---|
| **Course** | EMSC2010 – Data Science for Earth System Scientists |
| **Institution** | Australian National University (ANU) |
| **Week** | 7 |
| **Session** | Lectorial 1 |
| **Topic** | Bayesian Inference |

---

## License

This repository is released under the [MIT License](LICENSE).

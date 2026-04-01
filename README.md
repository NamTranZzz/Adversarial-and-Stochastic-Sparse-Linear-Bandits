# Adversarial and Stochastic Sparse Linear Bandits

Code for experiments related to the paper **“Sparse Linear Bandits with Fixed Sparsity Support: Adversarial and Stochastic Regimes”** by Kyoungseok Jang, Nam Phuong Tran, and Nicolò Cesa-Bianchi.

This repository contains notebook-based implementations for sparse linear bandit experiments in both the **adversarial** and **stochastic** settings, with a focus on the case where the unknown parameter/loss vector has a **fixed sparse support**.

## Overview

Sparse linear bandits are a high-dimensional bandit setting where only a small number of coordinates are relevant. This project studies both:

- **Adversarial sparse linear bandits**
- **Stochastic sparse linear bandits**

under a **fixed sparsity support** assumption.

The associated paper shows that this assumption can be used to break the usual dependence on the ambient dimension in several settings, including adversarial bandits over the \( \ell_\infty \) and \( \ell_2 \) action sets, and stochastic bandits over \( \ell_p \)-ball action sets.

## Repository structure

The repository currently consists of three Jupyter notebooks:

- `Spase adv hypercube.ipynb`  
  Experiments for the adversarial setting on the **hypercube / \( \ell_\infty \)-ball** action set.

- `sparse adv bandit l2.ipynb`  
  Experiments for the adversarial setting on the **\( \ell_2 \)-ball** action set.

- `lp Stochastic Bandit.ipynb`  
  Experiments for the **stochastic sparse linear bandit** setting over **\( \ell_p \)-ball** action sets.

## What is implemented

From the notebook code, the repository includes components such as:

- sparse environment / loss generation
- support-aware or support-identification-based experimental routines
- adversarial bandit algorithms for specific geometries
- stochastic linear bandit experiments for \( \ell_p \)-ball action sets
- regret computation and plotting utilities

For example, the hypercube notebook includes:
- sparse loss generation,
- OSMD-style routines for adversarial bandits,
- cumulative regret computation against the best fixed action in hindsight.

## Requirements

The notebooks use standard scientific Python packages:

- `numpy`
- `matplotlib`
- `math` (standard library)

A recent Python 3 version is recommended.

## Installation

Clone the repository and install the basic dependencies:

```bash
git clone https://github.com/NamTranZzz/Adversarial-and-Stochastic-Sparse-Linear-Bandits.git
cd Adversarial-and-Stochastic-Sparse-Linear-Bandits
pip install numpy matplotlib jupyter

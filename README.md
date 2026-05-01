# Multivector Morphological Networks

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.x](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)

This repository contains the official Python implementation of the Lattice Isomorphism Theorem and hardware synthesis methodologies presented in the IEEE manuscript:

**"Multivector Morphological Networks: A Clifford Algebraic Taxonomy for Non-Reciprocal Circuit Synthesis"** *Authors: Adnan H. Abdulwahid and Faycal Znidi (Texas A&M University–Texarkana)*

## Overview

Traditional morphological image processing operates purely in the digital domain. This codebase bridges the gap between abstract spatial-chromatic topology and physical analog hardware. 

By elevating multi-channel (RGB) images to the 3D Clifford algebra ($Cl_{3,0}$), this script demonstrates how to map spatial image gradients to continuous-time electrical lattices natively. It applies the discrete spatial Dirac operator ($\nabla$) to extract:
1. **Scalar Divergence:** Representing isotropic dissipation (luminance), which physically maps to resistive shunt passivity.
2. **Bivector Curl:** Representing chromatic edge transitions, which physically necessitates non-reciprocal couplings (gyrators).

The script outputs the theoretical **Nodal Admittance Matrix** ($\mathbf{Y}$) required to synthesize a hardware network capable of zero-latency morphological filtering.

## Repository Contents

* `clifford_synthesis.py`: The core synthesis engine. Contains the `CliffordLattice` class, the discrete Dirac operator application, and the $\mathbf{Y}$ matrix generation logic.
* `LICENSE`: The open-source MIT License governing this code.

## Prerequisites

This codebase is designed to be lightweight and highly accessible. It requires only standard Python and NumPy.

* Python 3.7+
* NumPy

You can install the required dependency via pip:
```bash
pip install numpy

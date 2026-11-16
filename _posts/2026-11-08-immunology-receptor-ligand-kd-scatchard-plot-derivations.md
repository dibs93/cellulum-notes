---
layout: post
title: "Receptor-Ligand Binding Kinetics, Dissociation Constant (Kd) & Scatchard Plots"
description: "Mathematical derivations of antibody-antigen affinity, receptor fractional occupancy, and Scatchard plot graphical interpretation for CSIR NET Unit 4."
date: 2026-11-08
categories: [Cell Signaling, Immunology]
---

Quantitative analysis of receptor-ligand interactions and antibody-antigen binding (Unit 4: Cell Communication and Cell Signaling) is a recurring theme in CSIR NET Part C. Questions frequently test the relationship between association/dissociation rate constants ($k_{\text{on}}$ and $k_{\text{off}}$), fractional receptor occupancy ($\theta$), and linear Scatchard plots.

## 1. Equilibrium Dissociation Constant ($K_d$) & Affinity

Consider a reversible, bimolecular interaction between a free receptor (or monovalent antibody binding site) $R$ and a free ligand (or hapten) $L$ to form a receptor-ligand complex $RL$:

$$R + L \underset{k_{\text{off}}}{\overset{k_{\text{on}}}{\rightleftharpoons}} RL$$

At equilibrium, the rate of association equals the rate of dissociation:

$$k_{\text{on}}[R][L] = k_{\text{off}}[RL]$$

The **Equilibrium Dissociation Constant ($K_d$)** and **Association (Affinity) Constant ($K_a$)** are defined as:

$$K_d = \frac{1}{K_a} = \frac{k_{\text{off}}}{k_{\text{on}}} = \frac{[R][L]}{[RL]} \quad (\text{Units of } K_d: \text{M})$$

* **Lower $K_d$ = Higher Binding Affinity:** A monoclonal antibody with $K_d = 10^{-10} \, \text{M}$ ($0.1 \, \text{nM}$) binds its epitope with $1,000$-fold higher affinity than an antibody with $K_d = 10^{-7} \, \text{M}$ ($100 \, \text{nM}$).
* **Physical Meaning of $K_d$:** When the concentration of free ligand equals $K_d$ ($[L] = K_d$), then $[R] = [RL]$, meaning **exactly $50\%$ of total receptors are occupied**.

## 2. Fractional Receptor Occupancy ($\theta$)

Let total receptor concentration be $[R]_T = [R] + [RL]$. The fraction of total receptors bound to ligand ($\theta$) is given by the hyperbolic Langmuir binding isotherm:

$$\theta = \frac{[RL]}{[R]_T} = \frac{[RL]}{[R] + [RL]} = \frac{[L]}{K_d + [L]}$$

* When $[L] = 0.1 \, K_d \implies \theta = \frac{0.1}{1.1} \approx 9.1\%$ occupied.
* When $[L] = K_d \implies \theta = \frac{1}{2} = 50\%$ occupied.
* When $[L] = 9 \, K_d \implies \theta = \frac{9}{10} = 90\%$ occupied.

## 3. The Scatchard Equation & Plot Interpretation

To determine both binding affinity ($K_d$) and the total number of receptor binding sites ($B_{\max}$ or $n$) from experimental equilibrium dialysis or radioligand binding data, let $[B] = [RL]$ represent **Bound ligand** and $[F] = [L]$ represent **Free ligand**. Substituting $[R] = B_{\max} - [B]$ into the $K_d$ expression gives the linear **Scatchard equation**:

$$\frac{\text{Bound}}{\text{Free}} = \frac{[B]}{[F]} = -\frac{1}{K_d}[B] + \frac{B_{\max}}{K_d}$$

When plotting **$\frac{[B]}{[F]}$ on the Y-axis** against **$[B]$ on the X-axis**:
* **Slope of the line:** $-\frac{1}{K_d}$ (or $-K_a$). A **steeper negative slope** indicates a smaller $K_d$ and therefore **higher binding affinity**.
* **X-intercept (where $\frac{[B]}{[F]} = 0$):** Equals **$B_{\max}$** (total receptor concentration or valency $n$ per molecule, such as $n = 2$ for intact $\text{IgG}$ and $n = 10$ for pentameric $\text{IgM}$).
* **Y-intercept:** $\frac{B_{\max}}{K_d}$.
* **Curved (Non-Linear) Scatchard Plots:** A concave-downward curve indicates positive cooperativity, whereas a concave-upward curve indicates either negative cooperativity or two distinct populations of high- and low-affinity receptors.

## 4. Worked CSIR NET Part C Numerical Problem

**Problem:** Surface plasmon resonance (SPR) analysis of two engineered scFv antibody fragments ($X$ and $Y$) binding to a viral spike antigen yielded the following kinetic parameters:
* **Fragment X:** $k_{\text{on}} = 2 \times 10^5 \, \text{M}^{-1}\text{s}^{-1}$ and $k_{\text{off}} = 4 \times 10^{-4} \, \text{s}^{-1}$
* **Fragment Y:** $k_{\text{on}} = 5 \times 10^5 \, \text{M}^{-1}\text{s}^{-1}$ and $k_{\text{off}} = 1 \times 10^{-2} \, \text{s}^{-1}$

1. Calculate $K_d$ (in $\text{nM}$) for both fragments and identify which fragment has higher affinity.
2. What concentration of free viral antigen is required to occupy $80\%$ of Fragment X binding sites?

**Solution:**
1. **Calculate $K_d$ for Fragment X and Fragment Y:**
   $$K_{d\text{ (X)}} = \frac{k_{\text{off}}}{k_{\text{on}}} = \frac{4 \times 10^{-4} \, \text{s}^{-1}}{2 \times 10^5 \, \text{M}^{-1}\text{s}^{-1}} = 2 \times 10^{-9} \, \text{M} = 2.0 \, \text{nM}$$
   $$K_{d\text{ (Y)}} = \frac{k_{\text{off}}}{k_{\text{on}}} = \frac{1 \times 10^{-2} \, \text{s}^{-1}}{5 \times 10^5 \, \text{M}^{-1}\text{s}^{-1}} = 2 \times 10^{-8} \, \text{M} = 20.0 \, \text{nM}$$
   Because $K_{d\text{ (X)}} (2 \, \text{nM}) < K_{d\text{ (Y)}} (20 \, \text{nM})$, **Fragment X has $10$-fold higher affinity** (driven by its $25$-fold slower off-rate).
2. **Calculate Free Ligand $[L]$ for $\theta = 0.80$ ($80\%$ occupancy) on Fragment X:**
   $$0.80 = \frac{[L]}{2.0 \, \text{nM} + [L]} \implies 1.6 \, \text{nM} + 0.80[L] = [L] \implies 0.20[L] = 1.6 \, \text{nM} \implies [L] = 8.0 \, \text{nM}$$

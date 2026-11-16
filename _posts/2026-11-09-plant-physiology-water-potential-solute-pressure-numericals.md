---
layout: post
title: "Plant Physiology: Water Potential, Osmotic Potential & Turgor Pressure Numericals"
description: "Complete guide to plant water relations, van 't Hoff solute potential calculations, plasmolysis, and cell-to-cell water movement for CSIR NET Unit 6."
date: 2026-11-09
categories: [Plant Physiology, Biophysics]
---

Water transport across plant cell membranes and vascular tissues (Unit 6: System Physiology – Plant) is governed by thermodynamic **water potential ($\Psi_w$)** gradients. CSIR NET Part C questions frequently ask you to compute osmotic potential using the van 't Hoff equation, predict the direction of water flow between adjacent mesophyll cells, and determine turgor loss points.

## 1. Components of Plant Water Potential ($\Psi_w$)

Water potential quantifies the chemical potential of water per unit partial molar volume, expressed in pressure units (**megapascals, $\text{MPa}$**, where $1 \, \text{MPa} = 10 \, \text{bar} \approx 9.87 \, \text{atm}$). By convention, **pure free water at atmospheric pressure has $\Psi_w = 0 \, \text{MPa}$**.

For a typical non-woody plant cell, total water potential is the sum of solute (osmotic), pressure (turgor), and gravitational potentials:

$$\Psi_w = \Psi_s + \Psi_p + \Psi_g$$

At the cellular scale, gravitational potential ($\Psi_g$) is negligible unless analyzing tall trees ($> 10 \, \text{m}$, where $\Psi_g$ increases by $+0.01 \, \text{MPa}$ per meter of height), simplifying the equation to:

$$\Psi_w = \Psi_s + \Psi_p$$

* **Solute (Osmotic) Potential ($\Psi_s$):** Always **$0$ or negative ($\le 0 \, \text{MPa}$)**. Dissolved solutes reduce the free energy (mole fraction) of water.
* **Pressure Potential ($\Psi_p$):** Positive in turgid living cells ($\Psi_p > 0$), zero in incipiently plasmolyzed/flaccid cells ($\Psi_p = 0$), and **negative ($\Psi_p < 0$)** inside transpiring xylem tracheary elements under tension.

### Fundamental Rule of Water Movement:
Water **always** moves passively by osmosis from a region of **higher (less negative) $\Psi_w$** to a region of **lower (more negative) $\Psi_w$**, regardless of individual $\Psi_s$ or $\Psi_p$ values.

## 2. Calculating Solute Potential ($\Psi_s$) via the van 't Hoff Equation

For dilute ideal solutions, solute potential ($\Psi_s$) is directly proportional to molarity ($C$) and absolute temperature ($T$):

$$\Psi_s = -i C R T$$

Where:
* $i$ is the **van 't Hoff ionization factor** ($i = 1$ for non-electrolytes like sucrose, glucose, or mannitol; $i \approx 2$ for $\text{NaCl}$; $i \approx 3$ for $\text{CaCl}_2$).
* $C$ is the solute concentration in $\text{mol}\cdot\text{L}^{-1}$ ($\text{M}$) or $\text{mol}\cdot\text{m}^{-3}$.
* $R = 0.008314 \, \text{L}\cdot\text{MPa}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$ (or $8.314 \times 10^{-6} \, \text{m}^3\cdot\text{MPa}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$).
* $T$ is absolute temperature in Kelvin ($\text{K} = ^\circ\text{C} + 273.15$).

**Exam Shortcut at $25^\circ\text{C}$ ($298 \, \text{K}$):**
At $25^\circ\text{C}$, the product $RT = 0.008314 \times 298 = \mathbf{2.478 \, \text{L}\cdot\text{MPa}\cdot\text{mol}^{-1}}$. Thus, a $1.0 \, \text{M}$ sucrose solution at $25^\circ\text{C}$ has $\Psi_s = -2.48 \, \text{MPa}$ (and a $0.1 \, \text{M}$ sucrose solution has $\Psi_s \approx -0.248 \, \text{MPa}$).

## 3. Cellular Physiological States in External Solutions

| Physiological State | Condition | Pressure Potential ($\Psi_p$) | Total Water Potential ($\Psi_w$) |
| :--- | :--- | :--- | :--- |
| **Fully Turgid Cell** (in pure water) | $\Psi_{w\text{ (cell)}} = \Psi_{w\text{ (water)}} = 0$ | $\Psi_p = -\Psi_s$ (Maximum turgor) | $\Psi_w = 0 \, \text{MPa}$ |
| **Flaccid / Incipient Plasmolysis** | Protoplast just detaches from cell wall | $\Psi_p = 0 \, \text{MPa}$ | $\Psi_w = \Psi_s$ |
| **Transpiring Xylem Conduit** | Open apoplastic tube under cohesion-tension | $\Psi_p < 0$ (Negative hydrostatic tension) | $\Psi_w \approx \Psi_p$ (since xylem $\Psi_s \approx 0$) |

*(Note: In a rigid plant cell wall with high volumetric elastic modulus $\varepsilon$, small changes in cell volume produce large changes in turgor pressure $\Psi_p$.)*

## 4. Worked CSIR NET Part C Numerical Problems

**Problem 1 (Equilibrium Turgor in Sucrose Solution):** A plant cell with an internal solute concentration equivalent to $0.3 \, \text{M}$ sucrose and an initial turgor pressure of $+0.2 \, \text{MPa}$ is immersed in an open beaker containing a $0.15 \, \text{M}$ sucrose solution at $25^\circ\text{C}$ ($RT = 2.48 \, \text{L}\cdot\text{MPa}\cdot\text{mol}^{-1}$). Assuming cell volume changes are negligible, calculate:
1. Initial $\Psi_w$ of the cell and the external solution.
2. Direction of water movement.
3. Final turgor pressure ($\Psi_p$) of the cell at equilibrium.

**Solution:**
1. **Calculate initial potentials:**
   * $\Psi_{s\text{ (cell)}} = -1 \times 0.3 \times 2.48 = -0.744 \, \text{MPa}$.
   * $\Psi_{w\text{ (cell, initial)}} = \Psi_s + \Psi_p = -0.744 + 0.200 = -0.544 \, \text{MPa}$.
   * External beaker is open to the atmosphere ($\Psi_{p\text{ (ext)}} = 0$):
     $$\Psi_{w\text{ (ext)}} = \Psi_{s\text{ (ext)}} = -1 \times 0.15 \times 2.48 = -0.372 \, \text{MPa}$$
2. **Direction of Water Flow:** Since $\Psi_{w\text{ (ext)}} (-0.372 \, \text{MPa})$ is higher (less negative) than $\Psi_{w\text{ (cell)}} (-0.544 \, \text{MPa})$, **water enters the cell**.
3. **Final Equilibrium Turgor Pressure ($\Psi_p$):** At equilibrium, $\Psi_{w\text{ (cell, final)}} = \Psi_{w\text{ (ext)}} = -0.372 \, \text{MPa}$:
   $$\Psi_{p\text{ (final)}} = \Psi_{w\text{ (cell, final)}} - \Psi_{s\text{ (cell)}} = -0.372 - (-0.744) = +0.372 \, \text{MPa}$$

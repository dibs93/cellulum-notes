---
layout: post
title: "Membrane Bioenergetics: Nernst Equilibrium Potential & Proton Motive Force"
description: "Complete derivations and CSIR NET Part C solved numericals on Nernst ion equilibrium potentials, Goldman-Hodgkin-Katz voltage, and mitochondrial proton motive force."
date: 2026-11-07
categories: [Cell Biology, Animal Physiology]
---

Quantitative questions on electrochemical ion gradients appear across Unit 2 (Cellular Organization – Membrane Transport) and Unit 7 (Animal Physiology – Excitable Membranes) in CSIR NET Life Sciences. Understanding the Nernst equation and Mitchell's chemiosmotic Proton Motive Force ($\Delta p$) allows you to solve both neurobiology action-potential problems and mitochondrial ATP synthase stoichiometry numericals.

## 1. The Nernst Equation for Ion Equilibrium Potential ($E_X$)

When a biological membrane is selectively permeable to a single ion species $X$ with valence (charge) $z$, diffusion of the ion down its concentration gradient generates an opposing electrical voltage across the membrane. Equilibrium is reached when the electrical force exactly balances the chemical concentration gradient:

$$E_X = \frac{RT}{zF} \ln \left( \frac{[X]_{\text{outside}}}{[X]_{\text{inside}}} \right) = \frac{2.303 \, RT}{zF} \log_{10} \left( \frac{[X]_{\text{outside}}}{[X]_{\text{inside}}} \right)$$

Where:
* $R = 8.314 \, \text{J}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$
* $T$ is absolute temperature in Kelvin
* $z$ is the ionic charge ($+1$ for $\text{K}^+$ and $\text{Na}^+$; $+2$ for $\text{Ca}^{2+}$; $-1$ for $\text{Cl}^-$)
* $F = 96,485 \, \text{C}\cdot\text{mol}^{-1}$

### High-Speed Constants for CSIR NET Exams:
* **At $25^\circ\text{C}$ ($298 \, \text{K}$):** $\frac{2.303 \, RT}{F} \approx \mathbf{59.2 \, \text{mV}}$ (often rounded to $60 \, \text{mV}$):
  $$E_X \, (\text{mV}) = \frac{59.2}{z} \log_{10} \left( \frac{[X]_{\text{out}}}{[X]_{\text{in}}} \right)$$
* **At $37^\circ\text{C}$ ($310 \, \text{K}$, Mammalian Body Temp):** $\frac{2.303 \, RT}{F} \approx \mathbf{61.5 \, \text{mV}}$:
  $$E_X \, (\text{mV}) = \frac{61.5}{z} \log_{10} \left( \frac{[X]_{\text{out}}}{[X]_{\text{in}}} \right)$$

| Ion Species | Typical $[\text{Ion}]_{\text{in}}$ (mM) | Typical $[\text{Ion}]_{\text{out}}$ (mM) | Nernst Equilibrium Potential ($E_X$ at $37^\circ\text{C}$) |
| :--- | :--- | :--- | :--- |
| **$\text{K}^+$ ($z = +1$)** | $140 \, \text{mM}$ | $5 \, \text{mM}$ | $\approx -89 \, \text{mV}$ |
| **$\text{Na}^+$ ($z = +1$)** | $12 \, \text{mM}$ | $145 \, \text{mM}$ | $\approx +67 \, \text{mV}$ |
| **$\text{Ca}^{2+}$ ($z = +2$)** | $0.0001 \, \text{mM}$ ($100 \, \text{nM}$) | $1.5 \, \text{mM}$ | $\approx +128 \, \text{mV}$ |
| **$\text{Cl}^-$ ($z = -1$)** | $9 \, \text{mM}$ | $110 \, \text{mM}$ | $\approx -67 \, \text{mV}$ |

Because a resting neuron has a much higher permeability to $\text{K}^+$ ($P_{\text{K}}$) through leak channels than to $\text{Na}^+$ ($P_{\text{Na}}$), the resting membrane potential ($V_m \approx -70 \, \text{mV}$) sits close to $E_{\text{K}}$ ($-89 \, \text{mV}$).

## 2. Chemiosmotic Proton Motive Force ($\Delta p$)

Across the inner mitochondrial membrane or chloroplast thylakoid membrane, proton pumping generates an electrochemical proton gradient ($\Delta \mu_{\text{H}^+}$) composed of an electrical membrane potential ($\Delta \Psi$) and a chemical $\text{pH}$ gradient ($\Delta \text{pH} = \text{pH}_{\text{in}} - \text{pH}_{\text{out}}$).

Expressed in voltage units ($\text{mV}$) at $25^\circ\text{C}$, the **Proton Motive Force ($\Delta p$)** is:

$$\Delta p \, (\text{mV}) = \Delta \Psi - \left( \frac{2.303 \, RT}{F} \right) \Delta \text{pH} \approx \Delta \Psi - 59 \, \Delta \text{pH}$$

* **In Mitochondria:** The matrix is negatively charged relative to the intermembrane space ($\Delta \Psi \approx 160\text{–}180 \, \text{mV}$) and slightly alkaline ($\Delta \text{pH} \approx 0.7\text{–}1.0$ unit), so **$\Delta \Psi$ dominates** the proton motive force.
* **In Chloroplast Thylakoids:** Because $\text{Mg}^{2+}$ and $\text{Cl}^-$ flux dissipates $\Delta \Psi$ across the thylakoid membrane, **$\Delta \text{pH}$ ($\sim 3.0\text{–}3.5$ units) dominates** the proton motive force.

## 3. Worked CSIR NET Part C Numerical Problems

**Problem 1 (Divalent Ion Nernst Potential):** In a resting skeletal muscle fiber at $25^\circ\text{C}$ ($\frac{2.303 RT}{F} = 60 \, \text{mV}$), the cytosolic free $\text{Ca}^{2+}$ concentration is $10^{-7} \, \text{M}$ and the extracellular $\text{Ca}^{2+}$ concentration is $10^{-3} \, \text{M}$. Calculate the Nernst equilibrium potential for $\text{Ca}^{2+}$ ($E_{\text{Ca}}$).

**Solution:**
1. Identify the charge on $\text{Ca}^{2+}$: $z = +2$.
2. Substitute into the Nernst equation:
   $$E_{\text{Ca}} = \frac{60 \, \text{mV}}{+2} \log_{10} \left( \frac{10^{-3} \, \text{M}}{10^{-7} \, \text{M}} \right)$$
   $$E_{\text{Ca}} = 30 \, \text{mV} \times \log_{10}(10^4) = 30 \, \text{mV} \times 4 = +120 \, \text{mV}$$

**Problem 2 (Energetics of Ion Transport Against Electrochemical Gradients):** Calculate the free energy change ($\Delta G$ in $\text{kJ/mol}$) required to pump $1 \, \text{mol}$ of $\text{Na}^+$ ions out of a cell at $310 \, \text{K}$ ($RT = 2.58 \, \text{kJ/mol}$) against a $10$-fold concentration gradient ($[\text{Na}^+]_{\text{out}} / [\text{Na}^+]_{\text{in}} = 10$) when the cell interior is at a membrane potential of $-70 \, \text{mV}$ ($-0.070 \, \text{V}$) relative to the exterior.

**Solution:**
The total electrochemical work ($\Delta G$) required to move an ion of charge $z = +1$ from inside to outside is the sum of the chemical work and electrical work:

$$\Delta G = RT \ln \left( \frac{[\text{Na}^+]_{\text{out}}}{[\text{Na}^+]_{\text{in}}} \right) + z F \Delta \Psi_{\text{in} \rightarrow \text{out}}$$

1. **Chemical gradient work:**
   $$\Delta G_{\text{chem}} = 2.303 \times 2.58 \, \text{kJ/mol} \times \log_{10}(10) = +5.94 \, \text{kJ/mol}$$
2. **Electrical work** (moving $+1$ charge from $-0.070 \, \text{V}$ inside to $0 \, \text{V}$ outside requires overcoming $\Delta \Psi = +0.070 \, \text{V}$):
   $$\Delta G_{\text{elec}} = (+1) \times 96.485 \, \text{kJ}\cdot\text{V}^{-1}\cdot\text{mol}^{-1} \times (+0.070 \, \text{V}) = +6.75 \, \text{kJ/mol}$$
3. **Total Free Energy Required:**
   $$\Delta G_{\text{total}} = +5.94 + 6.75 = +12.69 \, \text{kJ/mol}$$

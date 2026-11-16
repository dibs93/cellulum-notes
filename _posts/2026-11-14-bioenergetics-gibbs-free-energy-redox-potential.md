---
layout: post
title: "Bioenergetics, Gibbs Free Energy & Redox Potential Numericals for CSIR NET"
description: "Step-by-step derivations connecting standard Gibbs free energy, equilibrium constants, Nernst redox potentials, and ATP synthesis in oxidative phosphorylation."
date: 2026-11-14
categories: [Biochemistry, Bioenergetics]
---

Thermodynamics and bioenergetics form a core analytical pillar of CSIR NET Life Sciences Unit 1. Part C numericals routinely test your ability to calculate whether a metabolic reaction is spontaneous under cellular concentrations, link equilibrium constants ($K_{\text{eq}}$) to standard free energy changes ($\Delta G^{\circ\prime}$), and convert electron transport chain redox potentials ($\Delta E_0^{\prime}$) into ATP yield.

## 1. Actual vs. Standard Transformed Gibbs Free Energy ($\Delta G^{\circ\prime}$)

In biochemistry, standard state conditions are defined at $\text{pH } 7.0$ ($[H^+] = 10^{-7} \, \text{M}$), $25^\circ\text{C}$ ($298 \, \text{K}$), $1 \, \text{atm}$ pressure, and $1 \, \text{M}$ initial concentration of reactants and products. For a general reaction $aA + bB \rightleftharpoons cC + dD$, the actual free energy change ($\Delta G$) inside a living cell is given by:

$$\Delta G = \Delta G^{\circ\prime} + RT \ln \left( \frac{[C]^c [D]^d}{[A]^a [B]^b} \right)$$

Where:
* $R = 8.314 \, \text{J}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$ (or $1.987 \, \text{cal}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$)
* $T$ is the absolute temperature in Kelvin ($\text{K} = ^\circ\text{C} + 273.15$)
* $Q = \frac{[C]^c [D]^d}{[A]^a [B]^b}$ is the mass-action ratio at the current cellular concentrations

At chemical equilibrium, net reaction velocity ceases ($\Delta G = 0$) and the mass-action ratio equals the equilibrium constant ($K_{\text{eq}}^{\prime}$):

$$\Delta G^{\circ\prime} = -RT \ln K_{\text{eq}}^{\prime} = -2.303 \, RT \log_{10} K_{\text{eq}}^{\prime}$$

At standard physiological temperature ($298 \, \text{K}$ or $25^\circ\text{C}$), the factor $2.303 \, RT$ simplifies to approximately **$5.706 \, \text{kJ/mol}$** (or $1.36 \, \text{kcal/mol}$). Every $10$-fold increase in $K_{\text{eq}}^{\prime}$ shifts $\Delta G^{\circ\prime}$ by $-5.7 \, \text{kJ/mol}$.

## 2. Coupled Reactions & Additive Free Energy

Thermodynamically unfavorable (endergonic, $\Delta G > 0$) biosynthetic reactions are driven forward by coupling them to highly exergonic reactions ($\Delta G < 0$) such as ATP hydrolysis ($\Delta G^{\circ\prime} = -30.5 \, \text{kJ/mol}$) or pyrophosphate ($\text{PP}_i$) cleavage.

For sequential reactions $A \rightleftharpoons B$ ($\Delta G_1^{\circ\prime}$) and $B \rightleftharpoons C$ ($\Delta G_2^{\circ\prime}$):
* **Free energies are additive:** $\Delta G_{\text{overall}}^{\circ\prime} = \Delta G_1^{\circ\prime} + \Delta G_2^{\circ\prime}$
* **Equilibrium constants are multiplicative:** $K_{\text{eq, overall}} = K_{\text{eq}, 1} \times K_{\text{eq}, 2}$

## 3. Redox Potentials ($\Delta E_0^{\prime}$) & Electron Transport

In mitochondrial oxidative phosphorylation and photosynthetic electron flow, free energy changes are driven by electron transfer from a donor with a more negative reduction potential ($E_0^{\prime}$) to an acceptor with a more positive reduction potential:

$$\Delta E_0^{\prime} = E_0^{\prime}(\text{Acceptor / Reduced}) - E_0^{\prime}(\text{Donor / Oxidized})$$

The standard free energy change is linked to $\Delta E_0^{\prime}$ via the Faraday constant ($F = 96.485 \, \text{kJ}\cdot\text{V}^{-1}\cdot\text{mol}^{-1}$):

$$\Delta G^{\circ\prime} = -n F \Delta E_0^{\prime}$$

Where $n$ is the number of electrons transferred per molecule. A positive $\Delta E_0^{\prime}$ always yields a negative $\Delta G^{\circ\prime}$ (spontaneous electron transfer).

| Redox Couple (Oxidized / Reduced) | Electrons ($n$) | Standard Reduction Potential $E_0^{\prime}$ (V) |
| :--- | :--- | :--- |
| $\text{NAD}^+ + 2H^+ + 2e^- \rightarrow \text{NADH} + H^+$ | $2$ | $-0.320 \, \text{V}$ |
| $\text{FAD} + 2H^+ + 2e^- \rightarrow \text{FADH}_2$ | $2$ | $-0.219 \, \text{V}$ |
| $\text{Ubiquinone (Q)} + 2H^+ + 2e^- \rightarrow \text{QH}_2$ | $2$ | $+0.045 \, \text{V}$ |
| $\text{Cytochrome } c \, (\text{Fe}^{3+}) + e^- \rightarrow \text{Cyt } c \, (\text{Fe}^{2+})$ | $1$ | $+0.254 \, \text{V}$ |
| $\frac{1}{2}\text{O}_2 + 2H^+ + 2e^- \rightarrow \text{H}_2\text{O}$ | $2$ | $+0.816 \, \text{V}$ |

## 4. Worked CSIR NET Part C Numerical Problems

**Problem 1 (Glycolytic Equilibrium):** The isomerization of dihydroxyacetone phosphate (DHAP) to glyceraldehyde-3-phosphate (G3P) catalyzed by triose phosphate isomerase has a $\Delta G^{\circ\prime}$ of $+7.5 \, \text{kJ/mol}$ at $298 \, \text{K}$. Inside an actively respiring hepatocyte, $[\text{DHAP}] = 2 \times 10^{-4} \, \text{M}$ and $[\text{G3P}] = 3 \times 10^{-6} \, \text{M}$. Calculate the actual $\Delta G$ and state whether the reaction proceeds toward G3P formation in vivo.

**Solution:**
1. Set up the mass-action ratio $Q$:
   $$Q = \frac{[\text{G3P}]}{[\text{DHAP}]} = \frac{3 \times 10^{-6}}{2 \times 10^{-4}} = 0.015$$
2. Substitute into the Gibbs equation ($RT = 8.314 \times 298 = 2477.6 \, \text{J/mol} \approx 2.48 \, \text{kJ/mol}$):
   $$\Delta G = +7.5 + (2.48 \times \ln(0.015))$$
   $$\ln(0.015) = -4.20$$
   $$\Delta G = +7.5 + (2.48 \times -4.20) = +7.5 - 10.42 = -2.92 \, \text{kJ/mol}$$
3. Because cellular G3P is continuously consumed by subsequent glycolytic steps, $\Delta G$ becomes negative ($-2.92 \, \text{kJ/mol}$), driving the reaction spontaneously forward in vivo despite its positive $\Delta G^{\circ\prime}$.

**Problem 2 (ETC Redox Span):** Calculate the standard free energy released ($\Delta G^{\circ\prime}$) when $1 \, \text{mol}$ of $\text{NADH}$ is oxidized by molecular oxygen ($\text{O}_2$) via the mitochondrial electron transport chain.

**Solution:**
1. Identify $E_0^{\prime}$ for the acceptor ($\text{O}_2/\text{H}_2\text{O} = +0.816 \, \text{V}$) and donor ($\text{NAD}^+/\text{NADH} = -0.320 \, \text{V}$):
   $$\Delta E_0^{\prime} = +0.816 - (-0.320) = +1.136 \, \text{V}$$
2. For $n = 2$ electrons transferred per molecule of $\text{NADH}$:
   $$\Delta G^{\circ\prime} = -2 \times 96.485 \, \text{kJ}\cdot\text{V}^{-1}\cdot\text{mol}^{-1} \times 1.136 \, \text{V} = -219.2 \, \text{kJ/mol}$$
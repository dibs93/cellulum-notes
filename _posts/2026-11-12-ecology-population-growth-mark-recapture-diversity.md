---
layout: post
title: "Quantitative Ecology: Population Growth, Mark-Recapture & Diversity Indices"
description: "Complete mathematical derivations and solved CSIR NET Part C problems on exponential vs. logistic growth, Lincoln-Petersen mark-recapture, and Shannon/Simpson diversity."
date: 2026-11-12
categories: [Ecology, Population Biology]
---

Unit 10 (Ecological Principles) is one of the highest-return sections in CSIR NET Life Sciences because its Part C numericals rely on a compact set of predictable equations. Mastering exponential and logistic growth models, Lincoln-Petersen population estimation, and community diversity indices guarantees fast, accurate problem-solving.

## 1. Exponential vs. Logistic Population Growth Models

### A. Exponential (Density-Independent) Growth
When resources are unlimited, a population grows at a constant per-capita intrinsic rate of natural increase ($r = b - d$, where $b$ is instantaneous birth rate and $d$ is instantaneous death rate):

$$\frac{dN}{dt} = rN \implies N_t = N_0 \, e^{rt}$$

The **doubling time ($t_d$)** required for a population to double in size ($N_t / N_0 = 2$) is:

$$t_d = \frac{\ln(2)}{r} \approx \frac{0.693}{r}$$

### B. Logistic (Density-Dependent) Growth
In real environments with a finite **carrying capacity ($K$)**, intraspecific competition slows growth as $N$ approaches $K$:

$$\frac{dN}{dt} = rN \left( \frac{K - N}{K} \right) = rN \left( 1 - \frac{N}{K} \right)$$

* **Inflection Point (Maximum Sustainable Yield):** The population growth rate ($\frac{dN}{dt}$) reaches its absolute maximum when **$N = \frac{K}{2}$**.
* At $N = \frac{K}{2}$, the maximum addition of individuals per unit time is:
  $$\left( \frac{dN}{dt} \right)_{\max} = r \left( \frac{K}{2} \right) \left( 1 - \frac{1}{2} \right) = \frac{rK}{4}$$

## 2. Lincoln-Petersen Mark-Recapture Method

To estimate the total size ($\hat{N}$) of a mobile animal population in a closed habitat:
1. Capture, mark, and release **$M$** individuals in the first sampling.
2. Allow sufficient time for marked individuals to mix randomly into the general population.
3. Capture a second sample of **$C$** total individuals, among which **$R$** individuals carry marks.

Assuming equal catchability and no births, deaths, or migration between samples, the ratio of marked individuals in the second sample reflects the ratio in the entire population:

$$\frac{R}{C} = \frac{M}{\hat{N}} \implies \hat{N} = \frac{M \times C}{R}$$

## 3. Community Diversity: Shannon ($H'$) & Simpson ($D$) Indices

Species diversity incorporates both **species richness ($S$)** and **species evenness**. Let $p_i = \frac{n_i}{N}$ represent the relative abundance (proportion) of species $i$ in the community:

### A. Shannon-Wiener Diversity Index ($H'$)
$$H' = -\sum_{i=1}^{S} p_i \ln(p_i)$$

* $H'$ reaches its theoretical maximum ($H_{\max}' = \ln S$) when all species are present in equal abundance ($p_i = \frac{1}{S}$).
* **Pielou's Evenness ($J'$):** $J' = \frac{H'}{\ln S}$ (ranges from $0$ to $1$).

### B. Simpson's Index of Dominance ($D$) & Diversity ($1 - D$)
$$D = \sum_{i=1}^{S} p_i^2 \quad \text{or} \quad D = \frac{\sum n_i(n_i - 1)}{N(N - 1)}$$

* **Simpson's Index of Diversity:** $1 - D$ (probability that two randomly selected individuals belong to different species).
* **Simpson's Reciprocal Index:** $\frac{1}{D}$ (ranges from $1$ to $S$).

## 4. Worked CSIR NET Part C Numerical Problems

**Problem 1 (Logistic Yield):** A fish population in a lake follows logistic growth with an intrinsic growth rate $r = 0.4 \, \text{year}^{-1}$ and a carrying capacity $K = 10,000$ individuals. 
1. At what population size ($N$) does the population grow fastest?
2. What is the maximum number of fish that can be harvested per year without depleting the population below that optimal level?

**Solution:**
1. Maximum growth occurs at the inflection point: $N = \frac{K}{2} = \frac{10,000}{2} = 5,000 \text{ fish}$.
2. Maximum sustainable harvest equals $\left(\frac{dN}{dt}\right)_{\max}$:
   $$\left(\frac{dN}{dt}\right)_{\max} = \frac{rK}{4} = \frac{0.4 \times 10,000}{4} = 1,000 \text{ fish/year}$$

**Problem 2 (Mark-Recapture Trap):** Ecologists captured and tagged $120$ beetles in a forest plot. One week later, they captured $150$ beetles, of which $15$ had tags. However, laboratory testing revealed that $20\%$ of the tags fell off during the week. Calculate the true corrected population size ($\hat{N}$).

**Solution:**
* If $20\%$ of the tags were lost, the effective number of marked beetles remaining in the population ($M_{\text{effective}}$) or the effective recapture count must be corrected. Since $20\%$ of captured tagged beetles lost their tags, the $15$ observed tagged beetles represent $80\%$ ($0.8$) of the true recaptured cohort:
  $$R_{\text{true}} = \frac{15}{0.8} = 18.75$$
* Alternatively, effective marked individuals available for detection $= 120 \times 0.8 = 96$:
  $$\hat{N} = \frac{96 \times 150}{15} = 960 \text{ beetles}$$

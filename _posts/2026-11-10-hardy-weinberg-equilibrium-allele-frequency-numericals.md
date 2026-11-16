---
layout: post
title: "Hardy-Weinberg Equilibrium, X-Linked Traits & Inbreeding Coefficient Numericals"
description: "Step-by-step derivations and solved CSIR NET Part C problems on autosomal vs. X-linked allele frequencies, heterozygote carrier probabilities, and Wright's inbreeding coefficient."
date: 2026-11-10
categories: [Genetics, Evolution]
---

Population genetics bridges Unit 8 (Inheritance Biology) and Unit 11 (Evolution and Behavior) in CSIR NET Life Sciences. Part C numericals frequently combine Hardy-Weinberg Equilibrium (HWE) equations with pedigree carrier probabilities, X-linked recessive traits, or Wright's inbreeding coefficient ($F$).

## 1. Autosomal Diallelic & Multiallelic Hardy-Weinberg Equilibrium

In a large, randomly mating diploid population free from mutation, migration, natural selection, and genetic drift, allele and genotype frequencies remain constant across generations.

For a single autosomal locus with two alleles, $A$ (frequency $p$) and $a$ (frequency $q$):

$$p + q = 1$$

$$(p + q)^2 = p^2 + 2pq + q^2 = 1$$

* **Homozygous Dominant ($AA$):** $p^2$
* **Heterozygous Carrier ($Aa$):** $2pq$
* **Homozygous Recessive ($aa$):** $q^2$

### Calculating Allele Frequencies Directly from Observed Genotype Counts
When testing whether a real population is in Hardy-Weinberg equilibrium (or when selection/inbreeding distorts genotype ratios), **do not** take the square root of $q^2$. Instead, calculate $p$ and $q$ directly from total observed individuals ($N = N_{AA} + N_{Aa} + N_{aa}$):

$$p = \frac{2N_{AA} + N_{Aa}}{2N} = f(AA) + \frac{1}{2}f(Aa)$$

$$q = \frac{2N_{aa} + N_{Aa}}{2N} = f(aa) + \frac{1}{2}f(Aa)$$

### Extension to Three Alleles (e.g., ABO Blood Group System: $I^A = p, I^B = q, i = r$)
When three alleles control a locus ($p + q + r = 1$), the equilibrium genotype expansion is:

$$(p + q + r)^2 = p^2 + q^2 + r^2 + 2pq + 2pr + 2qr = 1$$

* **Blood Group O ($ii$):** $r^2$
* **Blood Group A ($I^A I^A + I^A i$):** $p^2 + 2pr$
* **Blood Group B ($I^B I^B + I^B i$):** $q^2 + 2qr$
* **Blood Group AB ($I^A I^B$):** $2pq$

## 2. X-Linked Recessive Traits in Males vs. Females

Because human males are hemizygous ($XY$) for X-linked genes, they inherit only one copy of the X chromosome. Therefore, the phenotypic incidence of an X-linked recessive disorder (such as hemophilia or red-green color blindness) in males directly equals the recessive allele frequency $q$:

| Sex / Ploidy | Affected Frequency | Carrier Frequency (Phenotypically Normal) |
| :--- | :--- | :--- |
| **Hemizygous Males ($XY$)** | $q$ | $0$ (Males cannot be silent carriers) |
| **Diploid Females ($XX$)** | $q^2$ | $2pq$ |

For rare X-linked recessive conditions ($q = 0.01$), affected males ($q = 1/100$) are $100$ times more common than affected females ($q^2 = 1/10,000$).

## 3. Wright's Inbreeding Coefficient ($F$) & Heterozygote Deficit

Inbreeding (non-random mating between genetic relatives) increases homozygosity at the expense of heterozygosity **without altering underlying allele frequencies ($p$ and $q$)**. If $F$ represents the inbreeding coefficient ($0 \le F \le 1$):

* **Observed Heterozygote Frequency ($H_O$):** $f(Aa) = 2pq(1 - F)$
* **Homozygous Dominant Frequency:** $f(AA) = p^2 + pqF$
* **Homozygous Recessive Frequency:** $f(aa) = q^2 + pqF$

Rearranging the heterozygote equation yields the standard formula for $F$ in CSIR NET Part C:

$$F = \frac{H_E - H_O}{H_E} = 1 - \frac{H_O}{2pq}$$

Where $H_E = 2pq$ is the expected Hardy-Weinberg heterozygosity under random mating.

## 4. Worked CSIR NET Part C Numerical Problems

**Problem 1 (Autosomal Recessive Carrier Probability):** Cystic fibrosis is an autosomal recessive disorder affecting $1$ in $2,500$ newborns in a population at Hardy-Weinberg equilibrium. What is the frequency of heterozygous carriers in this population?

**Solution:**
1. Homozygous recessive frequency $q^2 = \frac{1}{2500} = 0.0004$.
2. Recessive allele frequency $q = \sqrt{0.0004} = 0.02$.
3. Dominant allele frequency $p = 1 - 0.02 = 0.98$.
4. Heterozygous carrier frequency $2pq = 2 \times 0.98 \times 0.02 = 0.0392$ (or approximately **$1$ in $25.5$ individuals**).

**Problem 2 (Inbreeding Coefficient Calculation):** In a plant population of $1000$ individuals, genotyping at a codominant locus reveals $460 \, AA$, $160 \, Aa$, and $380 \, aa$ plants. Calculate the allele frequencies ($p$ and $q$) and Wright's inbreeding coefficient ($F$).

**Solution:**
1. **Calculate observed genotype frequencies:**
   * $f(AA) = 0.46$
   * $f(Aa) = H_O = 0.16$
   * $f(aa) = 0.38$
2. **Calculate true allele frequencies:**
   * $p = f(AA) + \frac{1}{2}f(Aa) = 0.46 + 0.08 = 0.54$
   * $q = f(aa) + \frac{1}{2}f(Aa) = 0.38 + 0.08 = 0.46$
3. **Calculate Expected Heterozygosity ($H_E$):**
   $$H_E = 2pq = 2 \times 0.54 \times 0.46 = 0.4968$$
4. **Calculate Inbreeding Coefficient ($F$):**
   $$F = \frac{H_E - H_O}{H_E} = \frac{0.4968 - 0.1600}{0.4968} = \frac{0.3368}{0.4968} \approx 0.678$$

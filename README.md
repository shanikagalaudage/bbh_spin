# Binary black hole spin distribution

This repository contains results and supplementary materials for the work presented in [arXiv:2109.02424](https://arxiv.org/abs/2109.02424) **_Building better spin models for merging binary black holes: Evidence for non-spinning and rapidly spinning nearly aligned sub-populations_**

## Abstract:
Recent work paints a conflicting portrait of the distribution of black hole spins in merging binaries measured with gravitational waves. Some analyses find that a significant fraction of merging binaries contain at least one black hole with a spin tilt >90∘ with respect to the orbital angular momentum vector, which has been interpreted as a signature for dynamical assembly. Other analyses find the data are consistent with a bimodal population in which some binaries contain black holes with negligible spin while the rest contain black holes with spin vectors preferentially aligned with the orbital angular momentum vector. In this work, we scrutinize models for the distribution of black hole spins to pinpoint possible failure modes in which the model yields a faulty conclusion. We reanalyze data from the second LIGO--Virgo gravitational-wave transient catalog (GWTC-2) using a revised spin model, which allows for a sub-population of black holes with negligible spins. In agreement with recent results by Roulet et al., we show that the GWTC-2 detections are consistent with two distinct sub-populations. We estimate that 29−75% (90\% credible interval) of merging binaries contain black holes with negligible spin χ≈0. The remaining binaries are part of a second sub-population in which the spin vectors are preferentially (but not exactly) aligned to the orbital angular momentum. The black holes in this second sub-population are characterized by spins of χ∼0.45. We suggest that the inferred spin distribution is consistent with the hypothesis that all merging binaries form via the field formation scenario.

## Repository contents
* [posterior samples](./posterior_samples) - the samples from the event posteriors read in for the population analysis
* [hyper posterior samples](./hyperposterior_samples) - samples for the population analysis using the _Extended_ spin model
* [plots](./plots) - contains the figures from the publication and additional plots

For results for the _Default_ spin model results, see the official data release from LIGO/Virgo [here](https://dcc.ligo.org/LIGO-P2000434/public) in `Population_Samples.tar.gz`

Detailed documentation on how to read in and plot the data is yet to be added to this repository. If you haave any questions about the data and/or results please contact me via email at shanika.galaudage@monash.edu

## Science summary

Two subpopulations for spin disribution of merging binary black holes.
1. ~54% of binaries with negliglible spins
2. remaining binaries rapidly spinning (χ∼0.45) that are preferentially aligned with the orbital angular momentum of the binary

The _Extended_ spin model is significantly favoured (by a log10 Bayes factor of ~3.55) compared to the _Default_ model. There is no _clear_ evidence for binaries tilted greater than 90 degrees w.r.t. the orbital angular momentum, suggesting that the current population can be explained by the isolated binary evolution scenario.

<!--
The results in the paper are also summarised in this [poster](https://shanikagalaudage.github.io/pdfs/talks_posters/Poster_LVK_Sep2021.pdf).
-->
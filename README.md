# Reservoir Computing (ESN) for Nonlinear Dynamics Prediction

This repository contains code and a short report on using **Echo State Networks (ESN)** / **reservoir computing** to (i) reconstruct system dynamics from experimental time series of a periodically driven nonlinear magnetic rotor, (ii) perform **short-term trajectory prediction**, and (iii) evaluate consistency between model and measurements via statistical quantities (e.g., autocorrelation, power spectrum) and predictability metrics (e.g., maximal Lyapunov exponent).

## Contents
- **Code**: ESN training/inference pipelines for both **open-loop** (externally driven) and **closed-loop** (autonomous feedback) prediction, plus evaluation utilities (wrapped angular error, short-horizon metrics, etc.).
- **Report**: `ESN Report.pdf` — the accompanying write-up describing the experimental setup, preprocessing, ESN methodology, results, and discussion.

## Highlights
- Open-loop ESN achieves high-accuracy short-term pointwise prediction under external driving.
- Closed-loop prediction can track the true trajectory briefly but typically exhibits error growth over time.
- Lyapunov exponent estimation requires careful methodology; naive fitting of true–prediction error can be misleading.


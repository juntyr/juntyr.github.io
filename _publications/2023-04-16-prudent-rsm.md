---
title: "Prudent Response Surface Models: Exploring a Framework for Approximating Simulations with Confidence and Certainty"
collection: publications
category: theses
permalink: /publication/2023-04-16-prudent-rsm
excerpt: 'The Icarus Response Surface Model architecture combines an out-of-distribution detector, a prediction model, and an uncertainty quantifier.'
date: 2023-04-16
venue: 'University of Helsinki'
paperurl: 'https://helda.helsinki.fi/items/5b2537e1-5673-4b7a-83a5-6fb35fc8255d'
citation: '<b>Tyree, J.</b> (2023) <i>Prudent Response Surface Models: Exploring a Framework for Approximating Simulations with Confidence and Certainty</i>. Master’s Thesis. Available from: <a href="http://urn.fi/URN:NBN:fi:hulib-202305151941">URN:NBN:fi:hulib-202305151941</a>.'
---

* Supervisors:
  * Prof. Michael Boy, University of Helsinki, LUT University
  * Dr Andreas Rupp, LUT University
  * Petri Clusius, University of Helsinki

## Abstract

Response Surface Models (RSM) are cheap, reduced complexity, and, usually, statistical models that are fit to the response of more complex models to approximate their outputs with higher computational efficiency. In atmospheric science, there has been a continuous push to reduce the amount of training data required to fit an RSM. With this reduction in costly data gathering, RSMs can be used more ad hoc and quickly adapted to new applications. However, with the decrease in diverse training data, the risk increases that the RSM is eventually used on inputs on which it cannot make a prediction. If there is no indication from the model that its outputs can no longer be trusted, trust in an entire RSM decreases. We present a framework for building *prudent* RSMs that always output predictions with confidence and uncertainty estimates. We show how confidence and uncertainty can be propagated through downstream analysis such that even predictions on inputs outside the training domain or in areas of high variance can be integrated.

Specifically, we introduce the Icarus RSM architecture, which combines an out-of-distribution detector, a prediction model, and an uncertainty quantifier. Icarus-produced predictions and their uncertainties are conditioned on the confidence that the inputs come from the same distribution that the RSM was trained on. We put particular focus on exploring out-of-distribution detection, for which we conduct a broad literature review, design an intuitive evaluation procedure with three easily-visualisable toy examples, and suggest two methodological improvements. We also explore and evaluate popular prediction models and uncertainty quantifiers.

We use the one-dimensional atmospheric chemistry transport model SOSAA as an example of a complex model for this thesis. We produce a dataset of model inputs and outputs from simulations of the atmospheric conditions along air parcel trajectories that arrived at the SMEAR II measurement station in Hyytiälä, Finland, in May 2018. We evaluate several prediction models and uncertainty quantification methods on this dataset and construct a proof-of-concept SOSAA RSM using the Icarus RSM architecture. The SOSAA RSM is built on pairwise-difference regression using random forests and an auto-associative out-of-distribution detector with a confidence scorer, which is trained with both the original training inputs and new synthetic out-of-distribution samples. We also design a graphical user interface to configure the SOSAA model and trial the SOSAA RSM.

We provide recommendations for out-of-distribution detection, prediction models, and uncertainty quantification based on our exploration of these three systems. We also stress-test the proof-of-concept SOSAA RSM implementation to reveal its limitations for predicting model perturbation outputs and show directions for valuable future research. Finally, our experiments affirm the importance of reporting predictions alongside well-calibrated confidence scores and uncertainty levels so that the predictions can be used with confidence and certainty in scientific research applications.

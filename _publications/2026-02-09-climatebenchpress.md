---
title: "ClimateBenchPress (v1.0): A Benchmark for Lossy Compression of Climate Data"
collection: publications
category: preprints
permalink: /publication/2026-02-09-climatebenchpress
excerpt: 'We address this gap by presenting ClimateBenchPress, a benchmark suite for lossy compression of climate data, which defines both data sets and evaluation techniques.'
date: 2026-02-09
venue: 'EGUsphere'
paperurl: 'https://doi.org/10.5194/egusphere-2026-60'
citation: 'Reichelt, T., <b>Tyree, J.</b>, Klöwer, M., Dueben, P., Lawrence, B. N., Baker, A. H., Faghih-Naini, S., Hoefler, T., and Stier, P. (2026). ClimateBenchPress (v1.0): A Benchmark for Lossy Compression of Climate Data. <i>EGUsphere</i> [preprint]. Available from: <a href="https://doi.org/10.5194/egusphere-2026-60">doi:10.5194/egusphere-2026-60</a>.'
---

## Abstract

The rapidly growing volume of weather and climate data, both from models and observations, is increasing the pressure on data centers, restricting scientific analysis, and data distribution. For example, kilometre-scale climate models can generate petabytes of data per simulated month, making it generally infeasible to store all output. To address this challenge, numerous novel compression techniques have been proposed to ease data storage requirements. However, there exist no well-defined benchmarks for rigorously evaluating and comparing the performance of these compressors, including their impact on the data's properties. The lack of benchmarks makes it difficult to design and standardize compressors for weather and climate data, and for scientists to trust that compression errors have no significant impact on their analysis. Here, we address this gap by presenting ClimateBenchPress, a benchmark suite for lossy compression of climate data, which defines both data sets and evaluation techniques. The benchmark covers climate variables following various statistical distributions at medium to very high resolution in time and space, from both numerical models and satellite observations. To ensure a fair comparison between different compressors, each variable comes with a set of maximum error bound checks that the lossy compressors need to pass. By evaluating an initial set of baseline compressors on the benchmark, we gather practical insights for effective application of lossy compression. Our benchmark is open source and extensible: users can easily add new compressors, data sources, and evaluation metrics depending on their own specific use cases.

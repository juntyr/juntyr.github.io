---
title: "Compression Safeguards: Building Trust into Lossy Data Compression"
collection: publications
category: preprints
permalink: /publication/2026-07-28-safeguards
excerpt: 'We introduce Compression Safeguards, a user-centric and domain-independent framework to overcome this trust gap. Safeguards can unlock the data reduction benefits of lossy compression and therefore solve many data storage problems across the scientific community that otherwise hinder research.'
date: 2026-07-28
venue: 'EGUsphere'
paperurl: 'https://doi.org/10.5194/egusphere-2026-4266'
citation: '<b>Tyree, J.</b>, Underwood, R., Bouvier, C., Köhler, D., Reichelt, T., Dueben, P., Faghih-Naini, S., Järvinen, H., and Klöwer, M. (2026). Compression Safeguards: Building Trust into Lossy Data Compression. <i>EGUsphere</i> [preprint]. Available from: <a href="https://doi.org/10.5194/egusphere-2026-4266">doi:10.5194/egusphere-2026-4266</a>.'
---

## Abstract

The growth in data volumes produced by scientific models is accelerating. Data production of high-resolution weather and climate models is outpacing the methods and budgets for storing, sharing, and analysing this data, posing a threat to scientific progress. Lossy data compression greatly reduces data sizes but loses some quality, detail, or precision of the original data. Even though some lossy compressors promise size reductions of 100x or more, the lack of trust in lossy compression, rooted in the risk of losing important information, has thus far limited their adoption.

We introduce Compression Safeguards, a user-centric and domain-independent framework to overcome this trust gap, with which

(i) scientists declare their precise safety requirements for what lossy compression must preserve, e.g. regionally varying error bounds on quantities derived from the decompressed data, then

(ii) wrap a compressor of their choice in the corresponding safeguards, which then

(iii) guarantee that the safety requirements are always met by the safeguarded compressor, at most at the cost of a reduced compression ratio.

The Compression Safeguards represent a paradigm shift: Data producers and users no longer carry the risks of lossy compression, having to manually check for problems after compression, but instead control up-front what needs to be safeguarded. With the appropriate safeguards, trust can grow in all lossy compressors and even untrusted, potentially unsafe compressors can be used safely and with confidence. Users thus no longer need to re-verify each new compressor for each new use case, or to restrict themselves to few safe compressors and supported use cases.

We showcase how our reference implementation of the Compression Safeguards can be flexibly applied to safeguard important properties across several real-world examples from weather and climate sciences for different compressors. The impact on compression ratio varies but is small in many cases. The computational load increases during compression but is negligible during decompression.

Altogether, Compression Safeguards provide a key modular tool that gives users the confidence to use lossy compression safely across scientific disciplines. Safeguards can unlock the data reduction benefits of lossy compression and therefore solve many data storage problems across the scientific community that otherwise hinder research.

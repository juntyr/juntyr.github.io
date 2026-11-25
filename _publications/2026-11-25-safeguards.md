---
title: "Compression Safeguards: building trust into lossy data compression"
collection: publications
category: manuscripts
permalink: /publication/2026-11-25-safeguards
excerpt: 'We introduce Compression <i>Safeguards</i>, a user-centric and domain-independent framework to overcome this trust gap. Safeguards can unlock the data reduction benefits of lossy compression and therefore solve many data storage problems across the scientific community that otherwise hinder research.'
date: 2026-11-25
venue: 'Geoscientific Model Development'
paperurl: 'https://doi.org/10.5194/gmd-19-11265-2026'
citation: '<b>Tyree, J.</b>, Underwood, R., Bouvier, C., Köhler, D., Reichelt, T., Dueben, P., Faghih-Naini, S., Järvinen, H., and Klöwer, M. (2026). Compression Safeguards: building trust into lossy data compression. <i>Geoscientific Model Development</i>, 19, 11265–11335. Available from: <a href="https://doi.org/10.5194/gmd-19-11265-2026">doi:10.5194/gmd-19-11265-2026</a>.'
---

## Abstract

The growth in data volumes produced by scientific models is accelerating. Data production of high-resolution weather and climate models is outpacing the methods and budgets for storing, sharing, and analysing this data, posing a threat to scientific progress. Lossy data compression greatly reduces data sizes but loses some quality, detail, or precision of the original data. Even though some lossy compressors promise size reductions of 100× or more, the lack of trust in lossy compression, rooted in the risk of losing important information, has thus far limited their adoption.

We introduce Compression <i>Safeguards</i>, a user-centric and domain-independent framework to overcome this trust gap, with which

(i) scientists declare their precise safety requirements for what lossy compression must preserve, e.g. regionally varying error bounds on quantities derived from the decompressed data, then

(ii) wrap a compressor of their choice in the corresponding safeguards, which then

(iii) <i>guarantee</i> that the user-declared safety requirements are <i>always</i> met by the safeguarded compressor.

The Compression Safeguards represent a paradigm shift: Data producers and users no longer carry the risks of lossy compression, having to manually check for problems after compression, but instead control up-front what needs to be safeguarded. With the appropriate application-specific safeguards, trust can grow in all lossy compressors and even untrusted, potentially unsafe compressors can be used safely and with confidence. Users thus no longer need to re-verify each new compressor for each new use case, or to restrict themselves to few safe compressors and supported use cases.

We showcase how our reference implementation of the Compression Safeguards can be flexibly applied to safeguard important properties across several real-world examples from weather and climate sciences for different compressors. The cost of the Safeguards is a reduced compression throughput, significantly when safeguarding complex safety requirements, and lower compression ratios if the Safeguards have to correct the decompressed data to uphold its safety. There is only minor overhead during decompression.

Altogether, Compression Safeguards provide a key modular tool that gives users the confidence to use lossy compression safely across scientific disciplines. Safeguards can unlock the data reduction benefits of lossy compression and therefore solve many data storage problems across the scientific community that otherwise hinder research.

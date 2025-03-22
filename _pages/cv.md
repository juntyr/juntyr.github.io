---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Doctoral Student in Atmospheric Sciences, University of Helsinki, Finland, 2023-2027 (expected)
* MSc in Theoretical and Computational Methods, University of Helsinki, Finland, 2021-2023
* MEng in Computing, Imperial College London, United Kingdom, 2017-2021
* Allgemeine Hochschulreife, Hans-Sachs Gymnasium Nürnberg, Germany, 2009-2017

Language Skills
=====
* German (native)
* English (C2)
* French (B1+)

Work Experience
======
* 2023/05-: Doctoral Researcher
  * University of Helsinki, Institute for Atmospheric and Earth System Research
  * Investigating safe lossy data compression for weather and climate model data
  * Supervisors:
    * Prof. Heikki J. Järvinen, University of Helsinki
    * Dr Milan Klöwer, University of Oxford
  * Thesis Committee:
    * Prof. Michale Boy, University of Helsinki, LUT University
    * Prof. James Rosindell, Imperial College London
    * Dr Holger Pirk, Imperial College London

* 2022/09-2023/04: Research Assistant
  * University of Helsinki, Institute for Atmospheric and Earth System Research
  * Investigated Out-of-Distribution Detection, Uncertainty Quantification, and Response Surface Modelling for a 1D atmospheric transport chemistry and aerosol process model, SOSAA
  * Implemented a graphical user interface to configure and run the SOSAA model
  * Supervisors:
    * Prof. Michael Boy, University of Helsinki, LUT University
    * Dr Andreas Rupp, LUT University
    * Petri Clusius, University of Helsinki

* 2022/05-2022/09: Research Assistant
  * University of Helsinki, Department of Computing
  * Investigated dimensionality reduction for eXplainable AI for molecular data
  * Implemented a WebAssembly-based serverless data analysis and visualisation platform, xiplot
  * Supervisors:
    * Prof. Kai Puolamäki, University of Helsinki
    * Anton Björklund, University of Helsinki

* 2020/04-2020/09: Industrial Placement
  * EMBL-EBI (European Bioinformatics Institute)
  * Automated and streamlined the curation process of the identifiers.org platform
  * Supervisors:
    * Henning Hermjakob, European Bioinformatics Institute
    * Manuel Bernal Llinares, European Bioinformatics Institute

* 2019/08-2019/09: Undergraduate Research Opportunity
  * Imperial College London, Department of Life Sciences
  * Investigated neutral simulations of species richness and extended the analytical description to account for endemic islands and the transition from endemicity to migration
  * Co-implemented the Gillespie algorithm as an optimisation to the coalescence simulation
  * Supervisors:
    * Prof. James Rosindell, Imperial College London
    * Dr Lucas D. Fernandes, Imperial College London

* 2017-2021: Group project leader
  * Imperial College London, Department of Computing
  * Developed & optimised a scalable peer-to-peer collaborative drawing Web App using conflict-free replicated data types (CRDTs) and WebRTC
  * Iteratively designed and user-tested the first prototype for the Octopus science publishing platform, <https://www.octopus.ac/>
  * Developed an optimising compiler with an error recovering frontend for the WACC language in Rust
  * Implemented system-level thread scheduling, system calls and virtual memory for PintOS in C
  * Created an assembler and emulator for the Raspberry Pi and its GPIO pins in C to develop a game

Teaching Experience
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Career Breaks
======
* Parental Leave, 2023/11-2024/01 (full-time), 2024/01-2025/07 (part-time)

Funding
======
* 2023-2026: 100% PhD salary, from: ESiWACE3, Center of excellence for weather and climate phase 3. Horizon EuroHPC. Available from: [doi:10.3030/101093054](https://doi.org/10.3030/101093054).

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        <ul>
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single-cv.html %}
    {% endfor %}
    {% if title_shown %}
      </ul>
    {% endif %}
  {% endfor %}
{% else %}
  <ul>{% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}</ul>
{% endif %}
  
Presentations
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Professional Contributions
======
* Convener: Bouvier, C., Co-Conveners: Ray, W., Santoro, M., **Tyree, J.**, Borejko, W., Tinto, O., Faghih-Naini, S. (05/2025). Big Data in Earth System Sciences: The Challenges of Data Compression & Data Spaces in the cloud computing era. *EGU25 Session ESSI2.13*. Available from: <https://meetingorganizer.copernicus.org/EGU25/session/52084> [Accessed: 17th March 2025]

Awards and Honours
======
* Governor’s MEng Prize in Computing to the final year student with the best overall performance, Imperial College London, 2020-2021
* Dean’s List (Year 4), Imperial College London, 2020-2021
* Aspect Capital Prize for an outstanding final year undergraduate individual projectImperial College London, 2020-2021
* Dean’s List (Year 3), Imperial College London, 2019-2020
* G-Research Prize for academic excellence, Imperial College London, 2019-2020
* David Howarth Group Project Prize for excellence in group projects in the third year, Imperial College London, 2019-2020
* G-Research Prize for academic excellence, Imperial College London, 2018-2019
* Olav Beckmann Project Prize for outstanding 2nd-year laboratory project work, Imperial College London, 2018-2019
* Computing Entrance Scholarship, Imperial College London, 2017-2018

References are available on request
======

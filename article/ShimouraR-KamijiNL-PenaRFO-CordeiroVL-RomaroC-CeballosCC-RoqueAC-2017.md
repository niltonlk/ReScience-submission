---
Title: "The cell-type specific cortical microcircuit: relating structure and activity in a full-scale spiking network model"
Author:
  - name: Renan O. Shimoura,
    affiliation: 1
  - name: Nilton L. Kamiji,
    affiliation: 1
  - name: Rodrigo F.O. Pena,
    affiliation: 1
  - name: Vinicius L. Cordeiro,
    affiliation: 1
  - name: Cesar C. Ceballos,
    affiliation: 1, 2
  - name: Cecilia Romaro,
    affiliation: 1
  - name: Antonio C. Roque,
    affiliation: 1
Address:
  - code:    1
    address: Faculty of Philosophy, Sciences and Letters at Ribeir\~{a}o Preto, Department of Physics, University of S\~{a}o Paulo, Ribeir\~{a}o Preto, S\~{a}o Paulo, Brazil
  - code:    2
    address: Department of Physiology, Ribeir\~{a}o Preto Medical School, School of Medicine, University of S\~{a}o Paulo, Ribeir\~{a}o Preto, Brazil
Contact:
  - antonior@usp.br
Editor:
  - Name Surname
Reviewer:
  - Name Surname
  - Name Surname
Publication:
  received:  Sep, 1, 2015
  accepted:  Sep, 1, 2015
  published: Sep, 1, 2015
  volume:    "**1**"
  issue:     "**1**"
  date:      Sep 2015
  number: 1
Repository:
  article:   "http://github.com/rescience/rescience-submission/article"
  code:      "http://github.com/rescience/rescience-submission/code"
  data:      
  notebook:  
Reproduction:
  - "The cell-type specific cortical microcircuit: relating structure and activity in a full-scale spiking network model, T.C. Potjans,  M. Diesmann, Cerebral Cortex, 24 (3): 785-806, 2014. DOI: 10.1093/cercor/bhs358"
Bibliography:
  ShimouraR-KamijiNL-PenaRFO-CordeiroVL-RomaroC-CeballosCC-RoqueAC-2017.bib

---

# Introduction

Most theoretical studies of cortical activity are based on networks of randomly connected units @brunel2000,@vogels2005,@kriener2014,@ostojic2014 
or with architectures artificially
built from random networks @tomov2014. In spite of the usefulness of these models, in order to understand the interplay between network structure and cortical dynamics it is essential to have computational models which accurately represent the cortical network architecture. Recently, Potjans and Diesmann @potjans2014 developed a network model of the local cortical microcircuit based on extensive experimental data on the intrinsic circuitry of striate cortex @thomson2002,@binzegger2004.
The model contains two cell types (excitatory and inhibitory) distributed over four layers, L2/3, L4, L5, and L6, and represents the cortical network below a surface area of 1 $mm^{2}$ (a scheme is shown in Fig.@fig:diagram_net).

![Schematic representation of the cortical network model (adapted from @potjans2014).
 The model consists of four layers (L2/3, L4, L5 and L6), each one populated with excitatory (triangles) and inhibitory (circles) neurons (Table @table:population). Arrows represent connections with probabilities $>$ 0.04: excitatory in red and inhibitory in blue (Table @table:conectivity). Black arrows represent background inputs.](diagram.pdf){#fig:diagram_net}

The original implementation was based on the NEST simulator @gewaltig2007 and the source code is available at the Open Source Brain platform @potjans2014pyNEST.
Here, we reimplemented the full model in the Brian 2 simulator @goodman2009 without direct reference to the original source code. 

# Methods

In this work, we replicated in Brian 2 every detail of the Potjans-Diesmann model as described in their original article @potjans2014. Hereafter, we will refer to the original NEST implementation of the Potjans-Diesmann model @potjans2014 as reference (or original) article.  In this section we explain how this reimplementation was done. Further statistical analyses were performed using SciPy, NumPy, and Matplotlib libraries for the Python language.

## Neurons

Network neurons are described by the leaky integrate-and-fire (LIF) neuron model. The subthreshold membrane voltage of neuron $i$ obeys the equation

$$ \dot{V}_i(t) = -\left( V_i(t) - V_{\rm reset} \right) /\tau_m + I_i(t)/C_m, $$ {#Eq:LIF}


# Results

The methods section should explain how you replicated the original results:

* did you use paper description
* did you contact authors ?
* did you use original sources ?
* did you modify some parts ?
* etc.

If relevevant in your domain, you should also provide a new standardized
description of the work.


# Results

Results should be compared with original results and you have to explain why
you think they are the same or why they may differ (qualitative result vs
quantitative result). Note that it is not necessary to redo all the original
analysis of the results.


# Conclusion

Conclusion, at the very minimum, should indicate very clearly if you were able
to replicate original results. If it was not possible but you found the reason
why (error in the original results), you should exlain it.


Heading 1                          Heading 2
---------- ----------- ----------- ----------- ----------- -----------
cell1 row1 cell2 row 1 cell3 row 1 cell4 row 1 cell5 row 1 cell6 row 1
cell1 row2 cell2 row 2 cell3 row 2 cell4 row 2 cell5 row 2 cell6 row 2
cell1 row3 cell2 row 3 cell3 row 3 cell4 row 3 cell5 row 3 cell6 row 3
---------- ----------- ----------- ----------- ----------- -----------

Table: Table caption {#tbl:table}

A reference to table @tbl:table.
A reference to figure @fig:logo.
A reference to equation @eq:1.
A reference to citation @markdown.

![Figure caption](rescience-logo.pdf){#fig:logo}

$$ A = \sqrt{\frac{B}{C}} $$ {#eq:1}


# References

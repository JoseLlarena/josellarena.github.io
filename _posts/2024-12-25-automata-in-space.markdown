---
layout: post
title:  "Automata in Spades"
date: Wed 25 Dec 21:01:04 GMT 2024
tags: [NNs WFSAs Explanation]
author: J. Llarena
---

PDF [Automata in Space: Formal Language Theory meets Neural Computation](/assets/doc/ais-paper-v2.pdf).

Code: [https://github.com/JoseLlarena/ais](https://github.com/JoseLlarena/ais)

BibTeX Citation:
```
@unpublished{llarena2024automata,
  author    = {Llarena, J.},
  title     = {Automata in Space: Formal Language Theory meets Neural Computation},
  note      = {https://josellarena.github.io/assets/doc/ais-paper-v2.pdf},
  year      = {2024}
}
```

_Automata in Space_ presents the main piece of work I've done in the last couple of years, laying the 
foundations of what I expect to be my core research topic moving forward. It intersects the fields of Formal Language Theory,
Computational Psycho-/Neuro-/Linguistics and Machine Learning.

The heart of my approach is to use weighted automata to understand neural computation. Though the use of
automata is not new, research on recurrent neural networks used them as early as the 80s [^servan] [^rodriguez],
it's only recently that researchers have used them to understand non-recurrent architectures like Transformers[^rizvi] and to
draw stronger theoretical links between Formal Language Theory and NNs[^merrill], with extensive empirical studies showing the strengths
and limits of different architecture[^deletang].

My work contrasts with existing research in that I:
 1. use the linear representation of Weighted Finite State Automata (WFSAs)[^balle] as a mathematically sound reverse 
 engineering normative models to compare the hidden space of neural networks against; vs the implicit or 
 ad-hoc approaches often found in the literature 

 2. set the scope to be studying all distributed representations for linguistic capabilities; vs specific architectures
 or general tasks

 3. tackle the study of neural representation mechanistically, treating models as white-boxes; vs extracting automata,
 proving expressivity limits or establishing empirical equivalences

 4. favour a geometric computational-state view, making heavy use of 3-dimensional state-diagrams; vs feature-based 
 analysis using 2D plots

_1\._ limits the study to tasks that can be represented as regular languages (like XOR/PARITY). I plan to lift that 
restriction by employing Weighted Pushdown Automata, extending the scope to context-free languages. It also 
restricts its remit to classification and language modelling, a limitation I plan to overcome using Weighted Finite 
State Transducers. See the "Conclusion and Future Work" section in the paper for other limitations of this technique and the 
future research paths they suggest.

_2\._ reflects my long-standing interest in how the higher-level organisation of language emerges from a lower-level 
non-symbolic substrate.

_3\._ is an attempt to cut through the historically protracted arguments about whether a computer program is or isn't a 
good model for human performance; and if not, how the human "algorithm" differs from the one learned by machines.

_4\._ stems from a strongly held belief that neural computation is best causally explained in terms of a series of
steps that (fail to) solve the task at hand, using well understood computational models (i.e. sequential automata), as 
opposed to the more common approach of comparing hidden representations of inputs.

If you are interested in this line of research, do get in touch through [email](mailto:jose.llarena@gmail.com), 
[linkedin](https://www.linkedin.com/in/josellarena), [mastodon](https://sigmoid.social/@LL4R3N4) or
[bluesky](https://bsky.app/profile/ll4r3n4.bsky.social). Looking forward to hearing your thoughts.
      

**References**

[^servan]: [_Servan-Schreiber, D., Cleeremans, A. and McClelland, J., 1988. Learning sequential structure in simple recurrent networks. Advances in neural information processing systems, 1._](https://proceedings.neurips.cc/paper/1988/file/9dcb88e0137649590b755372b040afad-Paper.pdf)
[^rodriguez]: [_Rodriguez P. Simple recurrent networks learn context-free and context-sensitive languages by counting. Neural Comput. 2001 Sep;13(9):2093-118. doi: 10.1162/089976601750399326. PMID: 11516_](https://pubmed.ncbi.nlm.nih.gov/11516359)
[^rizvi]: [_Rizvi-Martel, M., Lizaire, M., Lacroce, C. and Rabusseau, G., 2024, April. Simulating weighted automata over sequences and trees with transformers. In International Conference on Artificial Intelligence and Statistics (pp. 2368-2376). PMLR._](https://proceedings.mlr.press/v238/rizvi-martel24a/rizvi-martel24a.pdf)
[^merrill]: [_Merrill, W., 2021. Formal language theory meets modern NLP. arXiv preprint arXiv:2102.10094._](https://arxiv.org/pdf/2102.10094)
[^deletang]: [_Delétang, G., Ruoss, A., Grau-Moya, J., Genewein, T., Wenliang, L.K., Catt, E., Cundy, C., Hutter, M., Legg, S., Veness, J. and Ortega, P.A., 2022. Neural networks and the chomsky hierarchy. arXiv preprint arXiv:2207.02098._](https://arxiv.org/pdf/2207.02098)
[^balle]: [_Balle, B., Carreras, X., Luque, F.M. et al. Spectral learning of weighted automata. Mach Learn 96, 33–63 (2014). https://doi.org/10.1007/s10994-013-5416-x_](https://link.springer.com/article/10.1007/s10994-013-5416-x)


---
layout: post
title:  "Automata in Spades"
date:   2024-10-26 18:51:11 +0100
tags: [NNs WFSAs Explanation]
author: J. Llarena
---

Paper PDF [Automata in Space: Formal Language Theory meets Neural Computation](/assets/doc/ais.pdf).

_Automata in Space_ presents the main topic of research I've done in the last couple of years, laying the 
foundations of what I expect to be my core research topic moving forward. It intersects the fields of Formal Language Theory,
Computational Psycho-/Neuro-/Linguistics and Machine Learning.

The heart of my approach is to use weighted automata to understand neural computation. Though the use of
automata is not new, research on recurrent neural networks used them as early as the 80s (Giles et al. 1992)[^Giles92],
it's only recently that researchers have used them to understand non-recurrent architectures like Transformers[^citation2] and to
draw stronger theoretical links between Formal Langauge Theory and NNs, with extensive empirical studies showing the strengths
and limits of different architectures[^citation3].

My work contrasts with existing research in that I:
 1. use the linear representation of Weighted Finite State Automata (WFSAs)[^citation4] as a mathematically sound reverse 
 engineering normative models to compare the hidden space of neural networks against; vs the implicit or 
 ad-hoc approaches often found in the literature 

 2. set the scope to be studying all distributed representations for linguistic capabilities; vs specific architectures
 or general tasks

 3. tackle the study of neural representation mechanistically, treating models as white-boxes; vs extracting automata,
 proving expressivity limits or establishing empirical equivalences

 4. favour a geometric computational-state view, making heavy use of 3-dimensional state-diagrams; vs feature-based 
 analysis using 2D plots

_1\._ limits the study to tasks that can be represented as regular languages (like XOR/PARITY). I plan to lift that 
restriction by employing Weighted Pushdown Automata (WPDAs), extending the scope to context-free languages. It also 
restricts its remit to classification and language modelling, a limitation I plan to overcome using Weighted Finite 
State Transducers (WFSTs). See the "Future Work" section in the paper for other limitations of this technique and the 
future research paths they suggest.

_2\._ reflects my long-standing interest in how the higher-level organisation of language emerges from a lower-level 
non-symbolic substrate.

_3\._ is an attempt to cut through the historically protracted arguments about whether a computer program is or isn't a 
good model for human performance; and if not, how the human "algorithm" differs from the one learned by machines.

_4\._ stems from a strongly held belief that neural computation is best causally explained in terms of a series of
steps that (fail to) solve the task at hand, using well understood computational models (i.e. sequential automata), as 
opposed to the more common approach of comparing hidden representations of inputs.

If you are interested in this line or research, do get in touch through [email](mailto:jose.llarena@gmail.com), 
[linkedin](https://www.linkedin.com/in/josellarena), [mastodon](https://sigmoid.social/@LL4R3N4) or
[bluesky](https://bsky.app/profile/ll4r3n4.bsky.social). Looking forward to hearing your thoughts.
      

**References**

[^Giles92]: _Giles, C.L., Miller, C.B., Chen, D., Chen, H.H., Sun, G.Z. and Lee, Y.C., 1992. Learning and extracting finite state automata with second-order recurrent neural networks. Neural Computation, 4(3), pp.393-405._
[^citation2]: what
[^citation3]: what
[^citation4]: what



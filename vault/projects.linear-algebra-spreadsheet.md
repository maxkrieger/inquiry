---
id: 06ea3d39-0b83-4052-86f2-f1e82499b266
title: Linear Algebra as Spreadsheet
updated: 1711602765192
modified: 2024-03-27T23:57:37-07:00
desc: null
---

_Thanks to Garth Goldwater for a lot of the ideas here_

[The metaphor isn't mine](https://betterexplained.com/articles/linear-algebra-guide/). But it's a good one!

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Is there an intrinsic reason MATLAB-esque tasks can&#39;t be as WYSIWYG as a spreadsheet?<br><br>How do you represent matrix multiplication in a graphical environment? I want to drag and drop my eigendecomposition as tangibly as a sort operation.</p>&mdash; Max Krieger (@maxkriegers) <a href="https://twitter.com/maxkriegers/status/1246619921896873985?ref_src=twsrc%5Etfw">April 5, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Some tools on the way to supporting the magical, playful mode of waves:<a href="https://t.co/fa5Sunkwhh">https://t.co/fa5Sunkwhh</a><a href="https://t.co/FQKTRWzyje">https://t.co/FQKTRWzyje</a><br>and the unimplemented direct manipulation APL-spreadsheet-incantation environment of my dreams <a href="https://t.co/TFxhVS1UIq">https://t.co/TFxhVS1UIq</a></p>&mdash; Max Krieger (@maxkriegers) <a href="https://twitter.com/maxkriegers/status/1306129848038027265?ref_src=twsrc%5Etfw">September 16, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

So I was wondering why nobody took it literally.

> When you're manipulating matrices, you [often] lose track of, "what am I doing? what does this mean?" I've got this funny matrix, I multiply it by a vector, what was this supposed to do?

- Keenan Crane, [Discrete Exterior Calculus](https://youtu.be/-cUhuzwW-_A)

I can't find any existing _direct manipulation_ interfaces to perform linear algebra on raw data. Stuff like eigendecomposition or factorization. Or [constructing proofs of SVD](http://cognitivemedium.com/emm/emm.html).

The key, I think, is to map the _language_ of linear algebra to an _interaction semantics_ for linear algebra ([[theory.interaction-semantics]]).

Here's what I _have_ found:

## Excel!?

Sure I guess?

- [Performing Operations with Matrices on Spreadsheets](https://www.jstor.org/stable/27970545?seq=1)

## [[APL Is Really Cool|projects.linear-algebra-spreadsheet.apl]]

## Aesthetics

- ["Spectral decomposition? Oh you mean like when a ghost dies?"](https://twitter.com/likethebuilder/status/1326583332306554880?s=19)

## other

- What if there was a set of flashcards to learn all the APL symbols? Like [Elixir Cards](https://elixircards.co.uk/)/[PixelSpirit](https://patriciogonzalezvivo.github.io/PixelSpiritDeck/).

One subproject ([[theory.subprojecting]]) is not APL, but some CAS matrix toy - "Linearkit".

- Nicky Case's [transformation matrix toy](https://ncase.me/matrix/)

## Direct manipulation refs

- 2d

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">isolate a data column by dragging it out of the table. also got a little semantic text editing going <a href="https://t.co/ZW6ukuk2UK">pic.twitter.com/ZW6ukuk2UK</a></p>&mdash; Paul Shen (@_paulshen) <a href="https://twitter.com/_paulshen/status/1366801887341649924?ref_src=twsrc%5Etfw">March 2, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

![](assets/images/2021-03-09-21-13-39.png)

- [WebGL State Diagram](https://webglfundamentals.org/webgl/lessons/resources/webgl-state-diagram.html) - the "cells" are pointers
  - Maybe each matrix is a floating table and you can multiply by constructing a graph of edges?
  - [Graphical Linear Algebra](https://graphicallinearalgebra.net/)
- [**Graspable Math**](https://graspablemath.com/)
- [Responsive Matrix Cells: A Focus+Context Approach for Multivariate Graphs](https://imld.de/en/research/research-projects/responsive-matrix-cells/)
- [Loglo](https://loglo.app/)
- [Math Inspector](https://mathinspector.com/)
  - > Math inspector makes it easy for anyone to leverage the power of numpy, the most popular computational mathematics library in the world, without needing to know anything about programming or writing any code. “If watching math videos is like going to the movies instead of reading a book, then math inspector is like playing a video game instead of doing your homework.”
- [Interactivity of Visual Mathematical Representations: Factors Affecting Learning and Cognitive Processes](https://eric.ed.gov/?id=EJ726333) ([pdf](../assets/interactive-math-tools.pdf))

![](assets/images/2021-02-01-17-39-06.png)

[Forms/3](https://pdfs.semanticscholar.org/a074/a04c61f097ee9ad13f9061aee95d1dd0c01f.pdf)

## Semantics refs

- [Graphical Linear Algebra](https://graphicallinearalgebra.net/)
- [An Illustrated Guide to Arquero Verbs / UW Interactive Data Lab / Observable](https://observablehq.com/@uwdata/an-illustrated-guide-to-arquero-verbs)
- [A Grammar of Data Manipulation • dplyr](https://dplyr.tidyverse.org/)
- ["Verb-noun vs noun-verb"](https://mobile.twitter.com/tophtucker/status/1278184444428529665?s=19)
- [Thoughts on how to find alternate algebra-like systems](https://westoncb.blogspot.com/2017/10/thoughts-on-how-to-find-alternate.html)
- [Named tensor notation](https://namedtensor.github.io/)
- https://github.com/amzn/computer-vision-basics-in-microsoft-excel

Every right click transformation (eg transpose, get eigens) is not in-place but is placed somewhere else in space, immutable copy, like Paul Shen's systems.

## Applications

- Learning, proving, playing
- graphics pipelines (in 2d case of env layout)
- statistics
- DSP (vision - convolutions, audio)
- ML

## Why?

- Not sure.
  - Might be internalized trauma taking linear algebra without something that feels nice to use ([[rethinking-media.microworld-languages]]).
  - Practitioners make numpy mistakes a lot I bet
  - How do you communicate intuition about [powerful ideas](https://llk.media.mit.edu/courses/readings/Papert-Big-Idea.pdf) in linalg? Are pictures the best we have? What about the _algebra_, and the _data_ embedded in every matrix?
- The semantics of Linear Algebra are pretty well-defined I think? That's why it's an algebra, right?
- I want to do casual mathematics
- Linear Algebra can model a lot of other domains of math. Not to mention it's pretty useful for physics. So maybe the interface paradigm can be juiced into domain-specific applications ([[theory.juicing]], [[theory.bottom-up]]).

https://arxiv.org/abs/1702.02131

https://jhupbooks.press.jhu.edu/title/chinese-roots-linear-algebra

https://www.goodreads.com/book/show/2448489

https://github.com/Timwi/HexagonyColorer

https://cragl.cs.gmu.edu/iheartla/rethinkingpapers/preprint.pdf

https://iheartla.github.io/

https://twitter.com/anton_hilado/status/1289956291750887424?s=09

https://www.labri.fr/perso/nrougier/from-python-to-numpy/

https://github.com/rougier/numpy-100

https://rajatvd.github.io/Factor-Graphs/

https://guillaumegenthial.github.io/image-to-latex.html

Spectral clustering/decomposition of some images you drag in

Gensim

https://auto.gluon.ai/stable/index.html

https://math.mit.edu/~gs/learningfromdata/

https://twitter.com/SC_Griffith/status/1506489478453600258?s=20

Lots of matmul happening here:
https://www.mattkeeter.com/projects/mrep/

![](/assets/images/2022-04-24-19-42-52.png)

https://transformer-circuits.pub/2021/exercises/index.html

![](/assets/images/2022-04-28-19-49-07.png)

https://jalammar.github.io/illustrated-transformer/

![](/assets/images/2022-05-05-15-04-36.png)

![](/assets/images/2022-05-05-15-04-45.png)

![](/assets/images/2022-05-05-15-04-55.png)

https://dl.acm.org/doi/fullHtml/10.1145/3491102.3501823

https://twitter.com/jeremyphoward/status/1523775789879422976?s=21&t=ecPZB2KLDqNU4hC58wRbmQ

https://twitter.com/mark_riedl/status/1555188022534176768

https://github.com/quil-lang/magicl/blob/master/doc/high-level.md

https://twitter.com/joel_burget/status/1562469068464017408

https://towardsdatascience.com/mnist-handwritten-digits-classification-from-scratch-using-python-numpy-b08e401c4dab

https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/nbextensions/varInspector/README.html

![](/assets/images/2022-09-01-19-27-18.png)

https://e2eml.school/transformers.html

https://github.com/srush/Tensor-Puzzles

**I should definitely do this first**
https://minitorch.github.io/
https://numpy.org/doc/stable/user/basics.broadcasting.html

https://github.com/kenjihiranabe/The-Art-of-Linear-Algebra

https://github.com/xl0/lovely-tensors

https://twitter.com/_paulshen/status/1600653533371863040

https://news.ycombinator.com/item?id=30101637

Linear algebra brushes https://twitter.com/Wattenberger/status/1610472915623112704?s=20&t=ATlA1Rzg3kVKSSUco2KTLw

https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf

https://x.com/voooooogel/status/1701290465482645808?s=46&t=ZaQiMOEZuQ_6mGivtLEwMA

Pytorch made a visualizaton:

https://pytorch.org/blog/inside-the-matrix/

https://bhosmer.github.io/mm/ref.html

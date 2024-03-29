---
id: bff6ee82-45d7-4702-bb59-542b05920ae9
title: How do you create an interaction semantics?
updated: 1707948572135
modified: 2022-06-01T00:47:33+09:00
desc: null
---

Programming semantics are well-studied. What about direct manipulation semantics? Can they be [in bijection](https://twitter.com/sliminality/status/1227791682038452225)?

I'm especially interested in, say, reflecting mathematical semantics in interactive diagrams. With [Penrose](https://penrose.ink), we've been asking, eg, what dragging a point outside a circle in a venn diagram means mathematically - it's an "edit" in the mathematical construction.

This is true for other domains that have a formal representation underlying a highly interactive one.

![](assets/images/2021-02-13-23-23-06.png)

([UI Continuations](http://people.csail.mit.edu/karger/Papers/uist2003-uicont.pdf))

![](/assets/images/2021-10-13-01-23-46.png)

[Expressive Query Construction through Direct Manipulation of Nested Relational Results](http://people.csail.mit.edu/ebakke/research/sieuferd_sigmod2016.pdf)

[Karger's lab](http://people.csail.mit.edu/karger/) has a disproportionate number of these kinds of papers!

![fructure](https://raw.githubusercontent.com/disconcision/fructure/master/screenshots/fructure-rounded-modified.gif)

([Fructure](https://github.com/disconcision/fructure). BTW I'm not just talking about program editors, they're just a convenient example to point to.)

- [Semantics of Visual Languages](http://web.engr.oregonstate.edu/~erwig/vlsem/)

## Direct manipulation (mouse, not keyboard)

What even is a program? You can make great Smalltalk ([[projects.system-archaeology]]) programs without writing much code at all. I'm not talking about [no-code/future-code](https://futureofcoding.org/catalog/), but rather, _writing a trace of behavior_ by _live_ (not premeditated) interactions on objects.

- Context menus are cool, actually
- [UI Continuations](http://people.csail.mit.edu/karger/Papers/uist2003-uicont.pdf) - curried context menus!!!
- [Histogram by Tomas Petricek](http://tomasp.net/histogram/) - "We represent programs as _lists of interactions_"
- [Wrangler: Interactive Visual Specification of Data Transformation Scripts](http://idl.cs.washington.edu/papers/wrangler/)
- [You can model the domain of raytracing by interacting with InkScape layers](https://github.com/damienBloch/Inkscape-raytracing)
- [Interaction Techniques in InfoViz (Ji Soo Yi et al)](https://www.cc.gatech.edu/~stasko/papers/infovis07-interaction.pdf)
- Brad Myers' [TOPAZ](http://www.cs.cmu.edu/~amulet/papers/commandsbydemo.pdf)

![](assets/images/2021-02-11-15-39-10.png)

- [Self Language](https://selflanguage.org/) (and other Morphic environments) turns green empty "morphs" into rich interactive objects just through right-clicking

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">“Verb-noun vs noun-verb” <a href="https://t.co/eNPRq3AqrC">https://t.co/eNPRq3AqrC</a><br><br>Thanks to Omar <a href="https://t.co/WZk6BIbXX4">https://t.co/WZk6BIbXX4</a> for reminding me of Amit’s excellent post; see also <a href="https://t.co/fdf7EPmvKW">https://t.co/fdf7EPmvKW</a>.<br><br>Anyone have any other good literature on subject-verb order in GUIs? <a href="https://t.co/ntvKPyO4cd">https://t.co/ntvKPyO4cd</a> <a href="https://t.co/BCLu2D7WVH">pic.twitter.com/BCLu2D7WVH</a></p>&mdash; TOoᴼᵒº˙⁰0₀ₒ.·ph (@tophtucker) <a href="https://twitter.com/tophtucker/status/1278184444428529665?ref_src=twsrc%5Etfw">July 1, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## Structure editing (keyboard, not mouse)

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">an interface as a thin veneer over a structured program, manipulable in a structured manner, always in bijection 🥰</p>&mdash; Nintendo .DS_Store (@sliminality) <a href="https://twitter.com/sliminality/status/1227791682038452225?ref_src=twsrc%5Etfw">February 13, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

- [Fructure](https://github.com/disconcision/fructure) - "a structured interaction engine"
- [Hazel](https://hazel.org)
  - [You can formally prove every action in a structure editor](https://arxiv.org/abs/1703.08694)

[//begin]: # "Autogenerated link references for markdown compatibility"
[system-archaeology]: system-archaeology.md "System Archaeology Seminar"
[//end]: # "Autogenerated link references"

## Programming by demonstration

![](assets/images/2021-02-11-22-59-30.png)

- [Mondrian: A Teachable Graphical Editor](https://web.media.mit.edu/~lieber/Lieberary/Mondrian/Mondrian.html)

https://observablehq.com/@observablehq/data-wrangler

https://twitter.com/andy_matuschak/status/1435772997155971073?s=21

https://twitter.com/_paulshen/status/1463202129619808259

https://maryrosecook.notion.site/Scapula-9fc4b570f0234d569d982c022435433d

emacs’ context menu mode https://ruzkuku.com/texts/emacs-mouse.html

https://twitter.com/prathyvsh/status/1304420854135021575

https://twitter.com/yoshikischmitz/status/1232914839791493125

SnapGene is very much “gene programming by demonstration” - all your plasmid edits get recorded and diffed into a step by step protocol https://www.snapgene.com/features/#configured-for-automatic-documentation-and-easy-data-exchange

https://www.destroyallsoftware.com/screencasts/catalog/functional-core-imperative-shell

> This is a tiny toy programming system inspired by several ideas:

> Turtle graphics as in LOGO, but with a
> bidirectional user interface as in Sketch-n-Sketch, but using
> gradient-based updates as in ML systems.

Kartik Chandra's Differentiable Snap! https://kach.github.io/turtlegrad/

https://twitter.com/disconcision/status/1508912020380434439?s=20&t=gYgR5XSK1vgFHppPMZlIdg

https://faculty.washington.edu/ajko/papers/Ko2005Citrus.pdf

![](/assets/images/2022-04-11-12-47-00.png)

Figure 8 of https://profs.etsmtl.ca/mmcguffin/research/2020-mcguffin-VPLs/mcguffin-avi2020.pdf

There's a very deep truth about noun-verb distinction in UI.

Figure 4 of https://andrewhead.info/assets/pdf/augmented-formulas.pdf

https://twitter.com/rsnous/status/1531353260279402497?s=21&t=lenlmBapUWsoEj03jcBbbA

- [Mito: Edit a spreadsheet. Generate Python. All in Jupyter.](https://trymito.io/)

"Documents as user interfaces"
https://dl.acm.org/doi/abs/10.1145/108844.108994

EDA as query builder https://twitter.com/hamiltonulmer/status/1757793824649478149
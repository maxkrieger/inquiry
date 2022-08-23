---
id: 1rCLzzZwVdcOICn9eIrII
title: Most explorables should be IDE plugins
updated: 1661229722
created: 1644370273705
desc: null
---

Andy introduces a critique of explorables that has stuck with me:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Here&#39;s my crux: The Cartesian plane was not invented to disseminate mathematics, or to make math more engaging. It was invented to help *do math*.<br><br>The same point can be made about John Snow’s cholera map, Feynman QED diagrams, and our other most powerful representations.</p>&mdash; Andy Matuschak (@andy_matuschak) <a href="https://twitter.com/andy_matuschak/status/1305264244896587776?ref_src=twsrc%5Etfw">September 13, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

> [Explorables are] striking, they’re often more interesting to read than normal articles, and the dynamic elements often make it easier to understand the author, but one doesn’t walk away from the article with the dynamic environment in one’s pocket, so to speak.

([Most dynamic representations developed for communication aren’t very enabling](https://notes.andymatuschak.org/zB5wf5crA1jVZb6CycZSjGRTjSkw2BpsdjG))

An interpretation that follows: 3blue1brown's videos about linear algebra are beautiful and likely improve mental imagery when thinking causally about things like linear transformations. However, Gilbert Strang's notation-heavy lectures on the same subject are presented with the same interface learners use: chalkboards. When we have to actually factorize a matrix, the only way we can do that in our current media environment is by writing things down.

---

Explorables introduce novel UI and representational ideas all the time. Here's a possible shortcut to situating/testing these ideas in a working context: **put the interface in the IDE**.

Suppose I want to put A\* in my game. I should be able to see [RedBlobGames'](https://www.redblobgames.com/pathfinding/a-star/introduction.html) pathfinding representation as soon as I want to import A\* and integrate it in my codebase. Mapping my data structure to _his_ data structure and gaining an understanding of the algorithm's pathologies.

IDEs (and notebooks) are extensible objects, and you can often add arbitrary views on top of the original textual representation you're working with. This is the [Livelits](https://web.eecs.umich.edu/~comar/livelits-tyde.pdf) approach:

![Livelits](/assets/images/2022-02-08-18-07-55.png)

(see also [[theory.interaction-semantics]])

There are several recent explorables that could fit quite nicely into a larger IDE setting!

### Interfaces for Explaining Transformer Language Models

[by Jay Alammar](https://jalammar.github.io/explaining-transformers/)

This saliency list could easily be a notebook widget:

![](/assets/images/2022-02-08-18-11-45.png)

Same for these sparklines:

![](/assets/images/2022-02-08-18-12-28.png)

These seem like useful interfaces for doing real work with these models (not totally sure though).

### Giving scientists superpowers in the battle against aging with MegaMap

[by Spring Discovery](https://www.springdiscovery.com/blog/megamap/)

These also could be notebook widgets:

![](/assets/images/2022-02-08-18-16-03.png)

![](/assets/images/2022-02-08-18-15-52.png)

This is visualizing a for-loop! Could yield it [tqdm](https://tqdm.github.io/) style.

<video loop width="100%">
    <source src="https://i.imgur.com/JmkiFY4.mp4" type="video/mp4">
</video>

### Introduction to Computational Thinking

([started by Grant Sanderson](https://computationalthinking.mit.edu/))

This one's kinda cheating, it's literally a collection of notebooks. But Julia IDEs need better math notation support and you can extrapolate other representations from the ones in this course.

Like this grid literal!

![](/assets/images/2022-02-08-18-25-07.png)

### RedBlobGames

https://www.redblobgames.com/grids/line-drawing.html

https://handmade.network/p/283/bifold-text

---

Related: [[theory.ide-for-x]], [[rethinking-media.microworld-languages]]

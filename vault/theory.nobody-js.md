---
id: gq4j5n4nb4efyxn3ll5kl9e
title: Nobody Knows How To Write JavaScript
desc: ""
updated: 1646074103282
created: 1646073983970
---

From [Sig](https://twitter.com/sigfig): basic things like loop unrolling etc get JITted in mysterious ways that deeply affect performance. Twitter.com does `malloc` on each cursor movement.

Some learnings I got from her:

- Keep discriminated union discriminator key/values short so you don't have to do string comparison under the hood
- Sometimes for-loops are better than map/filter/reduce

Read https://v8.dev/blog and digest it into idioms/lint rules

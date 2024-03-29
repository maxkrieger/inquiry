---
id: 7b2d9c24-ae42-4d85-972e-6918eee280e9
title: Destroy Abstraction
desc: null
updated: 1619578421412
modified: 2021-08-30T14:55:38-07:00
---

_Re-bootstrapping your way to freedom_

Some of the most exciting software projects these days aren't new abstractions. They destroy existing abstractions. And they're fast and delightful.

This means no Webkit, Electron, or V8.

Evanw's [Esbuild](https://esbuild.github.io/faq/#why-is-esbuild-fast):

> **Everything in esbuild is written from scratch.**
> There are a lot of performance benefits with writing everything yourself instead of using 3rd-party libraries. You can have performance in mind from the beginning, you can make sure everything uses consistent data structures to avoid expensive conversions, and you can make wide architectural changes whenever necessary. The drawback is of course that it's a lot of work.
> For example, many bundlers use the official TypeScript compiler as a parser. But it was built to serve the goals of the TypeScript compiler team and they do not have performance as a top priority. Their code makes pretty heavy use of megamorphic object shapes and unnecessary dynamic property accesses (both well-known JavaScript speed bumps). And the TypeScript parser appears to still run the type checker even when type checking is disabled. None of these are an issue with esbuild's custom TypeScript parser.

## Some systems

- [ESBuild](https://esbuild.github.io/)
- [Xi Editor](https://raphlinus.github.io/xi/2020/06/27/xi-retrospective.html) (RIP?)
- [Volt](https://volt-app.com/) (and [V language](https://vlang.io/))
- [Ripcord](https://cancel.fm/ripcord/)
- [**Playbit**](https://playb.it/) - [podcast episode](https://museapp.com/podcast/27-playful-software/)
- [Nova](https://nova.app/) - no Vim emulation? wtf!
- [Neovim?](https://neovim.io/)
- Raft (vs Paxos)

**Observation**: Rewrites of large systems by tiny teams are powerful. Conway's law and all that.

In general, if something's rewritten in Go or Rust, it's probably faster. Not necessarily because the language is faster (Go is garbage collected!) but because the languages provide the clarity of thought needed to redesign a system, safely, from scratch.

Great counterpoint to this: Joel Spolsky calls rewrites a “[thing you should never do](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/)” because code is not a physical object. It doesn’t get rusty or get clean. While you might have more clarity the second time around, you won’t necessarily have fewer bugs or time consumed. There’s no a priori reason rewrites are good, it’s mostly aesthetic.

## What about virtualization?

JVM, Graal, Flutter/WASM??

See also [[projects.linux-desktop]]

## Misc

Dart, Vala, Kotlin

[Lunatic](https://lunatic.solutions/): an Erlang-inspired runtime for WebAssembly


[[theory.bottom-up]]

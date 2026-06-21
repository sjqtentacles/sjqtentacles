<div align="center">

# Hi, I'm sjqtentacles 🐙

### Programming-language enthusiast and prolific builder — I learn domains by writing libraries, engines, and tools from scratch.

[![Polyglot](https://img.shields.io/badge/polyglot-20%2B%20languages-DE3163?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories)
[![Functional](https://img.shields.io/badge/functional-first-1F6FEB?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories)
[![From scratch](https://img.shields.io/badge/built-from%20scratch-2EA043?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories)
[![Repos](https://img.shields.io/badge/public%20repos-200%2B-8957E5?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories)

</div>

---

## About

I build to understand. Whether it's a cryptographic primitive, a game engine, a parser, or a neural net, I tend to reach for a from-scratch implementation over a black box — usually in whatever language fits the problem best.

That curiosity runs widest through **programming languages** themselves: I'm most at home in functional ones (Standard ML, OCaml, Haskell, Clojure, Scala, Racket, Lisp, Elixir, F#), but happily drop into **Rust, C, Python, Go, and TypeScript** when the job calls for it. The throughline isn't a single stack — it's a habit of taking things apart and rebuilding them cleanly.

<div align="center">

![sjqtentacles' GitHub stats](https://github-readme-stats.vercel.app/api?username=sjqtentacles&show_icons=true&theme=tokyonight)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=sjqtentacles&layout=compact&theme=tokyonight&langs_count=12)

</div>

---

## What I build

- **Languages, parsers & interpreters** — Lisp/Scheme interpreters, parser combinators, regex engines, esolangs, and a from-scratch SQL engine.
- **Game development** — game libraries and prototypes across `raylib` (C), `phaser` (TS/JS), `love2d`, and several hand-rolled engines (ECS, pathfinding, collision, FOV).
- **Machine learning & AI** — learning resources, deep-learning experiments, and an autonomous multi-agent coding agent.
- **Cryptography & Bitcoin** — hashes, ciphers, elliptic curves, signatures, and Bitcoin/Ethereum primitives implemented to spec.
- **Systems & low-level** — codecs, compression, a software-defined acoustic modem, and runtime/tooling work in Rust and C.
- **Classics, languages & writing** — interlinear translations of Latin, Greek, and Old English, plus typesetting and longform writing projects in TeX.

---

## Selected work

A few projects that show the range — across domains and languages:

| Project | What it is |
| --- | --- |
| [open-source-machine-learning-degree](https://github.com/sjqtentacles/open-source-machine-learning-degree) | A free, self-directed ML curriculum — my most-starred project. |
| [forge](https://github.com/sjqtentacles/forge) | An autonomous coding agent built on a multi-agent LangGraph orchestrator. |
| [sonance](https://github.com/sjqtentacles/sonance) | High-performance adaptive acoustic modem in Rust — data over sound (adaptive OFDM, LDPC). |
| [raydial](https://github.com/sjqtentacles/raydial) · [raypals](https://github.com/sjqtentacles/raypals) | `raylib` libraries for dialogue boxes and ready-made 2D/3D sprites (C). |
| [chinalang](https://github.com/sjqtentacles/chinalang) | An esoteric language with Lisp-style macros — a tree-walking interpreter in Go. |
| [the `sml-*` ecosystem](https://github.com/sjqtentacles?tab=repositories&q=sml-) | ~100 zero-dependency Standard ML libraries — see below. |

---

## The Standard ML ecosystem

One of my longest-running threads: a family of **~100 pure-Standard-ML libraries**, each built to a real spec, TDD'd against official RFC/test vectors, and verified to produce **byte-identical** output on both **MLton** and **Poly/ML** with zero or vendored dependencies.

It spans the stack — cryptography & Bitcoin (`sml-secp256k1`, `sml-ed25519`, `sml-sha3`, `sml-bech32`), serialization & parsers (`sml-json`, `sml-cbor`, `sml-parsec`, `sml-packrat`), graphics & media (`sml-glm`, `sml-image`, `sml-raster`), data structures (`sml-graph`, `sml-rope`, `sml-crdt`), numerics (`sml-matrix`, `sml-bigdecimal`, `sml-rational`), and a full web stack (`sml-http`, `sml-router`, `sml-jwt`, `sml-ws`).

> Browse the whole set: **[all `sml-*` repositories →](https://github.com/sjqtentacles?tab=repositories&q=sml-)**

---

## How I like to build

- **From scratch, to spec.** Where a standard exists, I implement against its official test vectors rather than hand-rolled expectations.
- **Determinism over convenience.** Randomness, time, and I/O get pushed to the edges so cores stay pure, reproducible, and testable.
- **Zero / vendored dependencies.** Especially in the library work — every repo should build standalone.
- **Many languages, one set of habits.** New domain or new language, the goal is the same: understand it well enough to rebuild it cleanly.

<div align="center">

*Curious about most things. Building one of them at a time.*

</div>

# sjqtentacles 🐙

I write a lot of code in a lot of languages. Mostly functional ones (Standard ML, OCaml, Haskell, Clojure, Scala, Racket, Lisp, Elixir, F#), but also Rust, C, Python, Go, and TypeScript.

## What I work on

- Languages and parsers: Lisp/Scheme interpreters, parser combinators, regex engines, esolangs, a small SQL engine.
- Games: libraries and prototypes with raylib (C), phaser (TS/JS), love2d, and a few hand-rolled engines (ECS, pathfinding, collision, FOV).
- Machine learning: deep-learning experiments and a multi-agent coding agent.
- Cryptography and Bitcoin: hashes, ciphers, elliptic curves, signatures, Bitcoin/Ethereum primitives.
- Systems: codecs, compression, an acoustic modem (data over sound), tooling in Rust and C.
- Classics and writing: interlinear Latin, Greek, and Old English, plus longform writing in TeX.

## A few projects

- [forge](https://github.com/sjqtentacles/forge) — an autonomous coding agent on a multi-agent LangGraph orchestrator.
- [sonance](https://github.com/sjqtentacles/sonance) — an adaptive acoustic modem in Rust (OFDM, LDPC).
- [raydial](https://github.com/sjqtentacles/raydial) and [raypals](https://github.com/sjqtentacles/raypals) — raylib libraries for dialogue boxes and sprites (C).
- [chinalang](https://github.com/sjqtentacles/chinalang) — an esoteric language with Lisp-style macros; tree-walking interpreter in Go.

## The sml-* libraries

I maintain over 300 pure Standard ML libraries. They cover crypto and Bitcoin (`sml-secp256k1`, `sml-ed25519`, `sml-sha3`, `sml-aead`), parsers and serialization (`sml-json`, `sml-cbor`, `sml-parsec`, `sml-protobuf`), graphics and a self-drawn desktop GUI stack (`sml-canvas2d`, `sml-layout`, `sml-ui`, with `sml-window` opening a real window), data structures (`sml-graph`, `sml-rbtree`, `sml-btree`, `sml-fenwick`, `sml-kdtree`), numerics and science (`sml-matrix`, `sml-complex`, `sml-fft`, `sml-kalman`, `sml-physics`), logic and proofs (`sml-sat`, `sml-bdd`, `sml-smt`, `sml-hm`), audio and music (`sml-music`, `sml-midi`, `sml-synth`, `sml-dsp`), and a web stack (`sml-http`, `sml-router`, `sml-jwt`, `sml-tea`).

They have no external dependencies, run byte-identically on both MLton and Poly/ML, and are tested against the relevant RFC/spec vectors.

[All sml-* repositories →](https://github.com/sjqtentacles?tab=repositories&q=sml-)

<div align="center">

# Hi, I'm sjqtentacles 🐙

### Building a comprehensive, pure-Standard-ML ecosystem — one TDD'd, dual-compiler library at a time.

[![Standard ML](https://img.shields.io/badge/Standard%20ML-pure-DE3163?style=for-the-badge)](https://en.wikipedia.org/wiki/Standard_ML)
[![MLton](https://img.shields.io/badge/MLton-whole--program-1F6FEB?style=for-the-badge)](http://mlton.org/)
[![Poly/ML](https://img.shields.io/badge/Poly%2FML-interactive-2EA043?style=for-the-badge)](https://www.polyml.org/)
[![Dependencies](https://img.shields.io/badge/dependencies-zero%20%2F%20vendored-8957E5?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories&q=sml-)
[![sml-* libraries](https://img.shields.io/badge/sml--*%20libraries-90-FF8C00?style=for-the-badge)](https://github.com/sjqtentacles?tab=repositories&q=sml-)

</div>

---

## About

Making **Standard ML** great again — a growing ecosystem of **90 pure-SML libraries** spanning cryptography, serialization, graphics, web, data structures, and numerics.

- **Pure Standard ML** — no FFI, no external runtime dependencies; everything is either Basis-only or **vendored** in-tree.
- **Dual-compiler** — every library builds and runs identically on **MLton** (whole-program optimizing) and **Poly/ML** (interactive).
- **TDD-first** — exhaustive test suites validated against **RFC / spec test vectors** wherever a standard exists.
- **Deterministic** — byte-identical output across compilers and platforms; randomness is caller-supplied so results are reproducible.

<div align="center">

![sjqtentacles' GitHub stats](https://github-readme-stats.vercel.app/api?username=sjqtentacles&show_icons=true&theme=tokyonight)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=sjqtentacles&layout=compact&theme=tokyonight)

</div>

---

## The `sml-*` library catalog

A curated tour of the **90 pure-Standard-ML libraries**, grouped by what they do. Every link goes to a real repository.

### Cryptography, Bitcoin & Web3

| Library | What it does |
| --- | --- |
| [sml-crypto](https://github.com/sjqtentacles/sml-crypto) | HMAC-SHA256 (RFC 4231), constant-time compare, and signed tokens — verified against RFC vectors |
| [sml-codec](https://github.com/sjqtentacles/sml-codec) | Base64/Base16 (RFC 4648), SHA-1 (RFC 3174), SHA-256 (RFC 6234), CRC-32 |
| [sml-sha3](https://github.com/sjqtentacles/sml-sha3) | Keccak-f[1600] sponge, SHA3-224/256/384/512, SHAKE128/256 XOF, and KMAC |
| [sml-blake3](https://github.com/sjqtentacles/sml-blake3) | BLAKE3 cryptographic hash function |
| [sml-aes](https://github.com/sjqtentacles/sml-aes) | AES block cipher with ECB, CBC, CTR, and GCM modes (FIPS 197) |
| [sml-chacha20](https://github.com/sjqtentacles/sml-chacha20) | ChaCha20-Poly1305 and XChaCha20-Poly1305 AEAD (RFC 8439) |
| [sml-ed25519](https://github.com/sjqtentacles/sml-ed25519) | Ed25519 digital signatures over Edwards25519 (RFC 8032) |
| [sml-x25519](https://github.com/sjqtentacles/sml-x25519) | Curve25519 Diffie-Hellman key exchange (RFC 7748) |
| [sml-secp256k1](https://github.com/sjqtentacles/sml-secp256k1) | ECDSA and Schnorr (BIP-340) signatures over secp256k1 |
| [sml-bech32](https://github.com/sjqtentacles/sml-bech32) | Bech32 and Bech32m encoding with SegwitAddr support (BIP-173/350) |
| [sml-merkle](https://github.com/sjqtentacles/sml-merkle) | Merkle tree construction, root computation, and inclusion proofs |
| [sml-script](https://github.com/sjqtentacles/sml-script) | Bitcoin Script stack-machine interpreter (subset) |
| [sml-utxo](https://github.com/sjqtentacles/sml-utxo) | Bitcoin-style Unspent Transaction Output (UTXO) model |
| [sml-rlp](https://github.com/sjqtentacles/sml-rlp) | Recursive Length Prefix (RLP) encoder/decoder for Ethereum |
| [sml-trie](https://github.com/sjqtentacles/sml-trie) | Merkle Patricia Trie for key-value storage with cryptographic root hashing |

### Serialization & Parsing

| Library | What it does |
| --- | --- |
| [sml-json](https://github.com/sjqtentacles/sml-json) | Self-contained JSON parser + serializer, built on (vendored) sml-parsec |
| [sml-cbor](https://github.com/sjqtentacles/sml-cbor) | CBOR (Concise Binary Object Representation) encoder/decoder (RFC 8949) |
| [sml-msgpack](https://github.com/sjqtentacles/sml-msgpack) | MessagePack binary serialization (spec v2.0) |
| [sml-csv](https://github.com/sjqtentacles/sml-csv) | RFC 4180 CSV/TSV parser and writer with full quoting and escaping |
| [sml-toml](https://github.com/sjqtentacles/sml-toml) | TOML configuration parser (subset of v1.0.0) built on parser combinators |
| [sml-yaml](https://github.com/sjqtentacles/sml-yaml) | Subset YAML 1.2 parser (block + flow, multi-doc) |
| [sml-parsec](https://github.com/sjqtentacles/sml-parsec) | Parser combinators with position tracking and precise error reporting |
| [sml-packrat](https://github.com/sjqtentacles/sml-packrat) | Memoizing PEG (packrat) parser: ordered choice, `&`/`!` predicates, linear-time |

### Compression & Encoding

| Library | What it does |
| --- | --- |
| [sml-inflate](https://github.com/sjqtentacles/sml-inflate) | DEFLATE/zlib/gzip decompression (RFC 1950/1951/1952), CRC-32 + Adler-32 |
| [sml-deflate](https://github.com/sjqtentacles/sml-deflate) | RFC 1951 DEFLATE inflate + RFC 1950/1952 zlib/gzip wrappers |
| [sml-gzip](https://github.com/sjqtentacles/sml-gzip) | gzip (RFC 1952) container codec over DEFLATE/INFLATE with CRC32 verification |
| [sml-lz4](https://github.com/sjqtentacles/sml-lz4) | LZ4 block-format compressor and decompressor (zero dependencies) |
| [sml-hex](https://github.com/sjqtentacles/sml-hex) | Portable hexadecimal encode/decode: strict decoding, mixed-case tolerant |

### Graphics & Media

| Library | What it does |
| --- | --- |
| [sml-glm](https://github.com/sjqtentacles/sml-glm) | Graphics linear algebra: vec2/3/4, mat2/3/4, quaternions, transforms, projections |
| [sml-image](https://github.com/sjqtentacles/sml-image) | Image codecs: decode/encode PNM (PPM/PGM), BMP, TGA, and PNG (RGBA8) |
| [sml-raster](https://github.com/sjqtentacles/sml-raster) | 2D rasterizer: lines, rects, circles, triangles, polygons into RGBA8 images |
| [sml-color](https://github.com/sjqtentacles/sml-color) | Color-space math: sRGB/linear, HSL/HSV, RGBA8 packing, gamma, blending |
| [sml-noise](https://github.com/sjqtentacles/sml-noise) | Procedural noise: Perlin, simplex, value, and worley plus fbm/turbulence |
| [sml-obj](https://github.com/sjqtentacles/sml-obj) | Mesh parsers: Wavefront OBJ/MTL and PLY (ASCII + binary little-endian) |
| [sml-camera](https://github.com/sjqtentacles/sml-camera) | Scene math: transforms (TRS), camera view/projection, frustum culling, ray intersection |

### Game Development

| Library | What it does |
| --- | --- |
| [sml-ecs](https://github.com/sjqtentacles/sml-ecs) | Entity-Component-System architecture with sparse component stores |
| [sml-astar](https://github.com/sjqtentacles/sml-astar) | Generic A* and Dijkstra pathfinding with 2D grid support |
| [sml-collision](https://github.com/sjqtentacles/sml-collision) | 2D AABB, circle, and SAT convex polygon collision detection |
| [sml-fov](https://github.com/sjqtentacles/sml-fov) | Recursive shadowcasting field-of-view and Bresenham line-of-sight |
| [sml-fsm](https://github.com/sjqtentacles/sml-fsm) | Finite state machine and behavior tree for game AI |
| [sml-bsp](https://github.com/sjqtentacles/sml-bsp) | Binary Space Partitioning dungeon generator with rooms and corridors |
| [sml-tween](https://github.com/sjqtentacles/sml-tween) | 30 easing functions and keyframe timeline tweening |

### Data Structures & Algorithms

| Library | What it does |
| --- | --- |
| [sml-graph](https://github.com/sjqtentacles/sml-graph) | Graph algorithms: BFS, DFS, topological sort, SCC, MST, and max-flow |
| [sml-rope](https://github.com/sjqtentacles/sml-rope) | Persistent rope data structure with Fibonacci rebalancing |
| [sml-skiplist](https://github.com/sjqtentacles/sml-skiplist) | Probabilistic skip list ordered map and set functor |
| [sml-pqueue](https://github.com/sjqtentacles/sml-pqueue) | Purely functional priority queue (pairing heap), persistent, O(1) merge |
| [sml-deque](https://github.com/sjqtentacles/sml-deque) | Purely functional double-ended queue (banker's two-list), O(1) amortised |
| [sml-bitset](https://github.com/sjqtentacles/sml-bitset) | Portable packed bit-set: persistent set algebra, popcount, iteration |
| [sml-buffer](https://github.com/sjqtentacles/sml-buffer) | Growable byte/char buffer with rope-style concat |
| [sml-bloom](https://github.com/sjqtentacles/sml-bloom) | Bloom filter with optimal sizing and SHA-256 hashing |
| [sml-crdt](https://github.com/sjqtentacles/sml-crdt) | State-based CRDTs: G-Counter, PN-Counter, LWW-Register, and OR-Set |

### Math & Numerics

| Library | What it does |
| --- | --- |
| [sml-matrix](https://github.com/sjqtentacles/sml-matrix) | Dense linear algebra: multiply, transpose, LU, determinant, solve, inverse, QR |
| [sml-bigdecimal](https://github.com/sjqtentacles/sml-bigdecimal) | Arbitrary-precision decimal arithmetic (Java BigDecimal style) on IntInf |
| [sml-rational](https://github.com/sjqtentacles/sml-rational) | Exact rational-number arithmetic, built on IntInf |
| [sml-complex](https://github.com/sjqtentacles/sml-complex) | Complex numbers: arithmetic, exp/log/sqrt, powers, and polar form |
| [sml-poly](https://github.com/sjqtentacles/sml-poly) | Univariate polynomials over an arbitrary ring via a nesting Poly functor |
| [sml-units](https://github.com/sjqtentacles/sml-units) | Runtime dimensional analysis: dimension-checked quantities over SI base units |
| [sml-prng](https://github.com/sjqtentacles/sml-prng) | Deterministic PRNGs: SplitMix64, xoshiro256, PCG, uniform reals/ranges |
| [sml-random](https://github.com/sjqtentacles/sml-random) | Splittable deterministic PRNG (SplitMix64): tokens, nonces, session IDs |

### Text, Languages & Tooling

| Library | What it does |
| --- | --- |
| [sml-markdown](https://github.com/sjqtentacles/sml-markdown) | CommonMark-subset Markdown parser rendering to an sml-html node tree |
| [sml-rederiv](https://github.com/sjqtentacles/sml-rederiv) | Regex engine via Brzozowski derivatives, with search, replace, bounded quantifiers |
| [sml-diff](https://github.com/sjqtentacles/sml-diff) | Myers O(ND) sequence diff: edit scripts, LCS, edit distance, line diffing |
| [sml-pretty](https://github.com/sjqtentacles/sml-pretty) | Wadler/Leijen pretty-printer combinators (group/nest/line, width-aware) |
| [sml-tui](https://github.com/sjqtentacles/sml-tui) | Pure Elm-architecture terminal UI toolkit: widgets, screen buffer, ANSI |
| [sml-cli](https://github.com/sjqtentacles/sml-cli) | Declarative command-line argument parser with subcommands and auto-help |
| [sml-glob](https://github.com/sjqtentacles/sml-glob) | Shell-style glob matching: `*`, `?`, `[classes]`, ranges, negation, escapes |
| [sml-unicode](https://github.com/sjqtentacles/sml-unicode) | Unicode: UTF-8/UTF-16 codecs, NFC/NFD, case folding, grapheme segmentation |
| [sml-template](https://github.com/sjqtentacles/sml-template) | Logic-light Mustache/Handlebars-style templating with HTML escaping |
| [sml-test](https://github.com/sjqtentacles/sml-test) | Test framework with property-based testing, QuickCheck-style gens, shrinking |
| [sml-lisp](https://github.com/sjqtentacles/sml-lisp) | Small functional Scheme interpreter: closures, IntInf bignums, proper tail calls |
| [sml-sql](https://github.com/sjqtentacles/sml-sql) | Pure in-memory SQL query engine (tokenizer + parser + evaluator) |

### Web & Systems

| Library | What it does |
| --- | --- |
| [sml-web](https://github.com/sjqtentacles/sml-web) | Umbrella web stack: one request→response app wiring router + middleware + sessions |
| [sml-http](https://github.com/sjqtentacles/sml-http) | RFC 9110/9112 HTTP/1.1 message model: parser, chunked + Content-Length framing |
| [sml-router](https://github.com/sjqtentacles/sml-router) | Pure HTTP router: path patterns with `:params` and `*wildcards`, method dispatch |
| [sml-middleware](https://github.com/sjqtentacles/sml-middleware) | Composable handler→handler middleware: compose, error catching, body limits, logging |
| [sml-session](https://github.com/sjqtentacles/sml-session) | Session handling: in-memory and stateless HMAC-signed-cookie backends |
| [sml-cookie](https://github.com/sjqtentacles/sml-cookie) | RFC 6265 Cookie/Set-Cookie parse+build plus HMAC-signed cookies |
| [sml-negotiate](https://github.com/sjqtentacles/sml-negotiate) | RFC 9110 content negotiation: Accept / Accept-Encoding / Accept-Language + q-values |
| [sml-forms](https://github.com/sjqtentacles/sml-forms) | Decode form/query/JSON bodies into typed values via an error-accumulating applicative |
| [sml-html](https://github.com/sjqtentacles/sml-html) | HTML AST with safe-by-default, context-aware escaping (XSS holes are opt-in) |
| [sml-mime](https://github.com/sjqtentacles/sml-mime) | MIME media-type parse/format (RFC 9110), multipart/form-data (RFC 7578) |
| [sml-uri](https://github.com/sjqtentacles/sml-uri) | RFC 3986 URI + x-www-form-urlencoded: percent codec, reference resolution |
| [sml-uuid](https://github.com/sjqtentacles/sml-uuid) | RFC 4122/9562 UUID parse, format, and generate: v4 + v7 |
| [sml-datetime](https://github.com/sjqtentacles/sml-datetime) | Civil date arithmetic: leap years, epoch days, addDays/diffDays, ISO-8601 |
| [sml-jwt](https://github.com/sjqtentacles/sml-jwt) | JSON Web Tokens (JWS) with HMAC-SHA256 (HS256) signing and verification |
| [sml-ws](https://github.com/sjqtentacles/sml-ws) | RFC 6455 WebSockets: handshake, frame encode/decode, fragmentation reassembly |
| [sml-async](https://github.com/sjqtentacles/sml-async) | Portable, deterministic async library: scheduler + futures + async monad |
| [sml-config](https://github.com/sjqtentacles/sml-config) | Typed config from a pure key/value source (env map / dotenv) with coercion |
| [sml-log](https://github.com/sjqtentacles/sml-log) | Leveled structured logging with a pluggable, deterministic default sink |
| [sml-serve](https://github.com/sjqtentacles/sml-serve) | Design doc for the MLton-only socket adapter — the one impure edge of the stack |

> Explore the full set anytime: **[all `sml-*` repositories →](https://github.com/sjqtentacles?tab=repositories&q=sml-)**

---

## Engineering principles

- **TDD-first.** Each library ships with a real test suite. Where a standard exists, tests run against the **official RFC / spec test vectors** rather than hand-rolled expectations.
- **Dual-compiler determinism.** Everything is exercised on both **MLton** and **Poly/ML**, and is expected to produce **byte-identical** output on each.
- **Zero / vendored dependencies.** Libraries depend only on the SML Basis. When code is shared (e.g. `sml-parsec` inside `sml-json`, `sml-inflate` inside `sml-image`), it is **vendored** in-tree so every repo builds standalone.
- **Determinism over convenience.** Randomness, time, and I/O are pushed to the edges; cores are pure functions of their inputs, so results are reproducible and testable.
- **Visual libraries, visual proof.** Graphics/media libraries (`sml-image`, `sml-raster`, `sml-noise`, `sml-color`) produce real image files you can diff and eyeball.

<div align="center">

*Pure functions. Two compilers. One byte-identical answer.*

</div>

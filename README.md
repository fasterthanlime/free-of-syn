# free of syn

[![free of syn](https://img.shields.io/badge/free%20of-syn-hotpink)](https://github.com/fasterthanlime/free-of-syn)

Rid your rust crate of [syn](https://crates.io/crates/syn)!

"free of syn" is a movement — Rust crates shouldn't take forever to build.

And often, the culprit is proc macro crates that pull in heavy dependencies
like [syn](https://crates.io/crates/syn).

## What's the alternative?

Declarative macros (much faster, and cacheable!) may be more capable than
you realize!

  * Read [The Little Book of Rust Macros](https://veykril.github.io/tlborm/)

If you _have_ to use proc macros, then you may be interested in
[unsynn](https://crates.io/crates/unsynn), which allows writing proc-macro
parsers without heavy dependencies.

## Enforce it in CI

To make sure your crate is free of syn, run the provided `absolve.sh` script
in your CI pipeline.

Here's just the badge, as ANSI escapes:

```raw
\033[38;2;255;255;255;48;2;0;0;0m free of \033[38;2;255;255;255;48;2;255;105;180m syn \033[38;2;255;255;255;48;2;0;0;0m\033[0m
```

It renders as:

![example ANSI/terminal badge rendering](https://github.com/user-attachments/assets/67477769-7050-466b-ac03-9477349d50c7)

Alternatively, the [`cargo-deny`](https://github.com/EmbarkStudios/cargo-deny)
plugin lets you ban arbitrary crates.

## Spread the word

If you have a crate that's free of syn, you can display your support for
the "free of syn" campaign with a badge:

```markdown
[![free of syn](https://img.shields.io/badge/free%20of-syn-hotpink)](https://github.com/fasterthanlime/free-of-syn)
```

![example badge rendering in the facet readme](https://github.com/user-attachments/assets/e2b66ad5-04cd-430b-b30c-68201149e9a8)

## Hall of fame

These projects are free of syn (submit a PR to add yours):

  * [facet](https://github.com/facet-rs/facet) is a reflection and serialization/deserialization framework for Rust
  * [xmacro/xmacro_lib](https://docs.rs/xmacro_lib/latest/xmacro_lib/) Proc-Macro engine for templating rust code
  * [mident](https://github.com/ArcaneNibble/mident) is a toolbox for creating and manipulating identifiers in declarative macros
  * [eager2](https://github.com/Daniel-Aaron-Bloom/eager2) is a framework for eager macro expansion
  * [maybe_special](https://github.com/pypylia/maybe_special) is an attribute macro to automatically generate target feature specialisations.
  

# `foil`: paired performance benchmarking for R packages

[![build-status](https://github.com/VisruthSK/foil-ISC-2026/actions/workflows/publish-proposal.yaml/badge.svg)](https://github.com/VisruthSK/foil-ISC-2026/actions/workflows/publish-proposal.yaml)

This proposal is for an [R Consortium](https://www.r-consortium.org) ISC grant to extend [`foil`](https://github.com/VisruthSK/foil/), a Rust CLI for detecting performance regressions.

`foil` compares baseline and candidate revisions using randomized paired runs on the same machine, preserving the paired experimental design in its statistical analysis and reporting estimated performance changes with uncertainty. The proposed work will add memory measurement on Linux and Windows, prebuilt binaries for Linux, macOS, and Windows, and an R package for installing and configuring `foil`, reading results, and interpreting performance changes.

The goal is to make revision-level performance testing practical on ordinary development and CI infrastructure. `foil` is designed to be flexible and provide developers with the information they need to make decisions about performance.

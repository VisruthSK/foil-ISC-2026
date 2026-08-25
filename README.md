# `foil`: paired performance benchmarking for R packages

[![build-status](https://github.com/VisruthSK/foil-ISC-2026/actions/workflows/publish-proposal.yaml/badge.svg)](https://github.com/VisruthSK/foil-ISC-2026/actions/workflows/publish-proposal.yaml)

This proposal is for an [R Consortium](https://www.r-consortium.org) ISC grant to extend `foil`, a Rust CLI for detecting performance regressions, into a practical benchmarking workflow for R package maintainers.

`foil` compares baseline and candidate revisions using randomized paired runs on the same machine, preserving the paired experimental design in its statistical analysis and reporting estimated performance changes with uncertainty. The proposed work will add OS level peak-memory measurement for process trees on Linux and Windows, prebuilt binaries for Linux, macOS, and Windows, and an R package for installing and configuring `foil`, reading results, and interpreting performance changes.

The goal is to make revision-level performance testing practical on ordinary development and CI infrastructure, including workloads whose memory use occurs in compiled libraries, native extensions, or child processes and is therefore not fully represented by R-level allocation measurements. `foil` is designed to be flexible and provide maintainers with the information they need to make decisions about performance.

<!-- From the command line, run `quarto publish gh-pages isc-proposal.qmd`.  After this, the GitHub action should run every time you push a commit to the main branch. Your rendered proposal can then be viewed at https://VisruthSK.github.io/foil-ISC-2026/ -->

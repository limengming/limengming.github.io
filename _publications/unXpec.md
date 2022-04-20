---
title: "unXpec: Breaking Undo-based Safe Speculation"
collection: publications
permalink: /publication/unXpec
excerpt: '<div align="middle"><img align="middle" style="max-width: 540px; width: 100%" src="https://limengming.github.io/files/unXpec_figure.png" /></div> 
In this paper, we present unXpec as the first attack against Undo-based safe speculation. It exploits the secret-dependent timing channel exhibited through the rollback operations of Undo defenses. Specifically, the rollback process requires both invalidating cache lines brought into the cache by transient instructions and restoring evicted cache lines from the cache by transiently loaded data. This opens up a channel that encodes secret via the timing difference between when rollback involves much invalidation and restoration or not. We further leverage eviction sets to enforce more restoration operations. This yields a longer rollback time and thus a larger secret-dependent timing difference. We demonstrate the timing channel over the open-source CleanupSpec, a representative Undo solution. A single transient load can trigger a secret-dependent timing difference of 22 cycles (without eviction sets) of 32 cycles (with eviction sets), which is sufficiently exploitable for constructing a covert channel for speculative execution attacks. We run unXpec on the gem5 simulator with CleanupSpec enabled. The results show that unXpec can leak secrets at a high rate of 140Kbps with an accuracy over 90%. Simply enforcing constant-time rollback to mitigate unXpec may induce an over 70%.
date: 2022-04-05
venue: 'The 28th IEEE International Symposium on High-Performance Computer Architecture (HPCA)'
paperurl: 'https://limengming.github.io/publications/unXpec.pdf'
---

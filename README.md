This repository hosts code and data related to the paper titled [Minimal Subgroups of GL<sub>2</sub>(Z<sub>S</sub>)](https://arxiv.org/abs/2402.11049) by Harris B. Daniels and Jeremy Rouse, arXiv:2402.11049 (2024).

The directory structure is organized as follows:

**Ancestor:** This directory contains Magma code for computing the labels of all supergroups of a given subgroup of GL<sub>2</sub>(Z<sub>2</sub>).

**Aux Files:** Here you will find Magma code and data sourced from other papers used in our computations. Specifically, it includes:

`gl2.m`
`gl2data.m`
`gl2_big2adic`

These files originate from [ell-adic images of Galois for elliptic curves over Q](https://arxiv.org/abs/2106.11141) by Jeremy Rouse, Andrew V. Sutherland, and David Zureick-Brown, cited as [15] in our paper.

**Minimal Group Search:** The subdirectory **Found Groups** contains scripts dedicated to identifying minimal groups at various levels that are powers of 2. The file `minsearch.txt` is a `Magma` script that, given a positive integer n, finds subgroups of GL<sub>2</sub>(Z/2<sup>n</sup> Z) whose full preimage in GL<sub>2</sub>(Z<sub>2</sub>) is minimal. This script was run for n = 3 to n = 7 and the outputs are in the files `minfound3.txt`, `minfound4.txt`, …, `minfound7.txt`. (The file `minfoundn.txt` is formatted as a `Magma` script the specifies a tuple “subs” consisting of all of the minimal groups of level <= 2<sup>n</sup>.)  

The folder **Logs** houses the corresponding log files from these searches. The file `Genus0MinimalGroups.m` includes the Magma code needed to compute the models of the genus 0 minimal groups that appear in Section 5 of the paper.

**Plentiful:** This directory holds the code which does the calculation mentioned in the final paragraph of the proof of Theorem 4.2. In particular, it shows that for each pair (A,B) of matrices in GL<sub>2</sub>(Z/4Z)<sup>2</sup>, the power series d defined in the paper is nonzero.    

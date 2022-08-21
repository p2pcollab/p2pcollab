---
title: OCaml-P2P
subtitle: P2P protocols and algorithms in OCaml
---

# Design

The libraries here implement parts of the design described in:

[UPSYCLE: Ubiquitous Publish-Subscribe Infrastructure for Collaboration on Edge Networks](https://lofi.re/design/upsycle)

# P2P gossip-based protocols

## PolderCast

P2P topic-based pub/sub ([paper](https://hal.inria.fr/hal-01555561),
[code](https://github.com/p2pcollab/ocaml-p2p))\
Privacy enhancements: instead of transmitting node profiles with
full subscription sets in the clear, randomized Bloom filters using
BLIP are employed together with a Bloom filter-based Private Set
Intersection (BFPSI) protocol

## RingCast

P2P hybrid dissemination
([paper](https://www.distributed-systems.net/my-data/papers/2007.mw.pdf),
[code](https://github.com/p2pcollab/ocaml-p2p))

## VICINITY

P2P clustering & topology management
([paper](https://hal.inria.fr/hal-01480790/document),
[code](https://github.com/p2pcollab/ocaml-p2p))

## CYCLON

Random Peer Sampling
([paper](https://www.distributed-systems.net/my-data/papers/2005.jnsm.pdf),
[code](https://github.com/p2pcollab/ocaml-p2p))\
To ensure uniformity of peer sampling, URPS is used together with
CYCLON.

## TAPS

Trust-Aware Peer Sampling
([paper](https://tel.archives-ouvertes.fr/tel-01135867/file/JEGOU_Arnaud.pdf),
[code](https://github.com/p2pcollab/ocaml-p2p))\

## TAC

Trust-Aware Clustering
([paper](https://tel.archives-ouvertes.fr/tel-01135867/file/JEGOU_Arnaud.pdf),
[code](https://github.com/p2pcollab/ocaml-p2p))\

# P2P data structures

## URPS

Uniform Random Peer Sampler
([paper](https://hal.archives-ouvertes.fr/hal-00804430),
[code](https://github.com/p2pcollab/ocaml-urps))

## BLIP

Non-interactive differentially-private similarity computation on
Bloom filters
([paper](https://scholar.google.com/scholar?cluster=16665581281970888&hl=en),
[slides](https://malaggan.com/AGK2012.pdf),
[code](https://github.com/p2pcollab/ocaml-blip))

## BFPSI

Private Set Intersection based on Bloom filters
([paper](https://eprint.iacr.org/2013/620),
[code](https://github.com/p2pcollab/ocaml-psi))

# Transport

## NoiseSocket

Encoding layer for the Noise Protocol Framework
([spec](https://noisesocket.org/spec/noisesocket/),
[code](https://github.com/p2pcollab/ocaml-noise-socket))

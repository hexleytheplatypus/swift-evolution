# Modernize Hashable

* Proposal: [SE-NNNN](0000-seeded-hashable.md)
* Authors: [C. Heath](https://github.com/hexleytheplatypus)
* Review Manager: TBD
* Status: **Awaiting implementation** or **Awaiting review**
* Implementation: [apple/swift#NNNNN](https://github.com/apple/swift/pull/NNNNN) or [apple/swift-evolution-staging#NNNNN](https://github.com/apple/swift-evolution-staging/pull/NNNNN)
* Upcoming Feature Flag: *if applicable* `MyFeatureName`
* Review: ([pitch](https://forums.swift.org/...))

## Introduction

Modernize Hashable for simplicity with swift-crypto and explicity seeded Hasher
instances for networked usage.

## Motivation

Todo

## Proposed solution

Unifying Hashing across Swift (Cryptographic and Non-Cryptographic expressed in stdlib)
- `Hasher` becomes `SipHasher` (typealiased to `DefaultHasher`)
- `Hasher` now becomes a protocol equivalent to [`swift-crypto.HashFunction`] (https://developer.apple.com/documentation/cryptokit/hashfunction)

Allowing Hasher to be Seeded (Especially useful for Networking/Distributed Actor Clusters)
- `Hasher` gains `init(seed: Digest)`

## Detailed design

Todo

## Source compatibility

Todo - since this would be source breaking, our solution should be new diagnostics for Fix-It's

## ABI compatibility

Todo

## Implications on adoption

Todo

## Future directions

Todo

## Alternatives considered

Todo

## Acknowledgments

Todo

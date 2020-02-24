# RFC-0001: Generic Actions (GAs) Tooling

<dl>
  <dt>Author</dt>
  <dd>Jordan Ellis</dd>

  <dt>RFC pull request</dt>
  <dd><a href="URL">URL</a></dd>

  <dt>Date of submission</dt>
  <dd>2020-02-24</dd>

  <dt>Date of approval</dt>
  <dd>YYYY-MM-DD</dd>

  <dt>Approved by</dt>
  <dd>First Person, Second Person</dd>
</dl>

## Summary

Adding GA plugins within Alchemy currently has the following problems:  
- No UI for configuring & deploying a new GA plugin contract, must be done by a skilled programmer.
- No UI for knowing what types of GAs Alchemy supports (ENS Registrar, Uniswap, etc).
- No UI for creating new types of GAs that Alchemy can support (Compound, etc).
- - Must be PR'd into Alchemy for them to be usable.
- Complex UI for adding a GA plugin to the DAO via the plugin manager.
- Subgraph does not pickup on newly deployed GA plugin contracts.

## Goals & Motivation

Allow anyone (not just programmers) to be able to...
1. Add new GAs to their DAO (ENS management, Uniswap, etc)
2. Add new types of GAs to the "known GA" list (Compound, PoolTogether, etc)

## Urgency

I view this as hyper urgent, as the main users of Alchemy (dOrg, dxDAO, NecDAO, Fest DAO, Genesis) want to do more with their DAOs and evolve how they operate. This requires being able to easily add new Generic Actions to their DAOs set of capabilities.

## Terminology

GA Creator: TODO UI for deploying new generic action contracts (from known GAs)
GA Factory: TODO factory contract that spawns new generic action contracts (needed until arc-hives is live)
GA Designer: TODO UI for defining new generic actions
GA Registry: TODO on-chain registry of Generic Action JSONs, managed by the Alchemy DAO

## Detailed Design

This is the main section of the RFC. What does the proposal include? What are
the proposed interfaces/APIs? How are different affected parties, such as users,
developers or node operators affected by the change and how are they going to
use it?

## Compatibility

No breaking changes.

## Drawbacks and Risks

Nothing identifiable.

## Alternatives

Nothing currently.

## Open Questions

What are unresolved questions?

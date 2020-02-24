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
  - Must be PR'd into Alchemy for them to be usable.
- Complex UI for adding a GA plugin to the DAO via the plugin manager.
- Subgraph does not pickup on newly deployed GA plugin contracts.

## Goals & Motivation

Allow anyone (not just programmers) to be able to...
1. Add new GAs to their DAO (ENS management, Uniswap, etc)
2. Add new types of GAs to the "known GA" list (Compound, PoolTogether, etc)

## Urgency

I view this as hyper urgent, as the main users of Alchemy (dOrg, dxDAO, NecDAO, Fest DAO, Genesis) want to do more with their DAOs and evolve how they operate. This requires being able to easily add new Generic Actions to their DAOs set of capabilities.

## Terminology

**GA Creator**: UI for configuring & deploying new generic action plugins from within Alchemy. Deployment via the UI will (1) deploy a new GA plugin contract via the ***GA Factory*** and (2) call create a proposal in the DAO's Plugin Manager to add the new GA plugin.  
**GA Factory**: Contract factory that spawns new GA plugin contracts. This is needed until Arc-Hives is live.  
**GA Designer**: UI for defining new generic actions (Compound, Uniswap, Moloch, etc). The UI will be a front-end for defining [GA JSON files](https://github.com/daostack/alchemy/tree/dev/src/genericSchemeRegistry/schemes), and proposing them to the ***GA Registry***.  
**GA Registry**: On-chain registry of GA JSONs. This registry should be managed by a DAO made up by the stake-holders of Alchemy. The Alchemy DAO.  
**Known GA**: A Generic Action that's registered in the registry.  

## Detailed Design

TODO: detail each user flow in the "Goals & Motivations" section, and illustrate each change needed in the stack.  

## Compatibility

No breaking changes.

## Drawbacks and Risks

Nothing identifiable.

## Alternatives

Nothing currently.

## Open Questions

What are unresolved questions?

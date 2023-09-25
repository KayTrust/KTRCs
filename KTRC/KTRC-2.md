---
ktrc: 2
title: KTRC Editor Handbook
description: Organizational structure, decision making process, and other KTRC Editor odds and ends.
author: original authors Pooja Ranjan (@poojaranjan), Gavin John (@Pandapip1), Sam Wilson (@SamWilsn), et al.
discussions-to: https://ethereum-magicians.org/t/pr-5069-eip-editor-handbook/9137
status: Living
type: Meta
created: 2023-09-06
requires: 1
---

## Introduction

We, the KayTrust Request for Comments (KTRC) Editors, maintain a repository of documents related to the KayYTrust asset and its ecosystem. Consider us both _archivists_ making sure the community as a whole does not lose its history, and a _publisher_ making sure interested parties can stay up-to-date with the latest proposals.

## Mission

### What we Do

Our mission is to serve the KayTrust community, both present and future, by:

 - **Publishing Proposals**: Making proposals, including their history and associated discussions available over the long term at no cost.
    
    By doing so, we foster transparency and ensure that valuable insights from past proposals are accessible for future decision-making and learning.
 - **Facilitating Discussion**: Providing a forum for discussing proposals open to anyone who wants to participate civilly.
    
    By encouraging open dialogue and collaboration, we aim to harness the collective knowledge and expertise of the KayTrust community in shaping proposals.
 - **Upholding Quality**: Upholding a measure of minimally-subjective quality for each proposal as defined by its target audience.

    By adhering to defined criteria, we promote the development of high-quality and relevant proposals that drive the evolution of KayTrust.

### What we Don't

On the other hand, we do _not_:

 - **Decide Winners**: If there are multiple competing proposals, we will publish all of them. We are not in the business of deciding what is the right path for KayTrust, nor do we believe that there is One True Way to satisfy a need.

 - **Assert Correctness**: While we might offer technical feedback from time to time, we are not experts nor do we vet every proposal in depth. Publishing a proposal is not an endorsement or a statement of technical soundness.

 - **Manage**: We do not track implementation status, schedule work, or set due dates or contents.

 - **Track Registries**: We want all proposals to eventually become immutable, but a registry will never get there if anyone can keep adding items. To be clear, exhaustive and/or static lists are fine. 
 - **Provide Legal Advice**: Trademarks, copyrights, patents, prior art, and other legal matters are the responsibility of authors and implementers, not KTRC Editors. We are not lawyers, and while we may occasionally make comments touching on these areas, we cannot guarantee any measure of correctness.

Documenting all of the things we would not do is impossible, and the above are just a few examples. We reserve the right to do less work whenever possible!

## Structure

### KTRC Editors

We, the Editors, consist of some number of KTRC Editors and one Keeper of Consensus (or just Keeper for short) elected by and from the KTRC Editors.

KTRC Editors are responsible for governing the KTRC process itself, electing a Keeper, and stewarding proposals.

The Keeper's two responsibilities (on top of their KTRC Editor duties) are: to determine when rough consensus has been reached on a matter, and determine when/if it is appropriate to re-open an already settled matter.

## Membership

Anyone may apply to join as an KTRC Editor. Specific eligibility requirements are left to individual current KTRC Editors, but the general requirements are:

 - A strong belief in the above mission;
 - Proficiency with English (both written and spoken);
 - Reading and critiquing KTRC;
 - Participation in governance.

KTRC Editors are expected to meet these requirements throughout their tenure, and not doing so is grounds for removal. Any member may delegate some or all of their responsibilities/powers to tools and/or to other people.

## Making Decisions

### Informally

For decisions that are unlikely to be controversial —especially for decisions affecting a single proposal— an KTRC Editor may choose whatever option they deem appropriate in accordance with our mission.

### Formally

Electing a Keeper, adding/removing KTRC Editors, and any possibly-controversial decisions must all be made using variations of this formal process.

#### Preparation

##### Call for Input

For any matter requiring a decision, a call for input must be published in writing to the usual channels frequented by KTRC Editors.

##### Quorum

Within 7 days of the call for input, to establish a valid quorum, all KTRC Editors must express their opinion, vote (where appropriate), or lack thereof on the matter under consideration.

After 7 days from the call for input, if not all KTRC Editors have responded, the quorum is reduced to the Editors that have responded. This deadline may be extended in exceptional situations.

#### Deciding

##### Electing a Keeper of Consensus

Any KTRC Editor can call for an election for Keeper. Business continues as usual while the election is running. The KTRC Editor with the most votes once quorum is met is named Keeper until the next election completes. If there is a tie, we'll randomly choose between the KTRC Editors with the most votes, using a fair and agreed upon method (for example, a coin toss over a video call or a commit/reveal game of rock paper scissors.)

##### Adding an KTRC Editor

An KTRC Editor is added once quorum is met, provided the candidate consents and no current KTRC Editor objects.

##### Removing an KTRC Editor

An KTRC Editor is forcibly removed once quorum is met, provided no current KTRC Editor (aside from the one being removed) objects. An KTRC Editor may voluntarily leave their position at any time.

If the departing Editor was also the Keeper, an election for a new Keeper begins immediately.

##### Other Decisions

All other decisions are made through a "rough consensus" process. This does not require all KTRC Editors to agree, although this is preferred. In general, the dominant view of the Editors shall prevail. Dominance, in this process, is not determined by persistence or volume but rather a more general sense of agreement. Note that 51% does not mean "rough consensus" has been reached, and 99% is better than rough. It is up to the Keeper to determine if rough consensus has been reached. Every KTRC Editor is entitled to have their opinion heard and understood before the Keeper makes that determination.

No one, not the KTRC Editors and certainly not the Keeper, holds veto powers (except when adding/removing an Editor as defined above.) It is imperative that the KTRC process evolve, albeit cautiously.

_This section has been adapted from [RFC 2418] and [EIP 5069]._

## Copyright

Copyright and related rights ***TBD***.

[RFC 2418]: https://www.rfc-editor.org/rfc/rfc2418
[EIP 5069]: https://eips.ethereum.org/EIPS/eip-5069

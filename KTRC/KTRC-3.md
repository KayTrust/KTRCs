---
ktrc: 3
title:  KayWallet Contribution Guidelines
description: KayWallet Contributions Guidelines for all KTRC KayWallet editor.
author: David A., Juan José Miranda
discussions-to: Internal
status: Draft
type: Meta
created: 2023-09-24
updated: 2023-09-25
requires: KTRC-1
---

## Abstract
This KTRC will contain all the guidelines to take into account when contributing to the KayWallet source code. If you are a KayWaller developer please take all of these guidelines into account.

## Motivation
Document as clearly as possible all the guidelines to take into account to contribute to the KayWallet source code.

## Specification
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 and RFC 8174.

KayWallet now is a hybrid mobile app.

### One codebase, multiple wallets
Goal: minimize development efforts.
 - All wallets are built from a single codebase
 - Feature-flag mechanism to tune the behaviour. Example: disable certain actions
 - Branding mechanism to personalize the texts and visual style

### Pull requests welcome
Any team can contribute new features or fixes via pull requests.
A pull request must be associated to a task inside an approved User Story, itself associated to an approved Feature.
Core team is responsible for accepting and integrating them.
Guidelines for PRs. For example:
 - Balance between functionality and added weight (app size, responsiveness, UX complexity, restricted device compatibility etc.)
 - Consistency with app's goals. Example: no weather forecast features. No centralization. Etc.
 - Consistency with app's User Experience and User Interface guidelines
 - Code quality
 - Code consistency: use existing dependencies and mechanisms, don't do the same thing in different ways
 - Optionality: will everyone need it? If not, integrate with feature-flag mechanism

## Rationale
Does not apply, is like Motivation for this KTRC.

## Backwards Compatibility

<!--

  This section is optional.

  All KTRCs that introduce backwards incompatibilities must include a section describing these incompatibilities and their severity. The KTRC must explain how the author proposes to deal with these incompatibilities. KTRC submissions without a sufficient backwards compatibility treatise may be rejected outright.

  The current placeholder is acceptable for a draft.

  TODO: Remove this comment before submitting
-->

No backward compatibility issues found.

## Test Cases
As far as possible, all new features implemented in KayWallet should have a list of test cases.

## Reference Implementation
This section is optional.

The Reference Implementation section should include a minimal implementation that assists in understanding or implementing this specification. It should not include project build files. The reference implementation is not a replacement for the Specification section, and the proposal should still be understandable without it.
If the reference implementation is too large to reasonably be included inline, then consider adding it as one or more files in `../assets/ktrc-####/`. External links will not be allowed.

## Security Considerations
All KTRCs must contain a section that discusses the security implications/considerations relevant to the proposed change. Include information that might be important for security discussions, surfaces risks and can be used throughout the life cycle of the proposal. For example, include security-relevant design decisions, concerns, important discussions, implementation-specific guidance and pitfalls, an outline of threats and risks and how they are being addressed. KTRC submissions missing the "Security Considerations" section will be rejected. An KTRC cannot proceed to status "Final" without a Security Considerations discussion deemed sufficient by the reviewers.

## Copyright

Copyright and related rights waived via [license](../LICENSE.md).

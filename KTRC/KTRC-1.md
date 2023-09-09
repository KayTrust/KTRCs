---
eip: 1
title: KTRC Purpose and Guidelines
status: Living
type: Meta
author: Juan José Miranda <jmirandd@nttdata.com>, David Ammouial <dammouia@nttdata.com>, et al.
created: 2023-08-27
---

What is an KTRC?
----------------

KTRC stands for KayTrust Request for Comments. An KTRC is a design document providing information to the KayTrust community, or describing a new feature for KayTrust asset or its processes or environment. The KTRC should provide a concise technical specification of the feature and a rationale for the feature. The KTRC author is responsible for building consensus within the community and documenting dissenting opinions.

KTRC Rationale
--------------------------------------------------------------------

We intend KTRCs to be the primary mechanisms for proposing new features, for collecting community technical input on an issue, and for documenting the design decisions that have gone into kayTrust asset. Because the KTRCs are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.

For KayTrust implementers, KTRCs are a convenient way to track the progress of their implementation. Ideally each implementation maintainer would list the KTRCs that they have implemented. This will give end users a convenient way to know the current status of a given implementation or library.

KTRC Types
------------------------------------------------------------

There are three types of KTRC:

-   A Standards Track KTRC describes any change that affects most or all KayTrust implementations, such as---a change to the KayWallet feature, a change in supporting new DLTs for trust layer, proposed application standards/conventions, or any change or addition that affects the interoperability of applications using KayTrust. Standards Track KTRCs consist of three parts---a design document, an implementation, and (if warranted) an update to the formal specifications. Furthermore, Standards Track KTRCs can be broken down into the following categories:
    -   Core: improvements requiring integrate or modify industry standards (e.g. when are availables), as well as changes that are not necessarily critical but may be relevant to main features of the asset in general (e.g. when are availables).
    -   Provider: improvements requiring a new libraries or base software (e.g. when are availables), as well as changes that are not necessarily critical but may be relevant to main features in KayTrust Provider or APIs (Storage, Issuer, DID, Blockchain, Verifier) (e.g. when are availables).
    -   KayDev: improvements requiring a new libraries or base software (e.g. when are availables), as well as changes that are not necessarily critical but may be relevant to main features in KayDev libraries.
    - KayWallet: improvements requiring a new libraries (e.g. when are availables), as well as changes that are not necessarily critical but may be relevant to main features in KayWallet.
-   A Meta KTRC describes a process surrounding KayTrust asset or proposes a change to (or an event in) a process. Process KTRCs are like Standards Track KTRCs but apply to areas other than the KayTrust asset itself. They may propose an implementation, but not to KayTrust's codebase; they often require community consensus; unlike Informational KTRCs, they are more than recommendations, and users are typically not free to ignore them. Examples include procedures, guidelines, changes to the decision-making process, and changes to the tools or environment used in KayTrust development. Any meta-KTRC is also considered a Process KTRC.

-   An Informational KTRC describes an KayTrust design issue, or provides general guidelines or information to the KayTrust community, but does not propose a new feature. Informational KTRCs do not necessarily represent KayTrust community consensus or a recommendation, so users and implementers are free to ignore Informational KTRCs or follow their advice.

It is highly recommended that a single KTRC contain a single key proposal or new idea. The more focused the KTRC, the more successful it tends to be. A change to one client doesn't require an KTRC; a change that affects multiple clients, or defines a standard for multiple apps to use, does.

An KTRC must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement. The proposed implementation, if applicable, must be solid and must not complicate the asset unduly.

### Special requirements for Core KTRCs

If a Core KTRC mentions or proposes changes ***TBD***, consider this:
-  TBD
-  TBD
-  End list

[](#work-flow) KTRC Work Flow
--------------------------------------------------------------------

### [](#shepherding-an-KTRC) Shepherding an KTRC

Parties involved in the process are you, the champion or *KTRC author*, the [*KTRC editors*](#KTRC-editors), and the [*KayTrust Core Developers*](https://kaytrust.id/devs).

Before you begin writing a formal KTRC, you should vet your idea. Ask the KayTrust community first if an idea is original to avoid wasting time on something that will be rejected based on prior research. It is thus recommended to open a discussion thread on [Wiki pages](https://wiki.kaytrust.id/) to do this. ***TBD***

Once the idea has been vetted, your next responsibility will be to present (by means of an KTRC) the idea to the reviewers and all interested parties, invite editors, developers, and the community to give feedback on the aforementioned channels. You should try and gauge whether the interest in your KTRC is commensurate with both the work involved in implementing it and how many parties will have to conform to it. For example, the work required for implementing a Core KTRC will be much greater than for other KTRC and the core KTRC will need sufficient interest from the KayTrust different teams. Negative community feedback will be taken into consideration and may prevent your KTRC from moving past the Draft stage.

### [](#core-KTRCs) Core KTRCs

For Core KTRCs, given that they require client implementations to be considered Final (see "KTRCs Process" below), you will need to either provide an implementation for clients or convince clients to implement your KTRC.

The best way to get client implementers to review your KTRC is to present it on an AllCoreDevs call. You can request to do so by posting a comment linking your KTRC on an [Global channels for KayTrust Community](https://aver.cual.es.tbd).

The AllCoreDevs call serves as a way for client implementers to do three things. First, to discuss the technical merits of KTRCs. Second, to gauge what other SSI products and assets will be implementing. Third, to coordinate KTRC implementation for future upgrades.

These calls generally result in a "rough consensus" around what KTRCs should be implemented. This "rough consensus" rests on the assumptions that KTRCs are not contentious enough to cause an asset fork and that they are technically sound.

:warning: The KTRCs process and AllCoreDevs call were not designed to address contentious non-technical issues, but, due to the lack of other ways to address these, often end up entangled in them. This puts the burden on KayTrust implementers to try and gauge community sentiment, which hinders the technical coordination function of KTRCs and AllCoreDevs calls. If you are shepherding an KTRC, you can make the process of building community consensus easier by making sure that [Wiki pages](https://wiki.kaytrust.id/) ***TBD*** thread for your KTRC includes or links to as much of the community discussion as possible and that various stakeholders are well-represented.

*In short, your role as the champion is to write the KTRC using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea.*

### [](KTRC-process) KTRC Process

The following is the standardization process for all KTRCs in all tracks:

![KTRC Status Diagram](../assets/KTRC-1/KTRC-process-update.jpg)

Idea - An idea that is pre-draft. This is not tracked within the KTRC Repository.

Draft - The first formally tracked stage of an KTRC in development. An KTRC is merged by an KTRC Editor into the KTRC repository when properly formatted.

Review - An KTRC Author marks an KTRC as ready for and requesting Peer Review.

Last Call - This is the final review window for an KTRC before moving to `Final`. An KTRC editor will assign `Last Call` status and set a review end date (`last-call-deadline`), typically 14 days later.

If this period results in necessary normative changes it will revert the KTRC to `Review`.

Final - This KTRC represents the final standard. A Final KTRC exists in a state of finality and should only be updated to correct errata and add non-normative clarifications.

A PR moving an KTRC from Last Call to Final SHOULD contain no changes other than the status update. Any content or editorial proposed change SHOULD be separate from this status-updating PR and committed prior to it.

Stagnant - Any KTRC in `Draft` or `Review` or `Last Call` if inactive for a period of 6 months or greater is moved to `Stagnant`. An KTRC may be resurrected from this state by Authors or KTRC Editors through moving it back to `Draft` or it's earlier status. If not resurrected, a proposal may stay forever in this status.

> *KTRC Authors are notified of any algorithmic change to the status of their KTRC*

Withdrawn - The KTRC Author(s) have withdrawn the proposed KTRC. This state has finality and can no longer be resurrected using this KTRC number. If the idea is pursued at later date it is considered a new proposal.

Living - A special status for KTRCs that are designed to be continually updated and not reach a state of finality. This includes most notably KTRC-1.

[](#what-belongs-in-a-successful-KTRC) What belongs in a successful KTRC?
-----------------------------------------------------------------------------------------------------------

Each KTRC should have the following parts:

-   Preamble - RFC 822 style headers containing metadata about the KTRC, including the KTRC number, a short descriptive title (limited to a maximum of 44 characters), a description (limited to a maximum of 140 characters), and the author details. Irrespective of the category, the title and description should not include KTRC number. See [below](#KTRC-header-preamble) for details.
-   Abstract - Abstract is a multi-sentence (short paragraph) technical summary. This should be a very terse and human-readable version of the specification section. Someone should be able to read only the abstract to get the gist of what this specification does.
-   Motivation *(optional)* - A motivation section is critical for KTRCs that want to change the KayTrust asset. It should clearly explain why the existing specification or feature is inadequate to address the problem that the KTRC solves. This section may be omitted if the motivation is evident.
-   Specification - The technical specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow competing, interoperable implementations for any of the current integrations.
-   Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other DLTs/blockchain platforms. The rationale should discuss important objections or concerns raised during discussion around the KTRC.
-   Backwards Compatibility *(optional)* - All KTRCs that introduce backwards incompatibilities must include a section describing these incompatibilities and their consequences. The KTRC must explain how the author proposes to deal with these incompatibilities. This section may be omitted if the proposal does not introduce any backwards incompatibilities, but this section must be included if backward incompatibilities exist.
-   Test Cases *(optional)* - Test cases for an implementation are mandatory for KTRCs that are affecting core features changes. Tests should either be inlined in the KTRC as data (such as input/expected output pairs, or included in `../assets/KTRC-###/<filename>`. This section may be omitted for non-Core proposals.
-   Reference Implementation *(optional)* - An optional section that contains a reference/example implementation that people can use to assist in understanding or implementing this specification. This section may be omitted for all KTRCs.
-   Security Considerations - All KTRCs must contain a section that discusses the security implications/considerations relevant to the proposed change. Include information that might be important for security discussions, surfaces risks and can be used throughout the life-cycle of the proposal. E.g. include security-relevant design decisions, concerns, important discussions, implementation-specific guidance and pitfalls, an outline of threats and risks and how they are being addressed. KTRC submissions missing the "Security Considerations" section will be rejected. An KTRC cannot proceed to status "Final" without a Security Considerations discussion deemed sufficient by the reviewers.
-   Copyright Waiver - Not all KTRCs be in the public domain, probably only the KTRC type Standard/KayDev. For this KTRC type Standard/KayDev, ***TBD*** the copyright waiver MUST link to the license file and use the following wording: `Copyright and related rights ***TBD***.`

[](#KTRC-formats-and-templates) KTRC Formats and Templates
--------------------------------------------------------------------------------------------

KTRCs should be written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) format. There is a [template](KTRC-template.md) to follow.

##qw KTRC Header Preamble

Each KTRC must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order.

`KTRC`: *KTRC number*

`title`: *The KTRC title is a few words, not a complete sentence*

`description`: *Description is one full (short) sentence*

`author`: *The list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.*

`discussions-to`: *The url pointing to the official discussion thread*

`status`: *Draft, Review, Last Call, Final, Stagnant, Withdrawn, Living*

`last-call-deadline`: *The date last call period ends on* (Optional field, only needed when status is `Last Call`)

`type`: *One of `Standards Track`, `Meta`, or `Informational`*

`category`: *One of `Core`, `Provider`, `KayDev`, or `KayWallet`* (Optional field, only needed for `Standards Track` KTRCs)

`created`: *Date the KTRC was created on*

`requires`: *KTRC number(s)* (Optional field)

`withdrawal-reason`: *A sentence explaining why the KTRC was withdrawn.* (Optional field, only needed when status is `Withdrawn`)

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

### `author` header

The `author` header lists the names, email addresses or usernames of the authors/owners of the KTRC. Those who prefer anonymity may use a username only, or a first name and a username. The format of the `author` header value must be:

> Random J. User <address@dom.ain>

or

> Random J. User (@username)

or

> Random J. User (@username) <address@dom.ain>

if the email address and/or GitHub username is included, and

> Random J. User

if neither the email address nor the GitHub username are given.

At least one author must use a GitHub username, in order to get notified on change requests and have the capability to approve or reject them.

### `discussions-to` header

While an KTRC is a draft, a `discussions-to` header will indicate the URL where the KTRC is being discussed.

The preferred discussion URL is a topic on [Wiki internal](https://dev.azure.com/nttdata-peru/KayTrust/_wiki/wikis/KayTrust.wiki/1/Home) for internal KTRC or [Wiki GitHub](https://github.com/KayTrust/wiki-KTRC-public/wiki) for public KTRC. The URL cannot point to Github pull requests, any URL which is ephemeral, and any URL which can get locked over time (i.e. Reddit topics).

### `type` header

The `type` header specifies the type of KTRC: Standards Track, Meta, or Informational. If the track is Standards please include the subcategory (Core, Provider, KayWallet, or KayDev).

### `category` header

The `category` header specifies the KTRC's category. This is required for standards-track KTRCs only.

### `created` header

The `created` header records the date that the KTRC was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

### `requires` header

KTRCs may have a `requires` header, indicating the KTRC numbers that this KTRC depends on. If such a dependency exists, this field is required.

A `requires` dependency is created when the current KTRC cannot be understood or implemented without a concept or technical element from another KTRC. Merely mentioning another KTRC does not necessarily create such a dependency.

## Linking to External Resources

Other than the specific exceptions listed below, links to external resources SHOULD NOT be included. External resources may disappear, move, or change unexpectedly.

The process governing permitted external resources is described in [EIP-5757](https://eips.ethereum.org/EIPS/eip-5757).

### World Wide Web Consortium (W3C)

Links to a W3C "Recommendation" status specification may be included using normal markdown syntax. For example, the following link would be allowed:

```
[Secure Contexts](https://www.w3.org/TR/2021/CRD-secure-contexts-20210918/)

```

Which renders as:

[Secure Contexts](https://www.w3.org/TR/2021/CRD-secure-contexts-20210918/)

Permitted W3C recommendation URLs MUST anchor to a specification in the technical reports namespace with a date, and so MUST match this regular expression:

```
^https://www\.w3\.org/TR/[0-9][0-9][0-9][0-9]/.*$

```

### Web Hypertext Application Technology Working Group (WHATWG)

Links to WHATWG specifications may be included using normal markdown syntax, such as:

```
[HTML](https://html.spec.whatwg.org/commit-snapshots/578def68a9735a1e36610a6789245ddfc13d24e0/)

```

Which renders as:

[HTML](https://html.spec.whatwg.org/commit-snapshots/578def68a9735a1e36610a6789245ddfc13d24e0/)

Permitted WHATWG specification URLs must anchor to a specification defined in the `spec` subdomain (idea specifications are not allowed) and to a commit snapshot, and so must match this regular expression:

```
^https:\/\/[a-z]*\.spec\.whatwg\.org/commit-snapshots/[0-9a-f]{40}/$

```

Although not recommended by WHATWG, KTRCs must anchor to a particular commit so that future readers can refer to the exact version of the living standard that existed at the time the KTRC was finalized. This gives readers sufficient information to maintain compatibility, if they so choose, with the version referenced by the KTRC and the current living standard.

### Internet Engineering Task Force (IETF)

Links to an IETF Request For Comment (RFC) specification may be included using normal markdown syntax, such as:

```
[RFC 8446](https://www.rfc-editor.org/rfc/rfc8446)

```

Which renders as:

[RFC 8446](https://www.rfc-editor.org/rfc/rfc8446)

Permitted IETF specification URLs MUST anchor to a specification with an assigned RFC number (meaning cannot reference internet drafts), and so MUST match this regular expression:

```
^https:\/\/www.rfc-editor.org\/rfc\/.*$

```

### Bitcoin Improvement Proposal

Links to Bitcoin Improvement Proposals may be included using normal markdown syntax, such as:

```
[BIP 38](https://github.com/bitcoin/bips/blob/3db736243cd01389a4dfd98738204df1856dc5b9/bip-0038.mediawiki)

```

Which renders to:

[BIP 38](https://github.com/bitcoin/bips/blob/3db736243cd01389a4dfd98738204df1856dc5b9/bip-0038.mediawiki)

Permitted Bitcoin Improvement Proposal URLs must anchor to a specific commit, and so must match this regular expression:

```
^(https://github.com/bitcoin/bips/blob/[0-9a-f]{40}/bip-[0-9]+\.mediawiki)$

```

### National Vulnerability Database (NVD)
Links to the Common Vulnerabilities and Exposures (CVE) system as published by the National Institute of Standards and Technology (NIST) may be included, provided they are qualified by the date of the most recent change, using the following syntax:

```
[CVE-2023-29638 (2023-10-17T10:14:15)](https://nvd.nist.gov/vuln/detail/CVE-2023-29638)

```

Which renders to:

[CVE-2023-29638 (2023-10-17T10:14:15)](https://nvd.nist.gov/vuln/detail/CVE-2023-29638)


### Digital Object Identifier System

Links qualified with a Digital Object Identifier (DOI) may be included using the following syntax:

````markdown
This is a sentence with a footnote.[^1]

[^1]:
    ```csl-json
    {
      "type": "article",
      "id": 1,
      "author": [
        {
          "family": "Jameson",
          "given": "Hudson"
        }
      ],
      "DOI": "00.0000/a00000-000-0000-y",
      "title": "An Interesting Article",
      "original-date": {
        "date-parts": [
          [2022, 12, 31]
        ]
      },
      "URL": "https://sly-hub.invalid/00.0000/a00000-000-0000-y",
      "custom": {
        "additional-urls": [
          "https://example.com/an-interesting-article.pdf"
        ]
      }
    }
    ```
````

Which renders to:

<!-- markdownlint-capture -->
<!-- markdownlint-disable code-block-style -->

This is a sentence with a footnote.[^1]

[^1]:
    ```csl-json
    {
      "type": "article",
      "id": 1,
      "author": [
        {
          "family": "Jameson",
          "given": "Hudson"
        }
      ],
      "DOI": "00.0000/a00000-000-0000-y",
      "title": "An Interesting Article",
      "original-date": {
        "date-parts": [
          [2022, 12, 31]
        ]
      },
      "URL": "https://sly-hub.invalid/00.0000/a00000-000-0000-y",
      "custom": {
        "additional-urls": [
          "https://example.com/an-interesting-article.pdf"
        ]
      }
    }
    ```

<!-- markdownlint-restore -->

See the [Citation Style Language Schema](https://resource.citationstyles.org/schema/v1.0/input/json/csl-data.json) for the supported fields. In addition to passing validation against that schema, references must include a DOI and at least one URL.

The top-level URL field must resolve to a copy of the referenced document which can be viewed at zero cost. Values under `additional-urls` must also resolve to a copy of the referenced document, but may charge a fee.

## Linking to other KTRCs

References to other KTRCs should follow the format `KTRC-N` where `N` is the KTRC number you are referring to. Each KTRC that is referenced in an KTRC MUST be accompanied by a relative markdown link the first time it is referenced, and MAY be accompanied by a link on subsequent references. The link MUST always be done via relative paths so that the links work in this GitHub repository, forks of this repository, the main KTRCs site, mirrors of the main KTRC site, etc. For example, you would link to this KTRC as `./KTRC-1.md`.

## Auxiliary Files

Images, diagrams and auxiliary files should be included in a subdirectory of the `assets` folder for that KTRC as follows: `assets/KTRC-N` (where N is to be replaced with the KTRC number). When linking to an image in the KTRC, use relative links such as `../assets/KTRC-1/image.png`.

## Transferring KTRC Ownership

It occasionally becomes necessary to transfer ownership of KTRCs to a new champion. In general, we'd like to retain the original author as a co-author of the transferred KTRC, but that's really up to the original author. A good reason to transfer ownership is because the original author no longer has the time or interest in updating it or following through with the KTRC process, or has fallen off the face of the 'net (i.e. is unreachable or isn't responding to email). A bad reason to transfer ownership is because you don't agree with the direction of the KTRC. We try to build consensus around an KTRC, but if that's not possible, you can always submit a competing KTRC.

If you are interested in assuming ownership of an KTRC, send a message asking to take over, addressed to both the original author and the KTRC editor. If the original author doesn't respond to the email in a timely manner, the KTRC editor will make a unilateral decision (it's not like such decisions can't be reversed :)).

## KTRC Editors

This KTRC is based on the [EIP-1](https://eips.ethereum.org/EIPS/eip-1)

The current KTRC editors are

-   Juan José Miranda (@jjmiranda)
-   David Ammouial (@davux)

Emeritus KTRC editors are

-   Juan José Miranda (@jjmiranda)
-   David Ammouial (@davux)

If you would like to become an KTRC editor, please check [KTRC-2](./KTRC-2).

## KTRC Editor Responsibilities

For each new KTRC that comes in, an editor does the following:

-   Read the KTRC to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
-   The title should accurately describe the content.
-   Check the KTRC for language (spelling, grammar, sentence structure, etc.), markup (GitHub flavored Markdown), code style

If the KTRC isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the KTRC is ready for the repository, the KTRC editor will:

-   Assign an KTRC number (generally incremental; editors can reassign if number sniping is suspected)
-   Merge the corresponding [pull request](https://github.com/KayTrust/KTRCs/pulls)
-   Send a message back to the KTRC author with the next step.

Many KTRCs are written and maintained by developers with write access to the KayTrust codebase. The KTRC editors monitor KTRC changes, and correct any structure, grammar, spelling, or markup mistakes we see.

The editors don't pass judgment on KTRCs. We merely do the administrative & editorial part.

## Style Guide

### Titles

The `title` field in the preamble:

-   Should not include the word "standard" or any variation thereof; and
-   Should not include the KTRC's number.

### Descriptions

The `description` field in the preamble:

-   Should not include the word "standard" or any variation thereof; and
-   Should not include the KTRC's number.

### KTRC numbers

When referring to KTRCs with any other `category`, it must be written in the hyphenated form `KTRC-X` where `X` is that KTRC's assigned number.

### RFC 2119 and RFC 8174

KTRCs are encouraged to follow [RFC 2119](https://www.ietf.org/rfc/rfc2119.html) and [RFC 8174](https://www.ietf.org/rfc/rfc8174.html) for terminology and to insert the following at the beginning of the Specification section:

> The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 and RFC 8174.

## History

This document was derived heavily from [Ethereum's EIP-1](https://eips.ethereum.org/EIPS/eip-1) written by Martin Becze, Hudson Jameson, et al. which in turn was derived from [Bitcoin's BIP-0001](https://github.com/bitcoin/bips) written by Amir Taaki which in turn was derived from [Python's PEP-0001](https://peps.python.org/). In many places text was simply copied and modified. Although the PEP-0001 text was written by Barry Warsaw, Jeremy Hylton, and David Goodger, they are not responsible for its use in the KayTrust Request for Comments, and should not be bothered with technical questions specific to KayTrust or the KTRC. Please direct all comments to the KTRC editors.

## Copyright

Copyright and related rights ***TBD***.

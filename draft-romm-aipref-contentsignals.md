---
title: "Vocabulary For Expressing Content Signals"
abbrev: "AIPREF Content Signals"
category: info

docname: draft-romm-aipref-contentsignals-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: "Web and Internet Transport"
workgroup: "AI Preferences"
keyword:
 - AI preferences
 - content signals
venue:
  group: "AI Preferences"
  type: "Working Group"
  mail: "ai-control@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/ai-control/"
  github: "l-romm/draft-romm-aipref-vocab-contentsignals"
  latest: "https://l-romm.github.io/draft-romm-aipref-vocab-contentsignals/draft-romm-aipref-contentsignals.html"

author:
 -
    fullname: "Leah Romm"
    organization: Cloudflare
    email: "leahromm94@gmail.com"

normative:

informative:

--- abstract

This Internet Draft proposes three categories that would enable parties to express preferences regarding how digital assets are used by automated processing systems. The proposal is for these categories to nest within the larger category of Automated Processing, currently envisaged in the working group draft [[AIPREF-VOCAB]]

--- middle

# Introduction

This proposal introduces and aims to define a specific set of preferences to address the need for expressing how digital assets can be used by automated systems, particularly in the context of training artificial intelligence (AI) models and generating search results. These preference categories enable clear and explicit communication of preferences regarding the use of digital assets for search indexing and AI training.

# Conventions and Definitions

{::boilerplate bcp14-tagged}
For the purposes of this document, in addition to the definitions in [AIPREF-VOCAB] (5 September 2025), the following terms are used:
* **Search Results:** hyperlinks and short excerpts returned from contents of the retrieved asset(s)
* **Retrieval-Augmented Generation (RAG):** A technique where external content is retrieved at query time and supplied to a model to condition the generated output. See [[SUBSTITUTIVE-VOCAB]]

# Vocabulary Definition {: vocabulary}

## Search {: vocab-search}
The act of using one or more assets to build a search index and provide Search Results. Search does not include providing AI-generated search summaries.
The use of assets for Search is a proper subset of Automated Processing usage.

## AI Input {: vocab-ai-input}
The act of inputting an asset or assets into one or more AI models for purposes of retrieval-augmented generation, grounding, or other real-time taking of content for generative AI search answers.
The use of assets for AI Input is a proper subset of Automated Processing usage.

## AI Training {: vocab-ai-train}
The act of training or fine-tuning AI models.
The use of assets for AI Training is a proper subset of Automated Processing usage.

# Usage Category Labels

Each usage category in [] (vocabulary) is mapped to a short textual label. The table below (Table 2) tabulates this mapping.

| Category    | Label      | Reference              |
|:------------|:-----------|:-----------------------|
| Search      | `search`   | [] (vocab-search)      |
| AI Input    | `ai-input` | [] (vocab-ai-input)    |
| AI Training | `ai-train` | [] (vocab-ai-train)    |
: Table 1: Usage Category Labels


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.

# Addendum
The definition definition for Search (3.1) provided in this document may be replaced with the Search Category definition proposed in [[AIPREF-VOCAB]] and copied below:
Using one or more assets in a search application that directs users to the location from which the assets were retrieved.
Search applications can be complex and may serve multiple purposes. Only those parts of applications that direct users to the location of an asset are included in this category of use. This includes the use of titles or excerpts from assets that are used to help users select between multiple candidate options.
Preferences for the Search category apply to those parts of applications that provide search capabilities, regardless of what other preferences are stated.
Parts of applications that do not direct users to the location of assets, such as summaries, are not covered by this category of use.
The use of assets for Search is a proper subset of Automated Processing usage.

--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.


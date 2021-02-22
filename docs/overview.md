[Back: README](../README.md)

# Overview

This document proposes a logical architecture for a minimum viable Filecoin Secondary Retrieval Market. An extended architecture is defined in the appendices that outlines additional components that could be added to this minimalist architecture to provide a richer set of features.

Protocol Labs identified three key problems in creating a secondary retrieval market:

* **Caching strategy**: How do Retrieval Providers know what content is popular, and worth mirroring?
* **Discoverability**: How clients know which Retrieval Providers have their data, so they can target retrieval deal proposals correctly.
* **Incentives**: Are payments and other incentives correctly aligned for Retrieval Providers  to invest & participate?

This document defines an architecture that addresses these concerns and defines how payment channels work in the system. Discoverability and Incentives are addressed by the [Core Architecture](TODO). The caching strategy is primarily covered by the Caching Provider, that is part of the [Extended Architecture](TODO)

Design goals and objectives are listed in [Filecoin Secondary Market Retrieval Objectives](TODO).

[Next: Terminology](terminology.md)
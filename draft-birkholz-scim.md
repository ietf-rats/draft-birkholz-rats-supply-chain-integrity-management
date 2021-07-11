---
title: Supply Chain Integrity Model
abbrev: SCIM
docname: draft-birkholz-scim-latest
stand_alone: true
ipr: trust200902
area: Security
wg: RATS Working Group
kw: Internet-Draft
cat: std
pi:
  toc: yes
  sortrefs: yes
  symrefs: yes

author:
- ins: J. Doe
  name: John Doe
  org: ACME Inc.
  abbrev: ACME Inc.
  email: john.doe@loopback
  street: Loop Back 127
  code: '12712'
  city: Loopback
  country: Germany

normative:
  RFC2119:
  RFC8174:
  I-D.ietf-sacm-coswid: coswid

informative:

--- abstract

Abstract

--- middle

# Introduction

Introduction

# Terminology

Actors:
: Agent - individual or organization.
: Software Agent - software acting on behalf of an Agent.

Roles:
: Issuing Authority - Agent that issues Signed Evidence, e.g. Microsoft. 
: Evidence Generator - Software Agent that generates unsigned Evidence, e.g. Office build system.
: Evidence Signer - Software Agent that accepts unsigned Evidence and signs, e.g. Microsoft signing service.
: Ledger Authority - Agent that governs an evidence registry, e.g. 'Microsoft', 'Global Supply Chain Consortium'.
: Receipt Requestor - Software Agent that submits signed evidence to a Registry.
: Ledger Service - Software Agent that accepts and logs Signed Evidence.
: Evidence Store - Software Agent that supports query of Registered Evidence.

Messages:
: Evidence - unsigned Evidence.
: Signed Evidence - evidence evidence wrapped with a header and signed.
: Receipt Request - request to enter evidence in Registry.
: Receipt - receipt issued by Registry verify signed evidence is registered.
: Registered Evidence - (same as Receipt?)

Questions:
* How do we handle query and receipt of registered evidence in the model?
* How do we handle policy and verification in the model?
 
Ledger:
: tbd

## Requirements Notation

{::boilerplate bcp14-tagged}

{: #mybody}
# SCIM

## The SCIM Diagram

~~~~
{::include simple-diagram.ascii}
~~~~

# SCIM Roles and Messages

## Roles

### Claim-Set Generator

### Issuer

## Messages

# Issuers and Guaranteed Properties

## Component Properties and End-to-End Properties

You need sets of component properties to arrive at end-to-end properties.

### Integrity of the Ledger

* Role of Confidential Compute
* Roots of trusts
* Redundant Byzantine Fault Tolerance
  * what does it mean to be faithful?
  * what does it mean to be slow?
  * what does it mean to be malicious?

# CDDL

See {{-coswid}}.

~~~~ CDDL
<CODE BEGINS>
;{::include some.cddl}
<CODE ENDS>
~~~~

# Privacy Considerations

Privacy Considerations

# Security Considerations

Security Considerations

# IANA Considerations

See Body {{mybody}}.

--- back

# Mapping to RATS

~~~~
{::include scim-rats.ascii}
~~~~

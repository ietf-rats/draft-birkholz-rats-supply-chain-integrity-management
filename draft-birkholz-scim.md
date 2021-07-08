---
title: Supply Chain Integrity Management
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
: Agent
: Software Agent


Roles:
: SCIM Assertion-Set Generator
:

Messages:
: tbd
 
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
{::include simple-diagram.ascii}
~~~~

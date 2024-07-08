---
title: "SCION Deployment Issues"
abbrev: "SCION DI"
category: info
submissiontype: IRTF

docname: draft-meynell-scion-deployment-latest

v: 3
area: "IRTF"
workgroup: "Path Aware Networking RG"
keyword: Internet-Draft
venue:
  group: "Path Aware Networking RG"
  type: "Research Group"
  mail: "panrg@irtf.org"
  arch: "https://www.ietf.org/mail-archive/web/panrg/"
  github: "scionassociation/scion-deployment_I-D"
  latest: "https://scionassociation.github.io/scion-deployment_I-D/draft-meynell-scion-deployment.html"

author:
 -   ins: K. Meynell
     name: Kevin Meynell
     org: SCION Association
     email: kme@scion.org

 -   ins: N. Rustignoli
     name: Nicola Rustignoli
     org: SCION Association
     email: nic@scion.org

normative:
  RFC9217:
  I-D.scion-cp:
    title: SCION Control Plane
    date: 2023
    target: https://datatracker.ietf.org/doc/draft-dekater-scion-controlplane/
    author:
      -
        ins: C. de Kater
        name: Corine de Kater
        org: SCION Association
      -
        ins: N. Rustignoli
        name: Nicola Rustignoli
        org: SCION Association
      -
        ins: S. Hitz
        name: Samuel Hitz
        org: Anapaya Systems
  I-D.scion-cppki:
    title: SCION Control-Plane PKI
    date: 2023
    target: https://datatracker.ietf.org/doc/draft-dekater-scion-pki/
    author:
      -
        ins: C. de Kater
        name: Corine de Kater
        org: SCION Association
      -
        ins: N. Rustignoli
        name: Nicola Rustignoli
        org: SCION Association
      -
        ins: S. Hitz
        name: Samuel Hitz
        org: Anapaya Systems
  I-D.scion-dataplane:
    title: SCION Data Plane
    date: 2023
    target: https://datatracker.ietf.org/doc/draft-dekater-scion-dataplane/
    author:
      -
        ins: C. de Kater
        name: Corine de Kater
        org: SCION Association
      -
        ins: N. Rustignoli
        name: Nicola Rustignoli
        org: SCION Association
      -
        ins: S. Hitz
        name: Samuel Hitz
        org: Anapaya Systems
informative:


--- abstract

TODO Abstract here


--- middle

# Introduction

The goal of this draft is two-fold: it tries to document lessons learned in deploying SCION to some if its productive early adopters, and it tries to tries to answer questions 2.7 - Operating a Path-Aware Network, and 2.8 - Deploying a Path-Aware Network posed in {{RFC9217}}.

**Note:** This is the very first version of the SCION deployment draft, and it merely contains a skeleton of potential topics to be further discussed in this draft. Any feedback is welcome and much appreciated. Thanks!

* This draft assumes the reader is familiar with the overall core SCION specification, outlined in {{I-D.scion-dataplane}}, {{I-D.scion-cppki}}, {{I-D.scion-cp}}.


# Conventions and Definitions

{::boilerplate bcp14-tagged}

# Deployment Models

## SCION Network - How to roll it out.

## SCION-IP Gateway

Introduction to IP in SCION tunneling for ecosystems. See S. Hitz IETF118 presentation: https://datatracker.ietf.org/meeting/118/materials/slides-118-panrg-operational-aspects-of-scion-00

## SCION-enabled Applications/Native SCION Endpoint

## Implications for the transport layer

Address section 2.5 of {{RFC9217}}.


# Establishing and running an Isolation Domain

See F. Steinmann presentation IETF118 - https://datatracker.ietf.org/meeting/118/materials/slides-118-panrg-scion-deployment-experience-the-secure-swiss-finance-network-ssfn

## Description and use case

## Governance

## Core Members - TRC signers

## Issuing Members - issuers of AS certifications

(may be the same as Core Members)

## Non-Core Members

## Coordination

## Required contact information

## Methods of Communication and Authentication requirements

## ISD Policy Development & Maintenance

## Assignment and registration of ISD numbers

## Assignment and registration of SCION AS numbers

## Trust Root Configuration
* TRC signing
* TRC distribution & installation
* Maintaining cryptographic material
* Certificate issuance



# Establishing and running a SCION network

## Prerequisites - e.g. AS number, running existing intra-domain protocol if applicable

## How to join an ISD

## Obtaining a SCION AS number and AS certificate

## Setting up the Control Services (Beacon, Path and Certificate servers)

Also cover Availability & scalability of such services.

## Setting up SCION border routers


## Configuring path (segment) attributes/parameters

How do customers select paths?

## SCION & Network Address Translation

## Software Change Management

# Adding and removing networks from an Isolation Domain

## Adding a new Core network

## Removing an existing Core network

## Changes between existing Core networks

## Adding a new non-Core network

## Removing an existing non-Core network

## Changes between Core network and non-core network

# Connecting to other Isolation Domains

## Inter-ISD Governance

* Inter-ISD Governance (is this applicable?)
* Inter-ISD Policy Development & Maintenance
* Inter-ISD Path selection


# Performance Monitoring


# Security Considerations

## Security Incident Handling


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.

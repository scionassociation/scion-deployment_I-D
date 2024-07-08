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

* Problem statement.
* Refer to the PKI, Control Plane and Data Plane Internet Drafts here.
* Mention we try to answer 2.7 - Operating a Path-Aware Network, and 2.8 - Deploying a Path-Aware Network of rfc9217.

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# Deployment Models

## SCION Network - How to roll it out.
## SCION-IP Gateway & IP in SCION tunneling for ecosystems (see Anapaya IETF118 presentation)
## SCION-enabled Applications
## Implications for the transport layer (section 2.5 of rfc9217)

# Establishing and running an Isolation Domain

**(see SIX presentation IETF118 - https://datatracker.ietf.org/meeting/118/materials/slides-118-panrg-scion-deployment-experience-the-secure-swiss-finance-network-ssfn)**

## Description and use case

## Governance

## Core Members - TRC signers

## Issuing Members - issuers of AS certifications (may be the same as Core Members)

## Non-Core Members (is this the correct term - should we define a better term?)

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

## Security Incident Handling - this could go into the Security section


# Establishing and running a SCION network

## Prerequisites - e.g. AS number, running existing intra-domain protocol if applicable
## How to join an ISD
## Obtaining an SCION AS number and AS certificate
## Setting up the Control Services (Beacon, Path and Certificate servers)
## Availability & scalability
## Setting up SCION border routers
## Customer site deployment (native, SCION-IP gateway, SCION-enabled application)
## Configuring path (segment) attributes/parameters (and how do customers select paths) - this could be a separate section
## SCION & Network Address Translation
## Software Change Management

# Adding and removing networks from an Isolation Doman

## Adding a new Core network
## Removing an existing Core network
## Changes between existing Core networks
## Adding a new non-Core network
## Removing an existing non-Core network
## Changes between Core network and non-core network

# Connecting to other Isolation Domains

**There doesn't seem to be much/any documentation on what needs to be done to set-up inter-ISD communication, or how AS ‘peering’ works across different ISDs.**

* Inter-ISD Governance (is this applicable?)
* Inter-ISD Policy Development & Maintenance
* Inter-ISD Path selection

# SCION-IP Gateway Deployment

**Is this section needed for this Internet Draft? Could it go in the ‘Adding and removing networks from an Isolation Domain’ section?**

# End Host Deployment

**Is this section needed for this Internet Draft? Could it go in the ‘Adding and removing networks from an Isolation Domain’ section?**

# Performance Monitoring

**This is outlined in the 'Best Practices for SCION ISD Operations but is this strictly needed for an Internet Draft? Most/all networks should be monitored as a matter of good operational practice, and unless SCION networks need to meet stated parameters, is this section actually required?**

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.

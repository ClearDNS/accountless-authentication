# Accountless Authentication: A DNS-Based Architecture for Individualized Service Authorization

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23128122.svg)](https://doi.org/10.5281/zenodo.23128122)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

A white paper by ClearDNS, LLC. October 5, 2026.

**Personal identification is not a technical necessity.**

Many services ask for an email address before they do anything else, and that address links a person to the records associated with the account. This paper describes an architecture in which authenticated DNS use establishes an enrolled relationship between a service and a device, so that settings, shared access, individual permissions, recovery and paid features work without a name, an email address or an account password.

An encrypted-DNS configuration installed at enrollment carries a per-device credential. The resolver authenticates it, finds the policy, member and device it belongs to, and checks that the device is still permitted. A management dashboard uses that verified context together with a PIN or MFA in place of an email-and-password login. ClearDNS implements the architecture as a working DNS filtering service.

The paper covers enrollment, roles, sessions, revocation, recovery, data visibility and transport choices, gives procedures readers can use to test the service, and includes selected observations from our own testing.

## Read the paper

- [PDF](ClearDNS-Accountless-Authentication.pdf) (22 pages)
- [Markdown](ClearDNS-Accountless-Authentication.md), with diagrams rendered by GitHub

The same files are published at:

- ClearDNS research page: https://cleardns.com/research/
- Zenodo: https://doi.org/10.5281/zenodo.23128122

## Discuss it

We invite readers to examine the architecture, test the implementation and publish frank technical assessments. Critical findings, failed tests and different interpretations are all useful.

Questions and assessments are welcome in [Discussions](https://github.com/cleardns/accountless-authentication/discussions). Findings can also be sent to contact@cleardns.io.

Please do not post credentials, resolver addresses or identifiers from a real policy.

## Cite it

ClearDNS, LLC. *Accountless Authentication: A DNS-Based Architecture for Individualized Service Authorization.* White paper, October 5, 2026. https://doi.org/10.5281/zenodo.23128122

A machine-readable citation is in [CITATION.cff](CITATION.cff).

## Verify the files

SHA-256 checksums, also in [SHA256SUMS](SHA256SUMS):

```
4a690de4c99f03c0974d0e743502e34340e758ac81caf0d8e0546bec135d702c  ClearDNS-Accountless-Authentication.pdf
c5956a15636b944d6c2d122834d5e6ac90df57ef83ad1e9b655f49158c3d1584  ClearDNS-Accountless-Authentication.md
```

## Licence

© 2026 ClearDNS, LLC. The paper is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/): you may share it unchanged, with attribution, for non-commercial purposes.

More about how the service works and what data it handles is in the [ClearDNS Transparency Center](https://cleardns.com/technical-transparency/).

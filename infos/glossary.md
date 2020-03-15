## SSI Cloud Agents:
While not strictly logically necessary from a pure logical point-of-view, in practice this server-side DKMS layer plays a similar role in DID infrastructure as email servers play in SMTP email infrastructure or Web servers play in Web infrastructure. Like email or Web servers, cloud agents and cloud wallets are designed to be available 24 x 7 to send and receive communications on behalf of their identity owners. They are also designed to perform communications, encryption, key management, data management, and data storage and backup processes that are not typically feasible for edge devices given their typical computational power, bandwidth, storage capacity, reliability and/or availability.
Cloud agents and wallets will typically be hosted by a service provider called an agency. Agencies could be operated by any type of service provider—ISPs, telcos, search engines, social networks, banks, utility companies, governments, etc. A third party agency is not a requirement of DKMS architecture—any identity owner can also host their own cloud agents.

## SSI Edge Agents:
The edge layer is where most DKMS private keys and link secrets are generated and where most key operations and storage are performed. To meet the security and privacy requirements, DKMS architecture makes the following two assumptions:
- A DKMS agent is always installed in an environment that includes a secure element or Trusted Platform Module (for simplicity, this document will use the term "secure element" or “SE” for this module).
- Private keys used by the agent never leave the secure element.

## TSS vs SSS:
- Key Generation: in SSSS, there is a single party called “the dealer” that is in charge of generating the private key secret shares. It means that at time of Key Generation, the private key is generated at a single location and then distributed by the dealer to the different locations. In TSS, there is no dealer as its role is distributed such that the full private key is never at a single location.
- Signing: in SSSS, the parties must reconstruct the full private key in order to sign, which again results in a single point of failure each time a signature is needed. In TSS, the signing is done in a distributed way without ever reconstructing the secret shares.

## Distributed vs Decentralized
See links in links.md -> basically there is a lot of different information about decentralization. But decentralized systems are a subset of distributed systems. Decentralized: system with local information have local goals, distributed: computation across components to achieve a common goal

## HyperLedger Aries vs. Indy
https://sovrin.org/sovrin-proudly-contributes-to-hyperledger-aries: "One of the architectural components of Indy is called an Agent. This is software that acts on behalf of an identity owner to communicate off-ledger with other Agents. As Agent work continued with the development of message encryption standards, extensible message typing, and common protocols, interest grew in applying these concepts and practices to systems based on other ledgers. It became clear that the right future for Agent work was to extract it from Indy project and add support for other ledger technologies to make that integration easier and more powerful. That work is now known as Hyperledger Aries."

## Argent
Argent is a smart contract wallet.
It enables users to recover their wallets even after they've lost their seed phrases, by appointing "Guardians" (either friends, hardware wallets or Argent's own Guard service) who are tasked with agreeing to unlock your wallet.

## SSI Cloud Agents:
While not strictly logically necessary from a pure logical point-of-view, in practice this server-side DKMS layer plays a similar role in DID infrastructure as email servers play in SMTP email infrastructure or Web servers play in Web infrastructure. Like email or Web servers, cloud agents and cloud wallets are designed to be available 24 x 7 to send and receive communications on behalf of their identity owners. They are also designed to perform communications, encryption, key management, data management, and data storage and backup processes that are not typically feasible for edge devices given their typical computational power, bandwidth, storage capacity, reliability and/or availability.
Cloud agents and wallets will typically be hosted by a service provider called an agency. Agencies could be operated by any type of service provider—ISPs, telcos, search engines, social networks, banks, utility companies, governments, etc. A third party agency is not a requirement of DKMS architecture—any identity owner can also host their own cloud agents.

## SSI Edge Agents:
The edge layer is where most DKMS private keys and link secrets are generated and where most key operations and storage are performed. To meet the security and privacy requirements, DKMS architecture makes the following two assumptions:
- A DKMS agent is always installed in an environment that includes a secure element or Trusted Platform Module (for simplicity, this document will use the term "secure element" or “SE” for this module).
- Private keys used by the agent never leave the secure element.

## HyperLedger Aries recovery mechanism
- Offline recovery: Offline recovery is the conventional form of backup. It can be performed using many different methods. In DKMS architecture, the standard strategy is to store an encrypted backup of the identity owner’s wallet at the owner’s cloud agent, and then store a private backup recovery key offline. The private backup recovery key can be printed to a paper wallet as one or more QR codes or text strings. It can also be saved to a file on a detachable media device such as a removable disk, hardware wallet or USB key.
- Social Recovery: A trustee is any person, institution, or service that agrees to assist an identity owner during recovery by (1) securely storing recovery material (called a "share") until a recovery is needed, and (2) positively identifying the identity owner and the authenticity of a recovery request before authorizing release of their shares.

This second step is critical. Trustees MUST strongly authenticate an identity owner during recovery so as to detect if an attacker is trying exploit them to steal a key or secret. Software should aid in ensuring the authentication is strong, for example, confirming the trustee actually conversed with Alice, as opposed to getting an email from her.

## Threshold Signature Scheme TSS vs SSS:
- Key Generation: in SSSS, there is a single party called “the dealer” that is in charge of generating the private key secret shares. It means that at time of Key Generation, the private key is generated at a single location and then distributed by the dealer to the different locations. In TSS, there is no dealer as its role is distributed such that the full private key is never at a single location.
- Signing: in SSSS, the parties must reconstruct the full private key in order to sign, which again results in a single point of failure each time a signature is needed. In TSS, the signing is done in a distributed way without ever reconstructing the secret shares.

## Distributed vs Decentralized
See links in links.md -> basically there is a lot of different information about decentralization. But decentralized systems are a subset of distributed systems. Decentralized: system with local information have local goals, distributed: computation across components to achieve a common goal

## HyperLedger Aries vs. Indy
https://sovrin.org/sovrin-proudly-contributes-to-hyperledger-aries: "One of the architectural components of Indy is called an Agent. This is software that acts on behalf of an identity owner to communicate off-ledger with other Agents. As Agent work continued with the development of message encryption standards, extensible message typing, and common protocols, interest grew in applying these concepts and practices to systems based on other ledgers. It became clear that the right future for Agent work was to extract it from Indy project and add support for other ledger technologies to make that integration easier and more powerful. That work is now known as Hyperledger Aries."

## Argent
Argent is a smart contract wallet.
It enables users to recover their wallets even after they've lost their seed phrases, by appointing "Guardians" (either friends, hardware wallets or Argent's own Guard service) who are tasked with agreeing to unlock your wallet.

-----to show-----

## Dark Crystal
Dark Crystal transforms secrets into crystal shards that you can send to trusted friends. If you lose the secret, or something happens to you, your friends can combine the shards to recover the crystal and reveal the secret.
It uses cryptography so that no individual shard reveals anything about your secret on its own. Your secret is only revealed if the people you chose cooperate and put their shards together. It uses the Scuttlebutt Protocol.
"Sharding (aka Shamir's Secret Sharing) isn't new. What makes Dark Crystal different?" -> While sharding technology has been around for a long time, it hasn't been widely adopted. We think that's because the process is complicated, difficult, and error-prone. Dark Crystal makes it much simpler and more user-friendly. If more people use sharding successfully, fewer secrets will be lost unintentionally.

## Scuttlebutt Protocol 
Scuttlebutt is a protocol for building decentralized applications that work well offline and that no one person can control. Because there is no central server, Scuttlebutt clients connect to their peers to exchange information. This guide describes the protocols used to communicate within the Scuttlebutt network.
If the client is not publicy accessible it is possible to use Pubs which are publicly-accessible Scuttlebutt peers. Is this really decentralized?

## Three Rs of Key Management
The three main key management tasks are key reproduction, key recovery, and key rotation. We call these the three Rs of key management.

## Different Schemes
### Threshold Secret Sharing
- List:
 - Shamir (polynomial based)
 - Blakley (vector space based)
 - Mignotte (based on Chinese Remainder Theorem)
 - Asmuth-Bloom (based on Chinese Remainer Theorem)
- SSS vs Asmuth-Bloom: https://crypto.stackexchange.com/questions/34317/shamirs-secret-sharing-vs-asmuth-bloom-scheme (asmuth-bloom leaks some information while SSS does not)
- SSS vs Blakley: Blakley's scheme is less space-efficient than Shamir's [...] (https://en.wikipedia.org/wiki/Secret_sharing#Blakley's_scheme)
### Verifiable Schemes
- Pedersen Scheme 
- Feldman Scheme (based on Shamir)
- Schoenmakers scheme

# Linksammlung

## General
* Dezentralized vs. distributed:
  * Decentralized: https://medium.com/@VitalikButerin/the-meaning-of-decentralization-a0c92b76a274
  * Distributed: https://blog.stackpath.com/distributed-system/

## DKMS and SSI
### DKMS Intro 
- https://www.youtube.com/watch?v=LOrXOxc2yp0 (7m)
- general questions about key management
### Intro to problems and solutions from Evernym 
- Video (1h) and slides
- https://ssimeetup.org/decentralized-key-management-dkms-essential-missing-piece-ssi-puzzle-drummond-reed-webinar-8/
- extended introduction with a hint to Hyperledger Indy
### Different methods for key recovery (Ethereum)
- https://hackernoon.com/solutions-for-private-key-management-in-decentralized-apps-24f95634be16
### SSI
- https://medium.com/evernym/the-three-models-of-digital-identity-relationships-ca0727cb5186 -> links also to hyperledger/indy solution
- Book (A comprehensive guide to SSI - Kaliya Young)
- https://www.coindesk.com/theres-alternative-facebook-called-self-sovereign-identity
- https://identitywoman.net
- http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html
- DIDs (video by drummond reed): https://www.youtube.com/watch?v=LkUkcoyksSI / https://www.youtube.com/watch?v=gf2g4O3yqCc / https://www.youtube.com/watch?v=SHuRRaOBMz4
- Verifiable Credentials (video by drummond reed): https://www.youtube.com/watch?v=6O_iJnhIh5o
- Aries (Agents part) (video by drummond reed): https://www.youtube.com/watch?v=PXPZQB3VG9w

## Hyperledger Indy (open-source Sovrin):
### Documentation
- https://www.hyperledger.org/projects/hyperledger-indy
- https://hyperledger-indy.readthedocs.io/projects/sdk/en/latest/docs/design/005-dkms/
- https://wiki.hyperledger.org/display/indy/Hyperledger+Indy
- https://github.com/hyperledger/indy-sdk/blob/master/README.md
- https://github.com/WebOfTrustInfo/rwot4-paris/blob/master/topics-and-advance-readings/dkms-decentralized-key-mgmt-system.md
### Hyperledger Indy Agents
- https://www.youtube.com/watch?v=llwfb5Ut5sg (2h)
### Hyperledger Aries
- https://github.com/hyperledger/aries-rfcs/blob/master/concepts/0051-dkms/dkms-v4.md
- Workflows for Aries: https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0051-dkms/images

## Social recovery
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/social-key-recovery.md
This explains some problems of SSS. It also explains how something like 'It needs 1 of your friends, 1 of your family and 1 of your business partners' can be achieved without e.g. 3 business partners being able to restore the key, altough they are "3 our of N". (called circles)
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/security_shamirs.md
Their thoughts on SSS and their implementation changes. Also talk about revoking & verification of shares (did a certain party give their correct share -> Public publishing, feldman scheme, schoenmakers scheme). Products of them: **Dark-Crystal**, a social backup and recovery system for secrets such as cryptographic keys, built on the peer-to-peer protocol **Secure Scuttlebutt**. (MMT) -> https://darkcrystal.pw/
- https://github.com/blockades/mmt_resources/blob/master/research/coconut_brainstorm.md
Coconut-related scenarios - what happens if you loose trust in one holder of a shamir secret
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/Socia_%20Key_Recovery_design_implentation.md
Social Key Recovery in regards to the App "Zion"
- https://github.com/WebOfTrustInfo/rwot9-prague/blob/master/topics-and-advance-readings/zion-sdks-skr.md
Zion Key Management APIs and Social Key Recovery
- https://nbviewer.jupyter.org/github/WebOfTrustInfo/rwot8-barcelona/blob/master/final-documents/evaluating-social-recovery.pdf
RWOT8 Very very interesting thoughts about social recovery! Sentence "For encryption keys..." -> ?? Also says how TSS could be useful for our usecase. Also emphasises, that there is no sense in restoring a compromised signing key.

### SSSS - Shamir's Secret Sharing Scheme / Secret Sharing
- SSSS explained: https://www.youtube.com/watch?v=iFY5SyY3IMQ
- Case AGAINST SSS by Bitcoin: https://en.bitcoin.it/wiki/Shamir_Secret_Snakeoil
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/implementing-threshold-schemes.md
Daan Sprenkels talks about integrity protection of the shares -> Feldman VSS, Pederson VSS, Hashing. Gives advantages and disadvantages of all the possibilities and explains problems.
- https://github.com/WebOfTrustInfo/rwot9-prague/blob/master/topics-and-advance-readings/verifiable-secret-sharing.md
Publicly verifiable split-key schemes for hybrid secret sharing 
- https://github.com/satoshilabs/slips/blob/master/slip-0039.md
Complicated proposition for a standard of SSS.
- http://www.moserware.com/2011/11/life-death-and-splitting-secrets.html
He splitted his PW with SSS (own tool) and explained the process & maths.
- https://www.popsci.com/technology/article/2010-07/order-seven-cyber-guardians-around-world-now-hold-keys-internet/
Just the fact, that the DNSSEC Root key is split with SSS.
- https://pph.io/PolyPasswordHasher/
Password Managing Scheme for Servers based on SSS. Not so relevant for our use case
- https://github.com/ryancdotorg/threshcrypt
Implementation of file encryption using shamir's secret sharing. It takes things a step further, adding passwords to each shard.
- https://github.com/karlgluck/ThresholdJS
Basic SSS implementation with live demo
- https://www.vaultproject.io/
Vault also uses SSS, that's it.
- http://passguardian.com/
Webbased implementation of SSS.
- https://secrets.dyne.org/about
Simple Secret Sharing
- https://raw.githubusercontent.com/kyphae/truename-index/master/index.html
SSS in one single index.html
- https://github.com/dsprenkels/sss
Daan Sprenkels SSS Library with infos on SSS Schemes. Also talks about other libraries and their insecurities. Also says when to use verifiable shares and when not to. This is also the library which the Zion App by HTC Exodus uses! Good talk by him: https://www.youtube.com/watch?v=ojMFCpUt7OU
- https://cs.iupui.edu/~xzou/Papers/ICCCN2011-SecretSharing.pdf
New Approach to WEIGHTED secret sharing

## Sovrin (permissioned blockchain)
### Overview
- https://sovrin.org/library/
- Evernym (SSI Company behind Sovrin): https://www.evernym.com/
- stealing phone: https://sovrin.org/wp-content/uploads/2019/03/What-if-someone-steals-my-phone-110319.pdf
- https://www.windley.com/archives/2017/09/is_sovrin_decentralized.shtml

## re:ClaimID
- re:ClaimID based on GNS. Login just like OpenID Connect (transparent for user):
- https://media.ccc.de/v/ds19-10383-re_claimid
- https://arxiv.org/pdf/1805.06253.pdf

## Swisscom Blockchain
- https://www.blockchain.swisscom.com/event-details/

## Other Solutions
### longplay.me
- longplay.me
### Social key recovery
https://adorsys-platform.de/solutions/social-key-recovery/
### Bitcoin
- Bitcoin social recovery - threshold signature
- https://medium.com/iov-internet-of-values/private-key-recovery-decentralize-users-responsibility-88fa60ee905
### TSS - Threshold signatures
- https://www.binance.vision/security/threshold-signatures-explained
### Paralysis Proofs
- https://eprint.iacr.org/2018/096.pdf
- https://hackingdistributed.com/2018/01/18/paralysis-proofs/
### Anastasis
- Ein Distributed Key Management System (DKMS) auf Basis DHT ist Anastatis
- https://docs.taler.net/anastasis.html


## Other Infos
### NuCypher - Decentralized re-encryption
- https://www.youtube.com/watch?v=CxZqqfx24lc (20m)
- https://github.com/nucypher/nucypher

## Crypto Wallet Recovery
### Argent - Crypto wallet 
- https://github.com/argentlabs/argent-contracts/blob/develop/specifications/specifications.pdf
### Gnosis Safe - Crypto wallet
- https://gnosis-safe.readthedocs.io/en/latest/contracts/architecture.html
### ZenGo - "Keyless" Crypto wallet (using TSS)
- https://zengo.com/security/
- https://zengo.com/security-in-depth/
- https://github.com/KZen-networks/multi-party-ecdsa

## Indy Agent Demo
- Alice: http://147.87.118.10:3000
- Bob: http://147.87.118.10:3001
- Faber College: http://147.87.118.10:3002
- Acme Corp: http://147.87.118.10:3002

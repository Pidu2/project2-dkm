# Linksammlung

## SSI 
- https://www.youtube.com/watch?v=LOrXOxc2yp0 -> general questions about key management for SSI
- https://medium.com/evernym/the-three-models-of-digital-identity-relationships-ca0727cb5186 -> SSI basics
- https://sovrin.org/wp-content/uploads/2019/03/What-if-someone-steals-my-phone-110319.pdf -> stealing phone

## Social recovery
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/social-key-recovery.md
This explains some problems of SSS. It also explains how something like 'It needs 1 of your friends, 1 of your family and 1 of your business partners' can be achieved without e.g. 3 business partners being able to restore the key, altough they are "3 our of N". (called circles)
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/security_shamirs.md
Their thoughts on SSS and their implementation changes. Also talk about revoking & verification of shares (did a certain party give their correct share -> Public publishing, feldman scheme, schoenmakers scheme). Products of them: **Dark-Crystal**, a social backup and recovery system for secrets such as cryptographic keys, built on the peer-to-peer protocol **Secure Scuttlebutt**. (MMT) -> https://darkcrystal.pw/
- https://github.com/blockades/mmt_resources/blob/master/research/coconut_brainstorm.md
Coconut-related scenarios - what happens if you loose trust in one holder of a shamir secret
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/Socia_%20Key_Recovery_design_implentation.md
Social Key Recovery in regards to the App "Zion"
- https://nbviewer.jupyter.org/github/WebOfTrustInfo/rwot8-barcelona/blob/master/final-documents/evaluating-social-recovery.pdf
RWOT8 Very very interesting thoughts about social recovery! Sentence "For encryption keys..." -> ?? Also says how TSS could be useful for our usecase. Also emphasises, that there is no sense in restoring a compromised signing key. In the appendix, the questions that have to be answered when implementing a social recovery scheme are summarized, which is also great.

### Substrate - Blockchain framework with built-in social recovery
- https://substrate.dev/
- https://github.com/paritytech/substrate/blob/master/frame/recovery/src/lib.rs

### Biometric with secret sharing
- https://arxiv.org/pdf/1907.04156.pdf - Paper about using biometric with secret sharing

### SSSS - Shamir's Secret Sharing Scheme / Secret Sharing
- SSSS explained: https://www.youtube.com/watch?v=iFY5SyY3IMQ
- Case AGAINST SSS by Bitcoin: https://en.bitcoin.it/wiki/Shamir_Secret_Snakeoil
- https://github.com/WebOfTrustInfo/rwot8-barcelona/blob/master/topics-and-advance-readings/implementing-threshold-schemes.md
Daan Sprenkels talks about integrity protection of the shares -> Feldman VSS, Pederson VSS, Hashing. Gives advantages and disadvantages of all the possibilities and explains problems.
- https://www.popsci.com/technology/article/2010-07/order-seven-cyber-guardians-around-world-now-hold-keys-internet/
Just the fact, that the DNSSEC Root key is split with SSS.
- https://github.com/dsprenkels/sss
Daan Sprenkels SSS Library with infos on SSS Schemes. Also talks about other libraries and their insecurities. Also says when to use verifiable shares and when not to. This is also the library which the Zion App by HTC Exodus uses! Good talk by him: https://www.youtube.com/watch?v=ojMFCpUt7OU

## Other Solutions
### Bitcoin
- Bitcoin social recovery - threshold signature
- https://medium.com/iov-internet-of-values/private-key-recovery-decentralize-users-responsibility-88fa60ee905
### TSS - Threshold signatures
- https://www.binance.vision/security/threshold-signatures-explained
### Paralysis Proofs
- https://eprint.iacr.org/2018/096.pdf
- https://hackingdistributed.com/2018/01/18/paralysis-proofs/
### Different methods for key recovery (Ethereum)
- https://hackernoon.com/solutions-for-private-key-management-in-decentralized-apps-24f95634be16

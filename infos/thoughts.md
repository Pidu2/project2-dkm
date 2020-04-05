Solutions for private key recovery:
- Mnemonic: Is a series of words that can cryptographically derive a private key. Used for Ethereum and Binance.
- Social Recovery: Group of friends are able to recover access to the lost account. Used for WeChat. (SSS)
- Paralysis Proofs: Multisig-scheme and one looses a key. Recover this key by proving that the key is lost.
- Key recovery by MultiSigning the new key (name?)
- Idea: Generate a seed to deterministically generate private key from. Store the seed offline. Recover the keys from this seed. -> isn't this the same as mnemonic?
- Key escrow: 3rd party is granted access to key under certain circumstances

What about making this idiot proof?

Document layout:
- Management Summary
- Introduction
- Explain SSI and/or use case
- Key recovery technologies (basic technologies for key recovery e.g. crypto TSS/SSSS)
  * Possibly one example application using that technology
- Criteria catalog explanation
- Criteria catalog with a possible solutions per key recovery technology -> Table/Matrix
- Key recovery showcase (actual usage of one of these apps/technologies)
- Summary

Wording:
- DID (decentralized identifier)
- DDO (DID descriptor object, documents (infos) referenced by DID)

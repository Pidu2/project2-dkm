Solutions for private key recovery:
- Mnemonic / Seed phrase: Is a series of words that can cryptographically derive a private key. Used for Ethereum and Binance.
- Social Recovery: Group of friends are able to recover access to the lost account. Used for WeChat. (SSS)
- Paralysis Proofs: Multisig-scheme and one looses a key. Recover this key by proving that the key is lost. -> not really usable for SSI..?
- TSS: Key recovery by Threshold Signing the new key
- Key escrow: key is held under escrow- access to key is granted under certain circumstances
- Biometrics

Document layout:
- Management Summary
- Introduction
  * what if someone steals my phone (sovrin)
  * use cases (crypto, SSI, ...)
  * idea of sharding etc.
  * solution should be usable for ssi
- Explain SSI
  * grob (siehe links)
- Key recovery technologies (basic technologies for key recovery e.g. crypto TSS/SSSS)
  * incl. gedanken zu dingen wie anonymität unter teilnehmer etc
  * fazit mit fehlenden aspekten
- Applications with reference to technology
- Criteria catalog
  * explanation
  * Criteria catalog with a possible solutions per key recovery app -> Table/Matrix
- Key recovery showcase (actual usage of one or two of these apps for our use case)
- Summary

Possible subjects for BaTh:
- Creating a SSI app (lightweight) with a key recovery mechanism based on a existing app (and the local API)
  * Checking vault12 for local API
- Creating a Key Recovery app with an API (based on a known library and peer-to-peer protocol)
  * Searching for an open-source peer-to-peer protocol
- Extending a existing app with a Key Recovery function (open-source app)
  * Searching for open-source SSI apps

Wording:
- DID (decentralized identifier)
- DDO (DID descriptor object, documents (infos) referenced by DID)

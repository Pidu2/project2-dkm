BaTh:
- Kind of a similar use case: different keys are generated and then “merged” together to get one key
- In their thesis, there seem to always be an exact number of keys to restore “the one” key. We talked about having the possibility to restore the key with e.g. 3 out of 5 keys.

Book:
- The book does not yet have the chapters that would be most interesting for us (DKM: Introduction, Key regeneration, Key rotation, Key recovery)
- Still, parts of it should probably be read to have a good idea of SSI in general and how a DKM needs to be built to support it

Evernym and Sovrin:
- Funded with the money from U.S. Department of Homeland Security

Key recovery:
- Shamir secret sharing scheme -> Hyperledger Indy
- Threshold signature scheme -> Binance

Solutions for private key recovery:
- Mnemonic: Is a series of words that can cryptographically derive a private key. Used for Ethereum and Binance.
- Social Recovery: Group of friends are able to recover access to the lost account. Used for WeChat.
- Paralysis Proofs: Multisig-scheme and one looses a key. Recover this key by proving that the key is lost.
- Idea: Generate a seed to deterministically generate private key from. Store the seed offline. Recover the keys from this seed.
What about making this idiot proof?

SSSS vs TSS:
- Multiple parties have parts of the sk in TSS and not only one party

NuCypher and pyUmbral:
- pyUmbral is the cryptographic engine behind nucypher, a proxy re-encryption network to empower privacy in decentralized systems.
- pyUmbral distributes N parts of key on a DLT, whereas M parts are required to re-encrypt the data for another user
- Not usable for our projet as there are just multiple Ursulas (nodes) involved and not multiple social parts

Document layout:
- Management Summary
- Introduction
- Explain SSI and/or use case
- Key recovery technologies (basic technologies for key recovery e.g. crypto TSS/SSSS)
- Criteria catalog explanation
- Criteria catalog with a possible solutions per key recovery technology -> Table/Matrix
- Key recovery showcase (actual usage of one of these apps/technologies)
- Summary

Wording:
- DID (decentralized identifier)
- DDO (DID descriptor object, documents (infos) referenced by DID)

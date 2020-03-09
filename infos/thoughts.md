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

NuCypher and pyUmbral:
- pyUmbral is the cryptographic engine behind nucypher, a proxy re-encryption network to empower privacy in decentralized systems.
- pyUmbral distributes N parts of key on a DLT, whereas M parts are required to re-encrypt the data for another user
- Not usable for our projet as there are just multiple Ursulas (nodes) involved and not multiple social parts

Document layout:
- Management Summary
- Introduction
- Explain SSI and/or use case
- Overview of possible technologies (links)
- Key recovery technologies (basic technologies for key recovery e.g. crypto TSS/SSSS)
- Criteria catalog explanation
- Criteria catalog with 3 possible solutions
- Key Recovery (actual usage of one of these technologies)
- Summary

Wording:
- DID (decentralized identifier)
- DDO (DID descriptor object, documents (infos) referenced by DID)

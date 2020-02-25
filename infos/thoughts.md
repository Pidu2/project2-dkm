Thoughts BaTh:
- Kind of a similar use case: different keys are generated and then “merged” together to get one key. This is probably the way we will restore a lost private key for our project.
- A key difference being that we do not really have to worry about the public key part I guess
- Parts of the cryptography can be used 1:1? (Especially Point 3.3.5)
- In their thesis, there seem to always be an exact number of keys to restore “the one” key. We talked about having the possibility to restore the key with e.g. 3 out of 5 keys.
Toughts Book:
- The book does not yet have the chapters that would be most interesting for us (DKM: Introduction, Key regeneration, Key rotation, Key recovery)
- Still, parts of it should probably be read to have a good idea of SSI in general and how a DKM needs to be built to support it
Thoughts Evernym and Sovrin:
- Funded with the money from U.S. Department of Homeland Security
Thoughts key recovery:
- Shamir secret sharing scheme -> Hyperledger Indy
- Threshold signature scheme -> Binance

- Where are the exact differentiation between SSI and DKMS, are there any?
- Decentralized vs. distributed
- DLT for key recovery?
- NuCypher example, what's this?

Document layout:
- Introduction
- Explain SSI
- Different Technologies
- Key Recovery
- Summary

Wording:
DID (decentralized identifier)
DDO (DID descriptor object)

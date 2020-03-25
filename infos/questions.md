| Date issued  | Topic | Question | State | (Current) Solution | Next meeting |
| :-----------: | ------------- | --------------------- | ------- | ---------------------- | :---------: |
| | General | DKMS all of it or only key recovery (etc.)?  | Closed | Focus key recovery | |
| | General | SSI / DKMS -> SSI how deep? Key recovery only SSI? | Closed | Solution has to be usable for SSI/FIDO | |
| | General | Swisscom connections? | Open | Mrs Laube will check for connections | x |
| 03.03.2020 | General | Decentralized vs. distributed (naming) | Closed  | Check glossary | |
| 03.03.2020 | Applications | Usable Apps?: Have a look at streetcred.id, keepin, globaliD and other apps | Waiting | apps.md & Look into streetcred devportal. -> wallet is completely interoperable with aries protocol standard. devportal is easy way to talk to their API to issue credentials etc for aries wallets without writing code (connections, credentials, verifications, organizations..). wallet should be great tool for developing own applications with detailed error messages etc. Nothing for key recovery on the devportal -> email: no solution built in so far, but will also be using mnemonic (bip-0039).| x |
| 03.03.2020 | HyperLedger | HyperLedger Aries vs. Indy? | Closed | Check glossary | |
| 03.03.2020 | HyperLedger | What's necessary to install a HyperLedger Indy blockchain? | To test | Seems to be pretty easy with docker -> https://github.com/hyperledger/indy-node/blob/master/environment/docker/pool/README.md | |
| 03.03.2020 | nuCypher | NuCypher example (called DKMS), what's this? | Closed | Proxy Re-Encryption: Basically, Alice is able to encrypt her data, then let that data be "proxy-reencrypted" by Ursula (untrusted 3rd party) or in NuCyphers case multiple Ursulas (what makes it a **D**KMS). The Ursulas each get a fragment of the reencryption key (sharding similair to shamir secret sharing). Bob then goes to each of the Ursulas and asks for the data. If Alice granted Bob access, Bob needs to find M of N Ursulas to get the data which is decryptable by him. In the process, the data is never decrypted. | |
| 09.03.2020 | nuCypher | pyUmbral -> Crypto usable for our case? | Closed | NuCypher does not meet our requirements |  |
| 17.03.2020 | procivis | Look/ask for documentation (key recovery) | Open | Mail sent |  |
| 17.03.2020 | Applications | Look for applications that actually support social key recovery | Open | See glossary for Dark Crystal, | |
| 17.03.2020 | HyperLedger | Aries implementation w/ social recovery | Open | | |
| 17.03.2020 | Social Recovery | Look into social recovery links | Open | | |
| 17.03.2020 | Reclaim:ID | Ask for key recovery options | Done | No solution. They may use anastasis. | x |
| 17.03.2020 | Anastasis | Ask whether they are using SSS | Open | Mail sent | x |
| 21.03.2020 | Revocation | In a 2nd step, not only key recovery but also key revocation will be important | Open | As opposed to key recovery, revocation needs an implementation on the ledger side. -> How far is Indy etc on this? |X|
| 24.03.2020 | General | Comparing Applications (Dark Crystal, StreetCred.id) or key recovery mechanism? Use cases on Applications or on key recovery mechanism | Open || x |
| 24.03.2020 | General | Who backups the configuration if you loose the information who you gave shares? | Open |||

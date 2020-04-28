| Date issued  | Topic | Question | State | (Current) Solution | Next meeting |
| :-----------: | ------------- | --------------------- | ------- | ---------------------- | :---------: |
| 17.03.2020 | procivis | Look/ask for documentation (key recovery) | Open | Mail sent |  |
| 17.03.2020 | Applications | Look for applications that actually support social key recovery | Open | See glossary and apps.md | |
| 17.03.2020 | HyperLedger | Aries implementation w/ social recovery -> Check all "Sovrin Stewards" | Mails sent | | |
| 21.03.2020 | Revocation | In a 2nd step, not only key recovery but also key revocation will be important | Open | As opposed to key recovery, revocation needs an implementation on the ledger side. -> How far is Indy etc on this? ||
| 24.03.2020 | General | Who backups the configuration if you loose the information to whom you gave the shares? | Open |||
| 25.03.2020 | Scheme | Do we need verifiable Schemes? | Review | Pedersen, Feldman VSS...<br>-> For recovery, these schemes can be useful to prevent participants from cheating. For "revocation"-case, it does not really matter. ||
| 20.04.2020 | Applications | Look for open-source SSI applications | Open | not found | |
| 20.04.2020 | Applications | Check if vault12 has a usable local API | Closed | Android Share API | x |
| 20.04.2020 | Applications | Search open-source peer-to-peer protocols and known libraries for key sharding | Open | | |
| 20.04.2020 | General | What is possible with distributed apps | Open | | |
### Archived
| Date issued  | Topic | Question | State | (Current) Solution | Next meeting |
| :-----------: | ------------- | --------------------- | ------- | ---------------------- | :---------: |
| | General | Swisscom connections? | Closed | No | |
| | General | DKMS all of it or only key recovery (etc.)?  | Closed | Focus key recovery | |
| | General | SSI / DKMS -> SSI how deep? Key recovery only SSI? | Closed | Solution has to be usable for SSI/FIDO | |
| 03.03.2020 | General | Decentralized vs. distributed (naming) | Closed  | Check glossary | |
| 03.03.2020 | HyperLedger | HyperLedger Aries vs. Indy? | Closed | Check glossary | |
| 03.03.2020 | nuCypher | NuCypher example (called DKMS), what's this? | Closed | Proxy Re-Encryption: Basically, Alice is able to encrypt her data, then let that data be "proxy-reencrypted" by Ursula (untrusted 3rd party) or in NuCyphers case multiple Ursulas (what makes it a **D**KMS). The Ursulas each get a fragment of the reencryption key (sharding similair to shamir secret sharing). Bob then goes to each of the Ursulas and asks for the data. If Alice granted Bob access, Bob needs to find M of N Ursulas to get the data which is decryptable by him. In the process, the data is never decrypted. | |
| 03.03.2020 | Applications | Usable Apps?: Have a look at streetcred.id, keepin, globaliD and other apps | Discontinued | apps.md & Look into streetcred devportal. -> wallet is completely interoperable with aries protocol standard. devportal is easy way to talk to their API to issue credentials etc for aries wallets without writing code (connections, credentials, verifications, organizations..). wallet should be great tool for developing own applications with detailed error messages etc. Nothing for key recovery on the devportal -> email: no solution built in so far, but will also be using mnemonic (bip-0039).|x|
| 09.03.2020 | nuCypher | pyUmbral -> Crypto usable for our case? | Closed | NuCypher does not meet our requirements |  |
| 17.03.2020 | Reclaim:ID | Ask for key recovery options | Done | No solution. They may use anastasis. | |
| 17.03.2020 | Anastasis | Ask whether they are using SSS | Done | No they have their own implementation. | |
| 24.03.2020 | General | Comparing Applications (Dark Crystal, StreetCred.id) or key recovery mechanism? Use cases on Applications or on key recovery mechanism | Closed | More focus on apps or "merge" an SSI app together with a crypto sharing app | |
| 30.03.2020 | General | Comparing Apps with decentralized and social key recovery or all with key recovery | Closed  | It looks like comparing also other mechanism | |
| 17.03.2020 | Social Recovery | Look into social recovery links | Done so far | | |
| 03.03.2020 | HyperLedger | What's necessary to install a HyperLedger Indy blockchain? | Not useful atm | Seems to be pretty easy with docker -> https://github.com/hyperledger/indy-node/blob/master/environment/docker/pool/README.md | |
| 13.04.2020 | Recovery | Key Escrow as recovery technique? | Closed | Still useful ||

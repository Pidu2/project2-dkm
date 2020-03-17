| Date issued  | Topic | Question | State | Date resolved | (Current) Solution | Next meeting |
| :-----------: | ------------- | --------------------- | ------- | :-----------: | ---------------------- | :---------: |
| | General | DKMS all of it or only key recovery (etc.)?  | Closed | | Focus key recovery | |
| | General | SSI / DKMS -> SSI how deep? Key recovery only SSI? | Closed | | Solution has to be usable for SSI/FIDO | |
| | General | Swisscom connections? | Open | | Mrs Laube will check for connections | x |
| 03.03.2020 | General | Decentralized vs. distributed (naming) | Closed  | | Check glossary | |
| 03.03.2020 | Applications | Usable Apps?: Have a look at streetcred.id, keepin, globaliD and other apps | Open | | apps.md & Look into streetcred devportal.| |
| 03.03.2020 | HyperLedger | HyperLedger Aries vs. Indy? | Closed | | Check glossary | |
| 03.03.2020 | HyperLedger | What's necessary to install a HyperLedger Indy blockchain? | Postponed | | https://github.com/hyperledger/indy-node -> As soon as we have the VMs, we could try How-Tos found in this repo| |
| 03.03.2020 | nuCypher | NuCypher example (called DKMS), what's this? | Closed | |Proxy Re-Encryption: Basically, Alice is able to encrypt her data, then let that data be "proxy-reencrypted" by Ursula (untrusted 3rd party) or in NuCyphers case multiple Ursulas (what makes it a **D**KMS). The Ursulas each get a fragment of the reencryption key (sharding similair to shamir secret sharing). Bob then goes to each of the Ursulas and asks for the data. If Alice granted Bob access, Bob needs to find M of N Ursulas to get the data which is decryptable by him. In the process, the data is never decrypted. | |
| 09.03.2020 | nuCypher | pyUmbral -> Crypto usable for our case? | Closed | |NuCypher does not meet our requirements |  |
| 17.03.2020 | procivis | Look/ask for documentation (key recovery) | Open | ||  |
| 17.03.2020 | Applications | Look for applications that actually support social key recovery | Open | | | |
| 17.03.2020 | HyperLedger | Aries implementation w/ social recovery | Open | | | |
| 17.03.2020 | Social Recovery | Look into social recovery links | Open | | | |
| 17.03.2020 | Reclaim:ID | Ask for key recovery options | Open ||||
| 17.03.2020 | Anastasis | Ask whether they are using SSS | Open ||||

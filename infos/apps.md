# Mobile SSI Apps
| name | category | remarks |
|---|---|---|
|keepin|Identity Wallet|<ul><li>Own ecosystem with own DID method and own blockchain</li><li>**Mnemonic recovery** -> full responsibility to safe the "private key & recovery code"</li></ul>|
|uport|Identity Wallet|<ul><li>Based on Ethereum</li><li>Uses the open standards</li><li>**12 word recovery seed phrase**</li><li>Backup to server</li><li>made video and tested</ul>|
|Blockpass User-Controlled Identity|Identity Wallet for their own ecosystem|Completely own ecosystem, recovery by backup PIN|
|Connect.Me - Digital Identity Wallet|Identity Wallet|<ul><li>Sovrin Ecosystem, App by Evernym</li><li>Backup/Restore either in evernym cloud with **recovery phrase** or local backup file with recovery phrase. Altough we've seen that hyperledger indy does seem to support social recovery, it's not built into this app</li><li>"Real" SSI -> No lock-in on Evernym</li></ul>|

# Applications using Social Recovery
| name | category | remarks | tested? |
|---|---|---|---|
|DarkCrystal|Social Network| see glossary|splitting secrets does work with the patchbay version ("Bleeding-edge, tab-based interface with experimental features."). bit of a hassle getting it working though, but secret can be restored. BUT as far as  i understand it: scuttlebutt itself depends on exactly one file to be restorable, which is why you again have the problem of one file that is needed to be kept safe. and currently, the backup of this one is not yet implemented to dark crystal. didnt get darkcrystal-standalone to work|
|Vault12|Crypto App|see play store & whitepaper: https://s3-us-west-1.amazonaws.com/vault12/Vault12+Platform+White+Paper.pdf |open|
|Argent|Crypto Wallet|https://github.com/argentlabs/argent-contracts/blob/develop/specifications/specifications.pdf. Not opensource, not usable for our use case. <br>Everyone get an ENS (.argent.xyz) and has to define 1+ guardians. Guardians can be friend's wallet, hardware token, argent guard... Any guardian can lock wallet for security perdiod of 5 days. On a recovery, a new account is set as the wallet owner. To lock/unlock, 1 guardian is needed, to execute or cancel recovery always (n+1)/2 (round up)|a bit|
|Gnosis|Crypto Wallet|https://gnosis-safe.readthedocs.io/en/latest/contracts/architecture.html -> So far only seed phrase recovery in app...|a bit|
|Steemit|Bitcoin Wallet|https://steemit.com/blockchain/@dan/steemit-releases-groundbreaking-account-recovery-solution -> interesting approach but also has no value for us (besides the approach itself)|no|

# Applications using TSS
| name | category | remarks | tested? |
|---|---|---|---|
|ZenGo|Crypto Wallet| <ul><li>https://zengo.com/security/</li><li>https://zengo.com/security-in-depth/</li><li>Key Recovery: https://zengo.com/how-zengo-guarantees-access-to-customers-funds/</li></ul>|no|

# Applications using Key Escrow
| name | category | remarks | tested? |
|---|---|---|---|
|ZenGo|Crypto Wallet| <ul><li>https://zengo.com/security/</li><li>https://zengo.com/security-in-depth/</li><li>Key Recovery: https://zengo.com/how-zengo-guarantees-access-to-customers-funds/</li></ul>|no|

# Applications using Biometrics
| name | category | remarks | tested? |
|---|---|---|---|
|Offline Vault | Offline Vault |offline backup of seed phrase |no|
|Lastpass|PW Manager|replaceable with other pw managers using biometrics|no|
|Civic|Crypto Wallet|Not released yet - https://www.civic.com/wallet/. Will support biometrics|no|

# OpenSource SSI Apps
| name | remarks |
|---|---|
|SelfKey| Mobile & Desktop both Opensource, Ethereum ledger |
|Element-did | Not entirely sure: https://github.com/decentralized-identity/element |
| Echo| https://github.com/echoprotocol/echo-wallet Desktop |
| uPort | https://github.com/uport-project/uport-mobile |

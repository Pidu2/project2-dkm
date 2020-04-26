# Desktop SSI Apps
| name | category | remarks |
|---|---|---|
|sovrin | CLI Identity wallet | 32 characters seed phrase for recovery |
|bryk|CLI identity wallet | seems to have planned social recovery, is only cli and does not really work..?|
|JLINC|DID CLI client | no recovery, very minimal|


# Mobile SSI Apps
| name | category | remarks |
|---|---|---|
|streetcred.id|Identity Wallet|<ul><li>Donated Code to Aries Project</li><li>Supports Sovrin but also integrates to any other Hyperledger Indy network</li><li>Works with open standards</li><li>Free to use in a test environment</li><li>Recovery not really clear, referencing on the recovery options from indy github</li></ul>|
|keepin|Identity Wallet|<ul><li>Own ecosystem with own DID method and own blockchain</li><li>Mnemonic recovery -> full responsibility to safe the "private key & recovery code"</li></ul>|
|globaliD|Identity Wallet + Platform|Own ecosystem, recovery by "vaults" hosted by 3rd parties as far as I understand it -> mail sent for more infos -> not usable at the moment|
|uport|Identity Wallet|<ul><li>Based on Ethereum</li><li>Uses the open standards</li><li>12 word recovery seed phrase</li><li>Backup to server</li><li>made video and tested</ul>|
|Blockpass User-Controlled Identity|Identity Wallet for their own ecosystem|Completely own ecosystem, recovery by backup PIN|
|One Identity Digital Passport|App for their Ecosystem|Not using open standards, no real "open" documentation|
|Connect.Me - Digital Identity Wallet|Identity Wallet|<ul><li>Sovrin Ecosystem, App by Evernym</li><li>Backup/Restore either in evernym cloud with recovery phrase or local backup file with recovery phrase. Altough we've seen that hyperledger indy does seem to support social recovery, it's not built into this app</li><li>"Real" SSI -> No lock-in on Evernym</li></ul>|
|EarthId|Identity Wallet|Password based backup - no reply on chat|
|Farmer Connect |Identity for Farmers| mail sent |
|IdRamp |Identity Wallet| mail sent |
|HearRo |Phone System| mail sent |
|Axuall |Identity for Health Organizations| mail sent |
|truu.id |Identity for Health Organizations| mail sent |
|B!Wallet |Identity Wallet| mail sent |
|Keyless |Identity Wallet| not yet implemented |
|Sygnet |e-receipts via SSI| no information |
|Spaceman.id |Identity wallet| mail sent |
|Snapper Future Tech |Identity wallet| mail sent |
|ABT Wallet|Identity Wallet| <ul><li>mail sent</li><li>made video and tested</li><li>seems to support local backup only</li></ul>|
|Ontology ID Wallet|Identity and Crypto Wallet| <ul><li>tested</li><li>password based backup only</li></ul>|
|DPASS |Identity and Crypto Wallet| <ul><li>made video and tested</li><li>password based local backup or </li><li>Verification process with Email and Mobile to restore from vault</li></ul>|
|SelfKey |Identity Wallet| plans to set on uPort for recovery. talks about something like social recovery but not yet implemented neither in uport nor selfkey|
|Jolocom|Identity Wallet|seed phrase recovery|
|Alastra|?|according to schlup/scheck mobile app, did not find it, no information found either|

# Other mobile app
| name | category | remarks |
|---|---|---|
|Voice |Social app| mail sent |
|longplay.me |Crypto mobile wallet| mail sent |

# Applications using Social Recovery
| name | category | remarks | tested? |
|---|---|---|---|
|DarkCrystal|Social Network| see glossary|no|
|Argent|Ethereum Wallet|see glossary|no|
|Zion|HTC Exodus|see links|no - we can't|
|(Threshcrypt)|File Encryption|Only SSS, not Social Recovery...https://github.com/ryancdotorg/threshcrypt |no|
|(Vaultproject)|Secret Store|Only SSS, not Social Recovery...https://www.vaultproject.io/ |no|
|Vault12|Crypto Mobile App|see play store & whitepaper: https://s3-us-west-1.amazonaws.com/vault12/Vault12+Platform+White+Paper.pdf|open|

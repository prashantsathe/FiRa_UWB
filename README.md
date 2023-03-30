# Fira

## Implementeded FiRa features

* Secure channel protocols
* SC1/SC2(SC2 is not integrated with FiRa applet)
* SCP11C
* All FiRa commands implementations except Store Data
* ADF and Key Provisioning
* Host application to remote service applet command Routing
*  Ranging data set generation and transfer to SUS applet
* All cryptographic operations
* Session key based on cmac kdf counter mode
* SC2 root key based on cmac kdf counter mode
* SCP03 key derivation
* Cipher based on AES 128 block with cbc no pad
* Cmac based on AES 128 block
* Signature verification based on ECDSA plain using message digest 256
* Test applet to test FiRa secure channel interface
* Test service applet

## Implemented SUS features

* All Sus internal and external commands
* Secure channel communication with UWBs using SD’s SCP11a and SCP03 protocol
* Jcop test scripts to test all Sus commands based on SCP11a & SCP03 protocol
* FiRa development test suite (unit tests)
* Connect two Jcop simulators simultaneously
* Initiate provisioning process including ADF creation
* Initiate FiRa SC1 establishment and RDS generation/exchange
* Command routing
* Read RDS data using SCP03 protocol

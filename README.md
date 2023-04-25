# Fira

Repo links

https://github.com/prashantsathe/FiRa/tree/jcop_master

https://github.com/prashantsathe/SusApplets/tree/Jcop_master (private)

## Overview

FIRA Applet is a Javacard 3.0.5 compliant and Global Platform 2.3 compliant Secure Element (SE) Card applet, which implements the FIRA specifications[CSML]. It is a subsystem in FIRA CSML Architecture and it is only required for supporting UWB Dynamic STS based ranging sessions. Accordingly, the main purpose of this applet is as follows:
Generate a session key (or sub-session keys), which is used to secure the UWB ranging sessions that use dynamic STS.
Securely exchange the session key securely with peer FIRA applets along with other information in both unicast and multicast ranging scenarios. 
Enable secure exchanging of UWB Application specific information with other FIRA compliant devices.
The secure exchange includes establishing, secure channel which is mutually authenticated and encrypted as specified in the FIRA specifications[CSML]. 
Following reference documents provide background and technical information to understand the SUS Applet design.


[JC]  Javacard 3.0.5 Specifications.

[CSML] .FIRA CSML Specifications

[GP] Global Platform 2.3 Specifications.

[AMD-H] Global Platform Amendment H.

[SCP03] Global Platform SCP03 Specifications.

[SCP11] Global Platform SCP11 Specifications.

[SE] ISO 7816-4 2020 Specifications.

[SUS] FiRA SUS Applet Specifications.

[SUS API] FIRA SUS Internal API Specifications. 

[FW] FIRA FW Design for Dynamic STS.

[UML] Unified Modeling Language.

[OMAPI] Open Mobile API Specification.

[ARA] SE Access Control.

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

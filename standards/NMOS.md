> [Click here](/README.md) to go back to the start
 
# NMOS

## Contents
- [NMOS](#nmos)
  - [Contents](#contents)
  - [The Standard](#the-standard)
  - [Specifications](#specifications)
    - [IS-04 "Discovery and Registration"](#is-04-discovery-and-registration)
    - [IS-05 Device "Connection Management"](#is-05-device-connection-management)
    - [IS-07 "Event \& Tally"](#is-07-event--tally)
    - [IS-08 "Audio Channel Mapping"](#is-08-audio-channel-mapping)
    - [IS-09 "System Parameters"](#is-09-system-parameters)
    - [BCP-003](#bcp-003)
      - [BCP-003-01 "Secure API communications"](#bcp-003-01-secure-api-communications)
      - [BCP-003-02 "Authorization"](#bcp-003-02-authorization)
      - [BCP-003-03 "Certificate Provisioning"](#bcp-003-03-certificate-provisioning)
    - [IS-10 "Authorization"](#is-10-authorization)
  - [Recommended Practices](#recommended-practices)
    - [INFO-002](#info-002)
  - [Tools](#tools)


## The Standard
The Networked Media Open Specifications (NMOS) provide an open and simple to use control-plane solution that enables interoperability and management of IP connected audio and video devices.

## [Specifications](https://specs.amwa.tv/nmos/)

### [IS-04 "Discovery and Registration"](https://specs.amwa.tv/is-04/)
Allows control and monitoring applications to find the resources on a network

### [IS-05 Device "Connection Management"](https://specs.amwa.tv/is-05/)
Provides a transport-independent way of connecting Media Nodes

### [IS-07 "Event & Tally"](https://specs.amwa.tv/is-07/)
Provides an IP-friendly mechanism to carry time-sensitive information

### [IS-08 "Audio Channel Mapping"](https://specs.amwa.tv/is-08/)
Allows channel-level operations within NMOS environments
~How to set channel mapping/selecting/shuffling settings for use with NMOS APIs.~

### [IS-09 "System Parameters"](https://specs.amwa.tv/is-09/)
Allows an NMOS Node (also known as a “Media Node”) to obtain global configuration parameters that are common across the system.

### BCP-003
Foundations for securing the control plane. Ensures that encryption is sufficient, is built upon wider best practice, and is interoperatble.

#### [BCP-003-01 "Secure API communications"](https://specs.amwa.tv/bcp-003-01/)
Documents best practice for using secure transport for NMOS API communications.

#### [BCP-003-02 "Authorization"](https://specs.amwa.tv/bcp-003-02/)
Documents best practice for an API server to accept or reject requests depending on what a client is authorized to do.

#### [BCP-003-03 "Certificate Provisioning"](https://specs.amwa.tv/bcp-003-03/)
Documents best practice for automated provisioning of TLS Server Certificates to NMOS APIs.

### [IS-10 "Authorization"](https://specs.amwa.tv/is-10/)
Allows an API server to accept or reject requests depending on what a client is authorized to do

## Recommended Practices
### [INFO-002](https://specs.amwa.tv/info-002/)
Guide for implementers who want to add security to their NMOS Nodes and/or NMOS Controllers, according to the IS-10, BCP-003-01, BCP-003-02 and BCP-003-03 specifications.

## Tools
- [Pebble Control Free](https://www.pebble.tv/control-free/about/): Self-contained, scalable and easy to configure IP connection manager.
- [nmos-cpp](https://github.com/sony/nmos-cpp): Sony's NMOS Registry and Node Implementation in C++.
- [nmos-js](https://github.com/sony/nmos-js): Sony's NMOS Client Implementation in Javascript.
- [BBC's NMOS Authorisation Server Implementation](https://github.com/bbc/nmos-auth-server): A Flask-based implementation of an OAuth2 Authorisation Server based on [AMWA NMOS BCP-003-02](https://amwa-tv.github.io/nmos-api-security/best-practice-authorisation.html) using [RFC 6749](https://tools.ietf.org/html/rfc6749).
- [Ledger](https://github.com/Streampunk/ledger): Node.js Javascript implementation of the NMOS discovery and registration APIs.
- [Easy-NMOS Docker Compose Solution](https://github.com/rhastie/easy-nmos): Easy NMOS setup using Docker compose
- [NMOS-TESTING](https://specs.amwa.tv/nmos-testing/): Testing tool for the AMWA NMOS Specifications ([GitHub Repo](https://github.com/AMWA-TV/nmos-testing))
- [The Business Benefits of DNS-SD for NMOS](http://static.amwa.tv/business-benefits-of-nmos-plus-dns-sd.pdf): Why DNS Service Discovery in an NMOS environment?
- [NMOS Web Router](https://github.com/bbc/nmos-web-router): A web based application for connecting multicast RTP Senders and Receivers using AMWA NMOS IS-04 and IS-05. 
- https://github.com/AMWA-TV/sdpoker
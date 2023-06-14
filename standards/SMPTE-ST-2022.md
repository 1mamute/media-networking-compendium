> [Click here](/README.md) to go back to the start
 
# SMTPE ST 2022

## Contents
- [SMTPE ST 2022](#smtpe-st-2022)
  - [Contents](#contents)
  - [The Standard](#the-standard)
  - [Documents](#documents)
    - [ST 2022-1:2007 “Forward Error Correction for Real-Time Video/Audio Transport Over IP Networks”](#st-2022-12007-forward-error-correction-for-real-time-videoaudio-transport-over-ip-networks)
    - [ST 2022-2:2007 “Unidirectional Transport of Constant Bit Rate MPEG-2 Transport Streams on IP Networks”](#st-2022-22007-unidirectional-transport-of-constant-bit-rate-mpeg-2-transport-streams-on-ip-networks)
    - [ST 2022-3:2010 “Unidirectional Transport of Variable Bit Rate MPEG-2 Transport Streams on IP Networks”](#st-2022-32010-unidirectional-transport-of-variable-bit-rate-mpeg-2-transport-streams-on-ip-networks)
    - [ST 2022-4:2011 “Unidirectional Transport of Non-Piecewise Constant Variable Bit Rate MPEG-2 Streams on IP Networks”](#st-2022-42011-unidirectional-transport-of-non-piecewise-constant-variable-bit-rate-mpeg-2-streams-on-ip-networks)
    - [ST 2022-5:2012 “Forward Error Correction for High Bit Rate Media Transport Over IP Networks”](#st-2022-52012-forward-error-correction-for-high-bit-rate-media-transport-over-ip-networks)
    - [ST 2022-5:2013 - "Forward Error Correction for Transport of High Bit Rate Media Signals over IP Networks (HBRMT)"](#st-2022-52013---forward-error-correction-for-transport-of-high-bit-rate-media-signals-over-ip-networks-hbrmt)
    - [ST 2022-6:2012 “Transport of High Bit Rate Media Signals over IP Networks (HBRMT)”](#st-2022-62012-transport-of-high-bit-rate-media-signals-over-ip-networks-hbrmt)
    - [ST 2022-7:2013 “Seamless Protection Switching of SMPTE ST 2022 IP Datagrams”](#st-2022-72013-seamless-protection-switching-of-smpte-st-2022-ip-datagrams)
    - [ST 2022-8:2019 "Timing of ST 2022-6 Streams in ST 2110-10 Systems"](#st-2022-82019-timing-of-st-2022-6-streams-in-st-2110-10-systems)
    - [ST 2022-2:2019 "Unidirectional Transport of Constant Bit Rate MPEG-2 Transport Streams on IP Networks (????)"](#st-2022-22019-unidirectional-transport-of-constant-bit-rate-mpeg-2-transport-streams-on-ip-networks-)
    - [ST 2022-3:2019 "Unidirectional Transport of Variable Bit Rate MPEG-2 Transport Streams on IP Networks"](#st-2022-32019-unidirectional-transport-of-variable-bit-rate-mpeg-2-transport-streams-on-ip-networks)
    - [ST 2022-7:2019 "Seamless Protection Switching of RTP Datagrams"](#st-2022-72019-seamless-protection-switching-of-rtp-datagrams)

## The Standard
The SMPTE ST 2022 suite of standards provides a reliable way of using IP to transmit signals that were traditionally sent over serial interfaces.

## Documents

### [ST 2022-1:2007 “Forward Error Correction for Real-Time Video/Audio Transport Over IP Networks”](https://ieeexplore.ieee.org/document/7291470)
Defines a forward error correction technique for the carriage of real-time Video/Audio content over IP networks. <details><summary>Rough Explanation</summary>_Defines row/column FEC (Forward Error Correction) for IP video streams. Along with Section 2, this standard has been widely implemented. Row/Column FEC works by grouping IP video packets into logical rows and columns, and then appending one FEC packet to each row and each column.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-2:2007 “Unidirectional Transport of Constant Bit Rate MPEG-2 Transport Streams on IP Networks”](https://ieeexplore.ieee.org/document/7291740)
Defines a unidirectional transport protocol for the carriage of real-time [_Constant Bitrate (CBR)_](/README.md#cbr) MPEG-2 Transport Streams over IP networks. <details><summary>Rough Explanation</summary>_Specifies how constant bit rate compressed video signals that are encoded within MPEG-2 transport streams are encapsulated into IP packets. This standard covers the transport layer (RTP and UDP) as well as comments about timing and buffer sizes.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-3:2010 “Unidirectional Transport of Variable Bit Rate MPEG-2 Transport Streams on IP Networks”](https://ieeexplore.ieee.org/document/7290021)
Defines a transport protocol for the carriage of real-time [_piecewise constant variable bit rate (VBR)_](/README.md#piecewise-vbr) MPEG-2 Transport Streams over IP networks, either with or without Forward Error Correction for recovery from network transmission errors. <details><summary>Rough Explanation</summary>_Defines IP packets for variable bit-rate MPEG-2 TS streams that are constrained to have a constant bit rate between PCR messages (called piecewise-constant).[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-4:2011 “Unidirectional Transport of Non-Piecewise Constant Variable Bit Rate MPEG-2 Streams on IP Networks”](https://ieeexplore.ieee.org/document/7290516)
Defines a transport protocol for the carriage of real-time [_non-piecewise constant variable bit rate (VBR)_](/README.md#non-piecewise-vbr) MPEG-2 Transport Streams over IP networks, either with or without Forward Error Correction for recovery from network transmission errors. <details><summary>Rough Explanation</summary>_Similar to Section 3, except that it removes the constraint on bit rates.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-5:2012 “Forward Error Correction for High Bit Rate Media Transport Over IP Networks”](https://ieeexplore.ieee.org/document/7291908)
Defines a forward error correction technique for the carriage of High Bit Rate real-time media over IP networks. <details><summary>Rough Explanation</summary>_Expands on Section 1 to allow larger row/column FEC combinations to support signals with bit rates up to 3 Gbps and beyond.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-5:2013 - "Forward Error Correction for Transport of High Bit Rate Media Signals over IP Networks (HBRMT)"](https://ieeexplore.ieee.org/document/7291590)
Revision of ST 2022-5:2013. <details><summary>Rough Explanation</summary>TODO: What changed?</details>

### [ST 2022-6:2012 “Transport of High Bit Rate Media Signals over IP Networks (HBRMT)”](https://ieeexplore.ieee.org/document/7289943)
Defines a unidirectional IP-based protocol for the transport of real-time video, audio, and ancillary signals. <details><summary>Rough Explanation</summary>_Specifies a way to transport high bit-rate signals (including uncompressed 3 Gbps 1080p video) that are not encapsulated in MPEG-2 transport streams.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-7:2013 “Seamless Protection Switching of SMPTE ST 2022 IP Datagrams](https://ieeexplore.ieee.org/servlet/opac?punumber=7291849)”
Defines requirements for redundant streams of SMPTE 2022 packets to allow for creation of a single reconstructed output stream through seamless protection switching at the RTP datagram level. <details><summary>Rough Explanation</summary>_Describes a way to send two matching streams of packets from a source to a destination over different paths, and have the receiver switch automatically between them. This allows a perfect video signal to be reconstructed at the receiver as long as both paths do not fail simultaneously.[[1]](https://web.archive.org/web/20151208160422/http://www.tvtechnology.com/insight/0083/smpte--and-the-future-of-video-over-ip/220188)_</details>

### [ST 2022-8:2019 "Timing of ST 2022-6 Streams in ST 2110-10 Systems"](https://ieeexplore.ieee.org/document/8716819)
Specifies the use and constraints for SMPTE ST 2022-6 streams in conjunction with the timing model of SMPTE ST 2110-10, including definition of a Synchronizing Timestamp derived in the ST 2022-8 receiver to relate the two standards. It also documents the SDP announcement of SMPTE ST 2022-5 FEC and SMPTE ST 2022-7 redundancy for these streams. <details><summary>Rough Explanation</summary>_TODO_</details>

### [ST 2022-2:2019 "Unidirectional Transport of Constant Bit Rate MPEG-2 Transport Streams on IP Networks (????)"](https://ieeexplore.ieee.org/document/7291740)
Listed in the [SMPTE Standards list](https://www.smpte.org/standards/document-index/st#listing) but the hyperlink points to the ST 2022-2:2007 paper.

### [ST 2022-3:2019 "Unidirectional Transport of Variable Bit Rate MPEG-2 Transport Streams on IP Networks"](https://ieeexplore.ieee.org/document/8813131)
Revision of ST 2022-3:2010. <details><summary>Rough Explanation</summary>TODO: What changed?</details>

### [ST 2022-7:2019 "Seamless Protection Switching of RTP Datagrams"](https://ieeexplore.ieee.org/document/8716822)
Revision of ST 2022-7:2013. <details><summary>Rough Explanation</summary>TODO: What changed?</details>

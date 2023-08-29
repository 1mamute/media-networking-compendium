> [Click here](/README.md) to go back to the start
 
# SMTPE ST 2110

## Contents
- [SMTPE ST 2110](#smtpe-st-2110)
  - [Contents](#contents)
  - [The Standard](#the-standard)
  - [Specifications](#specifications)
    - [ST 2110-10:2017 "System Timing and Definitions"](#st-2110-102017-system-timing-and-definitions)
    - [ST 2110-20:2017 "Uncompressed Active Video"](#st-2110-202017-uncompressed-active-video)
    - [ST 2110-30:2017 "PCM Digital Audio"](#st-2110-302017-pcm-digital-audio)
    - [ST 2110-21:2017 "Traffic Shaping and Delivery Timing for Video"](#st-2110-212017-traffic-shaping-and-delivery-timing-for-video)
    - [ST 2110-31:2018 "AES3 Transparent Transport"](#st-2110-312018-aes3-transparent-transport)
    - [ST 2110-40:2018 "SMPTE ST 291-1 Ancillary Data"](#st-2110-402018-smpte-st-291-1-ancillary-data)
    - [ST 2110-43:2021 "Timed Text Markup Language for Captions and Subtitles":](#st-2110-432021-timed-text-markup-language-for-captions-and-subtitles)
    - [ST 2110-22:2022 "Constant Bit-Rate Compressed Video"](#st-2110-222022-constant-bit-rate-compressed-video)
  - [Recommended Practices](#recommended-practices)
    - [RP 2110-23:2019 "Single Video Essence Transport over Multiple ST 2110-20 Streams"](#rp-2110-232019-single-video-essence-transport-over-multiple-st-2110-20-streams)
    - [SMPTE RP 2110-25](#smpte-rp-2110-25)
    - [JT-NM TR1001-1 "System Environment and Device Behaviors for ST 2110 Media Nodes in Engineered Networks"](#jt-nm-tr1001-1-system-environment-and-device-behaviors-for-st-2110-media-nodes-in-engineered-networks)


## The Standard

The SMPTE ST 2110 suite of standards specifies the carriage, synchronization, and description of separate elementary essence streams over IP for real-time media applications. Each stream is individually timed by the ST 2110 system and can take different routes over the networked fabric to arrive via unicast or multicast at one or more receivers. The audio-video-data synchronization using PTP clocks ensures that the accurate synchronization of all streams regardless of how the packets were routed.


## Specifications
### [ST 2110-10:2017 "System Timing and Definitions"](https://ieeexplore.ieee.org/document/8165974)
This family of engineering documents defines an extensible system of RTP-based essence streams referenced to a common reference clock, in a manner which specifies their timing relationships. — This standard specifies the system timing model and the requirements common to of all of the essence streams. <details><summary>Rough Explanation</summary>_defines transport layer and synchronization (SMPTE2059, clocks, RTP, SDP etc.)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-20:2017 "Uncompressed Active Video"](https://ieeexplore.ieee.org/document/8167389)
The real-time, RTP-based transport of uncompressed active video essence over IP networks. An SDP-based signaling method is defined for image technical metadata necessary to receive and interpret the stream. <details><summary>Rough Explanation</summary>_defines payload format for raw video (RFC4175, RTP, SDP, constraints)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-30:2017 "PCM Digital Audio"](https://ieeexplore.ieee.org/document/8167392)
The real-time, RTP-based transport of PCM digital audio streams over IP networks by reference to AES67. An SDP-based signaling method is defined for metadata necessary to receive and interpret the stream. Non-PCM digital audio signals including compressed audio signals are outside the scope of this standard. <details><summary>Rough Explanation</summary>_defines payload format for linear audio (AES67, constraints)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-21:2017 "Traffic Shaping and Delivery Timing for Video"](https://ieeexplore.ieee.org/document/8165971)
A timing model for SMPTE ST 2110-10 video RTP streams as measured leaving the RTP sender, and defines the sender SDP parameters used to signal the timing properties of such streams. <details><summary>Rough Explanation</summary>_ defines timing model for senders and receivers (traffic shaping requirements)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-31:2018 "AES3 Transparent Transport"](https://ieeexplore.ieee.org/document/8454952)
The real-time, RTP-based transport of AES3 signals over IP networks, referenced to a network reference clock. <details><summary>Rough Explanation</summary>_defines payload format for non-linear audio (RAVENNA AM824)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-40:2018 "SMPTE ST 291-1 Ancillary Data"](https://ieeexplore.ieee.org/document/8353279)
The real-time, RTP payload based transport of SMPTE ST 291-1 Ancillary (ANC) Data packets related to digital video data streams, over IP networks, referenced to a common reference clock. <details><summary>Rough Explanation</summary>_defines RTP payload format for SDI ancillary data (new IETF draft)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### [ST 2110-43:2021 "Timed Text Markup Language for Captions and Subtitles"](https://ieeexplore.ieee.org/document/9521125):
The real-time, RTP-based transport of Timed Text Markup Language for captions and subtitles in systems conforming to SMPTE ST 2110-10. <details><summary>Rough Explanation</summary>_TODO_</details>

### [ST 2110-22:2022 "Constant Bit-Rate Compressed Video"](https://ieeexplore.ieee.org/document/9893780)
The real-time, RTP-based transport of constant bit-rate compressed video over IP networks, referenced to a common reference clock. <details><summary>Rough Explanation</summary>_defines payload format for CBR compressed video and a SMPTE registry for
various payload formats (codecs)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

## Recommended Practices

### [RP 2110-23:2019 "Single Video Essence Transport over Multiple ST 2110-20 Streams"](https://ieeexplore.ieee.org/document/8984684)
The document proposes a methodology to (i) split high bandwidth single video essence streams into several lower bandwidth SMPTE ST 2110-20 tributary streams , and (ii) to describe the appropriate grouping and signaling of these multiple SMPTE ST 2110-20 streams (SDP declarations, addressing conventions, RTP time stamp constraints, …).<details><summary>Rough Explanation</summary>_defines how to split high-bandwidth signals into several lower-bandwidth
2110-20 tributary streams(constraints, grouping, addressing, RTP timestamps, SDP …)[[1]](https://www.aimsalliance.org/wp-content/uploads/2019/02/4.-AIMS-Reception-ISE-2019-ST2110-explained-Hildebrand.pdf)_</details>

### SMPTE RP 2110-25

### [JT-NM TR1001-1 "System Environment and Device Behaviors for ST 2110 Media Nodes in Engineered Networks"](https://static.jt-nm.org/documents/JT-NM_TR-1001-1_2020_v1.1.pdf)
Technical Recommendation paper from JT-NM with a "goal to enable the creation of network environments where an end-user can take delivery of (recommended) equipment, connect it to their network, and configure it for use, with a minimum amount of human interaction."
---
layout: post
title: Using non-Cisco GBIC on Catalyst 9200
tags: cisco networking
---

The "service unsupported-transceiver" command is broken on Cisco Catalyst series running IOS version 16.9.X [1].

Worry not, without updating the IOS version we can still prevent the SFP ports from entering an err-disabled state by issuing the `no errdisable recovery cause gbic-invalid` command [2]. I've tested with FS and Cables and Kits branded Cisco "compatible"  transceivers and not encountered any issues.

[1] [https://quickview.cloudapps.cisco.com/quickview/bug/CSCvk03296](https://quickview.cloudapps.cisco.com/quickview/bug/CSCvk03296)  
[2] [https://www.reddit.com/r/networking/comments/f01htf/cisco_9200_service_unsupportedtransceiver_error/](https://www.reddit.com/r/networking/comments/f01htf/cisco_9200_service_unsupportedtransceiver_error/)

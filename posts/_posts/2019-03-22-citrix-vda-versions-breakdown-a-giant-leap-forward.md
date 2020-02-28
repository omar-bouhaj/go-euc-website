---
layout: post
title:  "Citrix VDA versions breakdown, a giant leap forward"
authors: [eltjo]
categories: [ 'citrix', 'VDA', 'firefox', 'chrome', 'browers']
image: assets/images/posts/005-citrix-vda-versions-breakdown-a-giant-leap-forward/021-citrix-vda-compare-feature-image.png
---
With each iteration of the Citrix Virtual Delivery Agent (VDA) software Citrix always treats us to new features and functionalities. For the Current Releases (CR) Citrix is constantly adding new features and functionalities while also improving the performance of the HDX protocol itself. This should, in theory, result in a better user experience, coupled with a higher user density and less strain on the system.

> **Disclaimer:** These results have been affected by the Login VSI progress bar and results may be different in practice. For more information please read the following [post]({{site.baseurl}}/important-influence-of-citrix-login-vsi-on-the-results/).

The Long Term Service Release (LTSR) program provides stability and long-term support for XenApp and XenDesktop releases. XenApp and XenDesktop LTSRs are currently available for Versions 7.6 and 7.15. Cumulative Update 3 (CU3) is the most recent update to the 7.15 LTSR.

Since the last LTSR release, Citrix has shipped five CRs: 7.16, 7.17, 7.18, 7 1808.2 and 7 1811.1.

Version 7 1808.2 is the first version to use not only the new product naming but also the new version naming scheme. For the sake of clarity, we will refer to Virtual Apps and Desktops for all product versions in this post.

In this research we will focus on the lasted latest three CRs from that list and compare them to the lasted latest two cumulative updates for 7.15 LTSR which at the time of writing are CU2 and CU3.

This means that there are five scenarios in total:

  * Desktop OS VDA version 7.15 LTSR CU2
  * Desktop OS VDA version 7.15 LTSR CU3
  * Desktop OS VDA version 7.18
  * Desktop OS VDA version 7 1808.2
  * Desktop OS VDA version 7 1811.1

## What’s new
To get some context for the different VDA versions here is a small breakdown of some of the more notable VDA improvements and new features that we suspect can have an impact on the user experience or the server scalability of the environment:


| Version | Feature | Remark | 
| :-----: | :-----: | :----: |
| 7.18 | Battery icon notification | While not necessarily performance related a very much requested feature nonetheless |
| 7.18 | Enhanced server VDA webcam functionality | Thinwire enhancements (‘Build to lossless’ preference of the Visual quality policy setting is now H.264 instead of JPEG for moving images) | 
| 7.18 | H.264 | Build-to-Lossless |
| 1808.2 | Better network throughput over high latency connection | [https://support.citrix.com/article/CTX125027](https://support.citrix.com/article/CTX125027) |
| 1808.2 | Chrome enhancement to browser content redirection | Browser content redirection now supports the Chrome browser in addition to the previously supported Internet Explorer browser |
| 1808.2 | NVENC video encoding support on Server OS VDAs | NVENC video encoding support on Server OS VDAs. The XenApp and XenDesktop 7.17 release introduced Desktop VDA support for selective H.264/H.265 encoding with NVIDIA NVENC GPUs. 
In this release, the similar capabilities have now been extended to Server OS VDAs equipped with NVIDIA NVENC GPUs |
| 1811.1 | Graphics status indicator | The Graphics status indicator policy has been updated to replace the display lossless indicator policy |
| 1811.1 |DPI matching on Windows 10 | DPI matching allows the Windows 10 desktop session to match the DPI of the endpoint when using Citrix Workspace app for Windows. |
| 1811.1 | HDX adaptive throughput | HDX adaptive throughput intelligently fine-tunes the peak throughput of the ICA session by adjusting output buffers. The number of output buffers is initially set at a high value.
This high value allows data to be transmitted to the client more quickly and efficiently, especially in high latency networks. Providing better interactivity, faster file transfers, smoother video playback, higher framerate and resolution results in an enhanced user experience. |

cjkncdjkk
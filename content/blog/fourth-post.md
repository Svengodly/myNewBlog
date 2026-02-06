---
author: Rickey Morris
title: Wrangling Cables
date: 2024-04-18T11:26:10-04:00
draft: false
# layout:
description: Come right on in and pull the plug.
tags: ["blog"]
# icon:
thumbnail:
    url: images/t568.jpg
    author: Lee Lawson
    # authorURL:
    # origin:
    # originURL:
---

Recently, we switched from a third-party carrier with several PCs, printers, and other devices hard-wired to our network via ethernet cables. Our policy calls for these connections to be physically secure within a cabinet. That means no one without authorization should be able to tamper with any of the cables connected to said cabinet. Upon visiting this cabinet, however, I was shocked to find one of the cabinet doors wide open with cables crawling out of it. The third party had its enclosure with its switch outside our cabinet, and they ran the wires out of the front door of our cabinet to their network enclosure. Any malicious actor had unfettered access to the exposed entrails of our cabinet. I needed to act urgently.

The swiftest, albeit reckless, solution would have been to cut the wires coming through the open door. Fortunately, the third party no longer needed to use their network box. They abandoned it with the switch that lay inside, with most of its LEDs now dormant. I decided to fluke the wires from their (now our) switch to wherever they terminated in the cabinet. The cables would be connected to one of our four patch panels, right? Nope. They were lying on the bottom of the cabinet, with their ends terminated with a keystone. One of our patch panels is a keystone panel, a type of patch panel that can accommodate several different connector types ranging from HDMI, coaxial, fiber, and more. I don't know why they didn't use this panel since it had over a dozen slots with empty keystones, but I did to clean up the shoddy work.

After replacing the unused keystones with the ones lying at the bottom, I was able to shut the other door of the cabinet and lock it down. A huge sigh of relief. Up to this point, I had practically no experience with cable management at an enterprise level. I had only the theory and knowledge gleaned from books and the Web. So these opportunities are most welcome. There are improvements that I am in the process of making, such as labeling all of our data drops in our network diagram and their corresponding wall jacks. No one should have to fluke a cabinet if it is well organized and tidy.

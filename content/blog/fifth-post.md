---
author: Rickey Morris
title: Predicting a Drive's Failure
date: 2024-05-01T14:39:31-04:00
draft: false
description: Keep tabs on the health of your drives.
tags: ["blog"]
---
Have you ever had a hard drive kick the bucket and lose all of your data? That happened to one of my Western Digital hard drives. Fortunately, that drive only contained games from my Steam Library that I could redownload any time. Aside from the audible clanking foreshadowing the failure of my hard drive, another tool suggested the hard drive was on its last legs.(Self-Monitoring, Analysis, and Reporting Technology) is a tool embedded in HDDs and SDDs that allows storage devices to provide metrics to gauge their health. These values, which may vary by vendor, include Read Error Rate, Reallocated Sectors Count, Power-On Hours, and many more. There are several ways to query this data from your storage device. The following is geared towards Windows, so the software mentioned may only be available on Windows. Crystal Disk, for example, is only available on Windows and not Mac or Linux. Also, if you are not yet performing routine backups of your data, begin with that first.

Crystal Disk is a third-party piece of software created by Noriyuki Miyazaki with a GUI. It is vendor-agnostic, which means you may use it to obtain S.M.A.R.T data from the gamut of PC storage manufacturers. If your rig has storage devices from different companies, then you may want to opt for this option.

Vendors also provide software that queries S.M.A.R.T. data. Samsung has Magician, and Western Digital has Digital Dashboard. Vendor software ensures that you have data tailored to a specific device. Also, this provides a straightforward method of updating the firmware of your storage devices.

PowerShell can query generic S.M.A.R.T. information. While this option lends itself to scripting, it is not as intuitive for the everyday user. Note that some commands, like the Get-StorageReliablityCounter, require you to run PowerShell as admin. Pipe either of the following commands to Get-Member to display all the properties. You can then use Select-Object to filter out the properties you want shown.

Get-Disk
Get-Disk | Get-StorageReliabilityCounter
Get-CimInstance Win32_DiskDrive

WMIC (Windows Management Instrumentation for the Command Line) is another option, but Microsoft deprecated it several years ago. It is now a part of Microsoft's Features on Demand.

---
author: Rickey Morris
title: The Death of a Hard Drive
date: 2023-12-07T13:01:26-05:00
description: An ounce of prevention is worth a pound of cure.
tags: ["blog"]
---
### I implore you…BACK UP YOUR DATA!

Well, it finally happened. My 2TB Hard Disk Drive died on me. It does not show in Windows, Ubuntu, or in BIOS. Also, it now makes a reoccurring clicking noise every 2 – 3 seconds. I read several stories of other individuals who experienced sudden hard drive failures, but of course I never thought that a hard drive would ever fail on me before I got a chance to upgrade from my current PC that I built back in 2015 (I had an Xbox 360 with a hard drive that would corrupt save data when it was shut down. Fun times). Yes, this hard drive lasted for 8 years before kicking the bucket so maybe I deserved it. I was well aware that most cites state that hard drives typically fail within 3 - 5 years, but I continued to delay back ups anyway. The silver lining is that the hard drive did not contain any crucial files. It was mainly used to store data-hungry games from my Steam Library. However, I took this as a lesson learned and I began researching tools and services that I can use to ensure that I am adequately prepared in case this event occurs again. Hopefully, the information that I will include here will be of use to you and I will continue to make addendums as I expand my knowledge and get hands-on time with some of the tools mentioned here. But first let us start with some considerations that need to be taken into account like why even perform backups in the first place? Should be a pretty obvious answer but some of us *cough* *cough* may be negligent.

March 31st is known as World Backup Day, and it was created in 2011 to raise awareness of the importance of taking measures to prevent data loss.

### Why to Perform Backups

If the above anecdote was not clear, backups need to be performed in preparation for contingencies that could result in a loss of data. This could be a sudden failure of the hard drive, corrupt data, malware, or physical damage. A backup allows you to restore your information in the event that it is lost or compromised.

Corporations may be required by law or policy to retain archives of data for a certain period of time for auditing or various other reasons. The Sarbones-Oxley Act and Health Insurance Portability and Accountability Act are two examples.

### What to Backup

To aid in identifying what data would benefit from a backup, there are a couple of questions you can ask yourself. How often does a file or folder change? Is it daily, weekly, or monthly? What are the ramifications if a file or folder is compromised or lost? Are there crucial documents or media that holds a sentimental value? Generally, you want to back up your personal files, which are all usually located in C:\Users\username. Fortunately, Windows 10 has a useful backup tool called File History which includes many of the files and folders that you may want to backup by default. This may take the hassle out of deciding what to backup. There is a plethora of backup tools, but I am going to focus on Window’s File History for now since it is a set it and forget it type deal.

Ensure that any files that you want backed up are in a folder that you are backing up.

### Where should you Backup

There are several factors to take into account when deciding where to backup your files:

- How quickly would you need to recover your files?

- Are you willing to pay a price for the retrieval/storage of your data?

- How likely is it that the location of your backup will be compromised?

- Does your backup contain any sensitive files that you don’t want prying eyes to see?

This write-up pertains to backups stored on your own separate storage device. I have my backups on a 12TB External HDD, which is partitioned to separate the backups of the several storage devices that I have in my PC. Unless some natural disaster occurs, which wipes out my PC and backup drive (they are in the same location), I can perform a rapid recovery in the event any of my PC’s storage devices fail. You could also backup your files to the cloud. If you are performing backups for yourself, that could be as simple as using Google Drive or OneDrive. If a more robust solution is desired, however, there are options like rclone, Backblaze, or Duplicacy.

### Performing the Backup using Window’s File History

Setting up File History is simple. There are several ways you can navigate to it, but we will use the search bar. Follow these steps:

1. Type “backup settings” in the search bar located on the left side of the taskbar.

1. Click on “Backup Settings”

1. Click on the “+” button to add a drive which is located under the “Back up using File History” section. This drive is where your backups will be stored.

1. The “Automatically back up my files” option should be toggled to “On” by default. If not, click it to switch it from “Off” to “On.”

1. Adjust the frequency, how long you want your backups stored, and what you want backed up by clicking “More Options.”

 At anytime you can manually start a backup by clicking “Back up now.” You can take a look at your backups by clicking “Restore files from current backup” at the bottom of the “Backup options” window. Note that clicking this will not start the restore. The File History window lists all of the files and folders that are in the backup. You can go into folders and choose to restore a specific file, or you can restore the entire backup if you wish by clicking the green button. This will restore the files and folders to their original locations. If you want to restore the backup to a different location, click the gear in the top left and select “Restore to.”

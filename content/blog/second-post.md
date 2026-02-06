---
author: Rickey Morris
title: First foray into the cloud 
date: 2023-10-04T11:51:58-04:00
# layout: 
description: Learning multiple technologies and tools using the cloud.
tags: ["blog"]
# icon: 
thumbnail: 
    url: images/linux_baby.png 
    author: Rickey Morris(Midjourney)
    # authorURL: 
    # origin: 
    # originURL: 
---

One of my objectives is to gain knowledge and experience with at least one cloud provider. Amazon Web Services that has the highest market share over Microsoft Azure and Google Cloud. So, I created this personal website to document my progress and get hands-on experience. However, I was initially unsure how to proceed with hosting my website on AWS. Searches about creating websites on AWS would return two methods: Amplify Hosting versus S3 and CloudFront. Initially I thought the two were distinct, but that is not the case. Amplify Hosting uses S3 and CloudFront, albeit AWS abstracts them from you. In other words, Amplify Hosting does not provide you with granular control over S3 and CloudFront. Amplify Hosting was a perfect fit since I am a newbie and wanted to get my website up and running with minimal configuration and low maintenance. Amplify Hosting also does not break the bank.

Amplify Hosting is free for 12 months for new AWS customers. You should note that you are allocated a certain amount of resources per month during those 12 months. If you exceed those thresholds, then you will incur a fee. It is Similar to capped data plans for your cell phone. I will also note that if you are following this tutorial that walks you through hosting a website via Amplify Hosting, note Amazon Route 53 is not a free service and has a minimum cost of $0.50 per hosted zone per month. I use a different provider for my domain, so I am not subject to that cost. Ensure you check which services are used for tutorials because not all the services are free. You do not want Amazon to hit you with a surprise bill. I expect the cost of my website to be insignificant after the 12 months. Even with that expectation, I will make it a habit to monitor metrics about my website, which Amazon CloudWatch provides. The more content and visitors to your website translates to a higher price.

This website of mine is part of a multi-faceted project. As mentioned in the introduction, I am using it to learn AWS. There are several other technologies and tools that I wish to study, however. Among them are Linux, Bash, Git and GitHub, static site generators (This site uses Hugo), and whatever else I stumble across.

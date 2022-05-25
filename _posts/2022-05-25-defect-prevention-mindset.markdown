---
title: QAs are now not asked to find defects
author: Brijendra Singh
category: Test Strategy
tags: [test pyramid, component test , microservices, API automation, contract test]
# img: ":post_pic_micro_test_strategy.jpg"
date: 2022-05-25 08:11:06 +0900
meta_description: "meta TBU"
published: false
---
> Prevention is better than cure! 
> lets find out how shifting a QA mindset from defect detection to defect Prevention can help YOUR team achieve goals without testing bottlenecks. 

## Why to avoid defect detection
Finding and fixing defects provides software team a boost to go ahead with production release. However, finding defects on lator stage of software development may cause possible changes in timelines and can also cause some compramises with quality.
Lets recall the SDLC flow.
- Requairement Gathering and Analysis
- Development
- Testing
- Deployment

If we go ahead with an attitude of finding defect post feature is built and deployd to dev/QA environment. Below things may happen
- RCA aroung defect is happen and concluded to be a requirement change
- Unit/Integration tests were missing or wrongly validated the module 
- e2e/Regression suites might be updated to accomodate possible fix in feature
- Retesting the feature and small regression around that featrure is required

Considering the above points
- Development team may have to rethink the feature and Rework on Analysis and Development
- It may be difficult to find the devs who might have developed the feature/story. They might have a new story to work upone.
- Context sharing will be required by the new developer

    
> Happy Testing :)

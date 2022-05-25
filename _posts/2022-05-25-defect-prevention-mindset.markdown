---
title: QAs are now not asked to find defects
author: Brijendra Singh
category: Test Strategy
tags: [test pyramid, component test , microservices, API automation, contract test]
# img: ":post_pic_micro_test_strategy.jpg"
date: 2022-05-25 08:11:06 +0900
meta_description: "meta TBU"
# published: true
---
> Prevention is better than cure! 
> lets find out how shifting a QA mindset from defect detection to defect Prevention can help YOUR team achieve goals without causing testing bottlenecks. 

## Why to avoid defect detection
Finding and fixing defects provides software team a boost to go ahead with production release. However, finding defects on lator stage of software development may cause possible changes in timelines and can also cause some compramises with quality.
Lets recall the SDLC flow.
- Requairement Gathering and Analysis
- Development
- Testing
- Deployment

If we go ahead with an attitude of finding defect post feature is built and deployd to dev/QA environment. Below things may happen
- RCA might be concluded as requirement change
- Unit/Integration tests were missing or wrongly validated for the module 
- e2e/Regression suites might needs to be updated to accomodate possible fix in feature
- Re-testing and small regression around that featrure is required

Considering the above points
- Development team may have to re-think the feature and rework on Analysis and Development
- It may be difficult to find the devs who might have developed the feature/story. They might have a new story to work upone.
- Context sharing will be required by the new developer.
- whole dev-test cycle will be triggered and tested once the fix is deployed to dev/qa env.

Look at the above points a bit more seriously. It may hint you below gaps
- QAs where not invloved in requirement/feature refinement and consultation: If done so posible requirement defects detected post development might have been solved earlier
- test pyamid is not effectively followed and edge cases and data criticle scenarios were mised while development. If tests were properly written/validated  on lower layers while developer were working on story. Defects would have prevented.
- overll development rework and testing rework would have been avoided.

## How to focus more on Defect Prevention 
YOU should perform Quality checks right from the begining of Requirement gathering and refinement. You (QAs) should wear a user hat and shoud consult on how they would imagine a feature to be. What might help them and what may cause a confusion or not enough informations.
Once feature is well groomed and ACs are finalized its becomes very rare to find any issue related to this on lator stages of development.

YOU along with BA and dev should clear out things and agree on the ACs and tech approach before devs pick up the story for development. YOU can call this check as STORY KICKOFF. 
Next stage for you to be contineously invlved with developers while they are working on the story to ensure they are following the
- good code quality: code should be clear enough for others so that future modifications can be made easily.
- code/framework should be capable enough to accomodate any future enhancements 
- unit/integration test coverage: YOU should not only focus on code coverage %. Sometimes data permutation and combination on same code can cause issues on feature. 
- Look for an opportunity where you can pick up the early validation for fast feedback.

Once dev work is done and ready to be deployed YOU all three (QAs, BAs and Devs) should come together. In this connect you all go through the ACs and validate the feature. Here it becomes very easy to accommodate any feedback and validate the outcome to finalise the decision and approach. You can call this connect as devbox. I have seen people using other names as well like deskcheck and volleyball for this kind of connect and precheck.

once all satisfied, dev changes are now ready to be deplyed on env and becomes ready for you (QAs) for the exploratory testing.
- filter out what really is needed to be part of Automated UI end to end test suites. YOU should not cover everything on this layer.
- Take laverage of API tests and validate various business use cases in this layer.
- 
Now you can try to emagine the confidence level over the feature. QAs effort will be reduced drastically and you will get ample amount of time to break the application on edge cases.

There is one more thing you can try out before regression testing. Before Regression bring up everyone from team and ask them to test application for any possible defects or break it all together. We call it Bug bash and trust me , it will work as wonder to find out issues that would not have been discovered by any other means.

These things have helped me and my peers to avoid testing bottlenecks and a lot of teams rework. It also helped us to stick on our timeline and deliver the release on scheduled time. 

What do you think about this? Did this writeup helped you to change your perspective on testing ? 
    
> Happy Testing :)

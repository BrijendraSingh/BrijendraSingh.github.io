---
title: QAs are not asked to find defects
author: Brijendra Singh
category: Test Strategy
tags: [test pyramid, component test, test strategy]
img: ":defects-prev.jpg"
date: 2022-05-25 08:11:06 +0900
meta_description: "meta TBU"
# published: true
---
> `Prevention is better than cure!` 
> 
> lets find out how shifting a QA mindset from defect detection to defect Prevention can help YOUR team achieve goals without causing testing bottlenecks. 

## Why to avoid defect detection
Finding and fixing defects provides software team a boost of confidence to go ahead with production release. However, finding defects on lator stages of software development may cause possible changes in timeline. This can also results into a compramise with quality.

Lets recall the SDLC flow.
> - Requairement Gathering and Analysis
> - Development
> - Testing
> - Deployment

We will figure out together what may go wrong, if we go ahead with a mindset of finding defects post feature deployment to dev/QA environment. 
- RCA concluded to be a requirement change
- Unit/Integration tests were missing or wrongly validated for that module 
- e2e/Regression suites needs to be updated to accomodate possible fix in feature
- Re-testing and small regression around that featrure is required

Considering the above points
- Development team may have to re-think the feature and rework on Analysis and Development
- It may be difficult to find the devs who might have developed the feature/story. They might have a new story to work upone. They may also take up some time to switch between the stories and tasks.
- If new dev signs up for it then context sharing will be required.
- The same Development-QA cycle will start. 

I am now looking at those above points a bit more seriously. Few gaps comes to my mind.
- QAs where not invloved in requirement/feature refinement and consultation: If done so posible requirement defects detected post development might have been solved earlier
- `Test pyamid` is not effectively followed. Edge cases and data criticle scenarios were mised. YOU (devs/QAs) should have written/validated tests on  Unit/Integration test layers. This would have reduce defects to be slipped on lator stages of SDLC.
- Overll development and testing `re-work` would have been avoided.

## How to focus more on Defect Prevention 
QAs should perform Quality checks right from the `begining` of Requirement gathering and refinement. QAs should wear an `end user` hat and shoud `consult` on how they would imagine a feature to be. What might help them and what may cause a confusion or might not work.
Once feature is well groomed and ACs are finalized its becomes very rare to find any issue related to this on lator stages of SDLC.

QAs along with BA and dev should clear out things and agree on the ACs and tech approach `before` devs pick up the story for development. YOU can call this check as `STORY KICKOFF`. 

Next stage for QAs to be `contineously` involved with developers while they are working on the story to ensure they are following the
- good code quality: code should be clear enough for others so that future modifications can be made easily.
- code/framework should be capable enough to accomodate any future enhancements 
- unit/integration test coverage: QAs should not only focus on code coverage overall %. Sometimes data permutation and combination on same code can cause issues on feature. 
- Look for an opportunity where you can pick up the `early validation` for fast feedback.

Once dev work is done and ready to be deployed YOU all three (QAs, BAs and Devs) should come together. In this connect you all go through the ACs and validate the feature. Here it becomes very easy to accommodate any feedback and validate the outcome to finalise the decision and approach. You can call this connect as devbox. I have seen people using other names as well like deskcheck and volleyball for this kind of connect and precheck.

once all satisfied, dev changes are now ready to be deplyed on env and becomes ready for you (QAs) for the exploratory testing.
- filter out what really is needed to be part of Automated UI end to end test suites. YOU should not cover everything on this layer.
- Take laverage of API tests and validate various business use cases in this layer.
- 
Now you can try to imagine the confidence level over the feature. QAs effort will be reduced drastically and you will get ample amount of time to break the application on edge cases.

There is one more thing you can try out before regression testing. Before Regression, bring up everyone from the team and ask them to test application for any possible defects or break it all together. We call it Bug bash and trust me , it will work as wonder to find out issues that would not have been discovered by any other means.

![defect-prevention](https://user-images.githubusercontent.com/19272137/170416790-9ca64642-d90f-4845-927d-0c2ccec23c68.jpg)


> Its not like Defect detection is all bad and you should stop doing it. I am saying you to focus more on Defect prevention rather than detection. I personally follow the 80-20 split. where 80% of my effort goes to defect preevntation and only 20% to defect detection (exploratory testing and bug bash).
> These things have helped me and my peers to avoid testing bottlenecks and a lot of teams rework. It also helped us to stick on our timeline and deliver the release on scheduled time. 


> What do you think about this? Did this writeup helped you to change your perspective on testing ? 
    
> Happy Testing :)

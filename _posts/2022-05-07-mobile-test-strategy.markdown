---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_Examples
title: Practicle Mobile Test Strategy

# post specific
# if not specified, .name will be used from _data/owner.yml
author: Mr. Brij
# multiple category is not supported
category: mobile test strategy
# multiple tag entries are possible
tags: [mobile test strategy, mobile testing, automation ]
# thumbnail image for post
img: ":post_pic1.jpg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-05-07 08:11:06 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-02-10 08:11:06 +0900
# check the meta_common_description in _data/lang/[language].yml
meta_description: "meta description"

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---

<!-- outline-start -->

This is an example page to display markdown related styles for Mr. Green Jekyll Theme.

<!-- outline-end -->

## Why Test Strategy is important ?
The purpose of a Test Strategy is to create an understanding of the overall targets, approach, tools and timing of test activities to be done. It should clarify the major challenges and tasks of the test project.


## How do you build mobile test strategy ?
we should avoid some anti patterns while building test strategy
* Look for template available in your organization
* Ask your colleagues 
* Look online


**Do you see a problem in this approach ?** 
Earlier stated approach may not be directly applicable to your project.
As your app may have specific need , function and target user
{: .notice}

## Your app may have unique requirements
understanding business behind the app, stakholders mindset and technical feasibilty is important.

## You should seek answer to these questions first
- Who are the various stakeholders on who quality would be dependent?
- Do you have a RACI* matrix for the most important processes? 
- Thought about Definition of Done ?
- Any CI/CD pipeline guideline that would ensure quality is shifted left ?
- What would be the release frequency ?
- Possible Testing bottleneck ? 
- What are the Legal requirements ?
- Failure points ?
- What would happen if quality is not maintained ?
- Architecture ? 

### RACI matrix
<img width="1081" alt="Screenshot 2022-05-06 at 2 35 28 PM" src="https://user-images.githubusercontent.com/19272137/167105977-6bb1ddcd-ba8a-4098-913d-abebe837dd5a.png">

tbu - RACI details

## Business priorities
* What is the client most worried about?
* Who are the implicit users?
* What is the risk appetite of the client in case of a calamity in production?

## Identify your app
<img width="1125" alt="Screenshot 2022-05-06 at 3 16 44 PM" src="https://user-images.githubusercontent.com/19272137/167109144-bbaf06a8-8224-420e-9ca4-2dd8b48660de.png">

* **Native mobile apps (i.e., downloadable apps)** are smartphone apps specifically designed for a particular operating system—iOS or Android. They are written in cross-platform frameworks like React Native or platform-specific languages such as Swift or Objective-C (for iOS) or Java or Kotlin (for Android). Native apps are installed on a device. They are built using an operating system’s SDKs and have access to different resources on a device: camera, GPS, phone, device storage, etc.
* **Web mobile apps** are websites optimized for mobile browsers. Their functionality resides entirely on a server. They are written in JavaScript and HTML5.
* **Hybrid mobile apps** combine features of native and web apps. They are written in HTML5 and JavaScript, like web apps. For the most part, they are web pages wrapped in a mobile app using WebView. However, they also have access to the built-in capabilities of a device. They are built using cross-platform frameworks like React, Ionic, Sencha and Xamarin.
* **Progressive web apps (PWAs)** are web applications designed to work on any standards-compliant web browser on both desktop and mobile devices. They are written in JavaScript, HTML, and CSS. They function like native mobile apps in that they use an app shell that allows for app-style gestures and navigations.

## Target Platform
<img width="930" alt="Screenshot 2022-05-06 at 12 08 13 PM" src="https://user-images.githubusercontent.com/19272137/167079894-b69e9e2c-b49c-4a1b-a24a-a4df4687f2a4.png">
- What analysis should help
- External factors to cover
- Apple guidelines
- brands/os guidelines or news
- How we did the research

## Device Selection for testing
<img width="997" alt="Screenshot 2022-05-06 at 3 00 38 PM" src="https://user-images.githubusercontent.com/19272137/167106080-7e5adae0-a918-4779-8a84-e25f384efdb5.png">

- What hardware/software combination to make
- virtual/real device or cloud?
- Fat finger issues

## Custom Settings
<img width="760" alt="Screenshot 2022-05-06 at 12 11 15 PM" src="https://user-images.githubusercontent.com/19272137/167080181-3a095a46-7301-45ac-853c-4a54eaed63b3.png">
- Why custom settings and what all are important
- Do you need it? based on user support you can define 
- examples


## Interruptions 
<img width="1094" alt="Screenshot 2022-05-06 at 12 12 52 PM" src="https://user-images.githubusercontent.com/19272137/167080432-3aa17414-60ae-4ea9-b13e-3b1f0329d820.png">

- Real time usage -> how can app get impacted
- 2G/3G financial transactions -> emergency app usage
- Educational backgrounds-> financial transactions

## Specific conditions
Device specific conditions
* Memory consumption
* Power utilization
* Network connectivity
* Operating in the background
* Switching between applications
* Memory leakage
* Storage
* Image capture/upload/scan
* File download
* Location


Application Specific Conditions
- Installation
- Uninstallation
- Update
- Backward compatibility
- App launch
- App data
{: .notice}

## Testing type
<img width="679" alt="Screenshot 2022-05-06 at 2 42 42 PM" src="https://user-images.githubusercontent.com/19272137/167106187-f84231b7-76f1-4d80-b750-a40ca0f33ba0.png">

- What all testing types can be applied to
- How it impacts can be explained with next slide

## Path to production
<img width="1318" alt="Screenshot 2022-05-06 at 3 39 16 PM" src="https://user-images.githubusercontent.com/19272137/167112101-1652dbaf-988e-4683-b76a-679c3d03958e.png">

dev-> qa-> uat-> pen testing-> DS approval-> prod sanity-> submission to store-> rollout to customer as in part/full


## Automation Testing
<img width="940" alt="Screenshot 2022-05-06 at 12 16 08 PM" src="https://user-images.githubusercontent.com/19272137/167080854-6d47b8c9-e058-462b-a563-bfc11c387ace.png">
take advantages of lower level automated tests


## Define test pyramid
<img width="635" alt="Screenshot 2022-05-06 at 12 17 33 PM" src="https://user-images.githubusercontent.com/19272137/167081022-04defe91-c701-4b28-8a8e-256eaa53f23b.png">

decide % distribution of each layer -> it will vary based of project stack characteristics

## Automation tool and framework selection
<img width="1282" alt="Screenshot 2022-05-06 at 12 18 22 PM" src="https://user-images.githubusercontent.com/19272137/167081138-60cd467a-5763-45d2-85d6-17813fb7601b.png">

### How ?
- List down different mobile test automation options
- Advantages and disadvantages of cross-platform v/s native frameworks
- How to choose the right mobile test automation framework for your testing needs
- How to leverage the unique benefits of a testing cloud
- Refer official documentation 
<img width="575" alt="Screenshot 2022-05-06 at 3 06 06 PM" src="https://user-images.githubusercontent.com/19272137/167106862-201d104e-8b54-4556-9640-a9426c6101f5.png">


## Try Pugh Matrix comparison
<img width="1267" alt="Screenshot 2022-05-06 at 12 20 17 PM" src="https://user-images.githubusercontent.com/19272137/167081349-17e2ea21-2fd9-4edb-8fcd-505895c7a090.png">

## Be aware of
Number of choices increases due to:
* Available list of tools/frameworks - Democratization of source code led to development of tools with similar features but subtle differences
* Team constraints/preferences
* Client requirements
<img width="957" alt="Screenshot 2022-05-06 at 1 41 54 PM" src="https://user-images.githubusercontent.com/19272137/167093649-dc48b735-3d8f-4a3f-9d6e-1cc56e67cdf1.png">


## Identify your risk
- What to test first and what to test last
- Risk based approach to determine testing automation priority
- You can determine risk/priority of each thing you want to test
- Consider making RAID matrix
<img width="1297" alt="Screenshot 2022-05-06 at 3 14 36 PM" src="https://user-images.githubusercontent.com/19272137/167108106-927de03d-096c-40f4-ab40-261200d913c2.png">

* A key part of any test automation strategy is knowing what to test first and what to test last. 
* You should use a risk-based approach to determine this testing automation priority. 
* You can determine the risk, or priority, of each thing you want to test by figuring out its business impact and adding that to the probability of it failing. 
* Obviously, the things with the highest business impact and highest probability of failure should be highest on your priority list, while the things with the lowest business impact and lowest probability of failure should be at the bottom. 
* This will also help quite a lot with the aforementioned testing squeeze and knowing what you want to cut first.
{: .notice}

## Importance of Manual Exploratory Testing
tbu 


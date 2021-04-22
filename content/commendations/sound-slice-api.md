+++
title = "Utilize Soundslice's JS API to make our Custom Player UI control Soundslice Iframe Embed"
score = "5.00"
description = "Igor is incredible. He is entirely reliable, highly skilled, easy to work with, and trustworthy. In short, a perfect contract partner."
date = 2018-04-21T00:00:00+01:00
author = "Darren Jahn"
company = "FiddleQuest LLC"
+++

https://app.fiddlequest.com - React. Typescript, business logic-rich, media rich, reactive/realtime, html5 game app, ios/android video shoot/upload app.

Infrastructure: AWS for synchronisation with the html game app and the teacher mobile app; maintenance tasks, emailing, video converting, file storage, backup storage. Stripe for non-trivial billing setup (coupons, discounts, subscription grades).
DigitalOcean for hosting the apps. Docker, Ansible for building it.

Backend: Meteor, Node.js with Typescript, custom Meteor protocol for data exchange with frontend.

Frontend: React and Typescript.

I’ve been improving this app from the start, where it started as a prototype html page with js integration with an external notation service iframe API.
I was improving it since; the client proposed to use MeteorJS hyped at that point of time, in hindsight it wasn’t the greatest decision technically but it was good enough to get the revenue flowing.

I’ve been improving it in accord with quickly growing and changing requirements, moving it to React at some point, with no development performance impact thanks to down-to-the-top approach.

There’s some parts still on older techs/libs but the trick I do is I load this code chunks only when these parts are used, therefore performance for most of users is better.

There’s from time to time were requirements for faster feature development and we employed additional workforce. I’ve been supervising them and reviewing their code, hence we have eslint rules for the codebase.

Features:

* four account types with unique business logic for each; i.e. teachers can assign/evaluate students or student groups, parents can pay and enroll/unsubscribe their children, independent students can do parts of what parents can do and what children can do.
* “Demo students” for teachers to check the app. At some point, “demo” account type for students/parents with special permissions (due to a business decision we removed it)
*  feature rich work with media - video sharing with special ‘static’ paths for facebook bot, video upload/encode/watermark/thumbnails from the React Native app, realtime integration with Badges (archievements) from the game app, using external notation service for playing music through our player interface
* admin interface and other rarely used parts of the app are loaded only when accessed
* user announcement/feedback system (first Intercom, then in-house), in-house TOS accepting modal
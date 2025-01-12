---
layout: page
title: Projects
permalink: /projects/
---

## [MPN Lookup](https://jonathan-gartland.github.io/mpn-lookup-nextjs) <span style="padding-left: 50px;"> ![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)</span>
[![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.
com/jonathan-gartland/mpn-lookup-nextjs)

[![Playwright Tests](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml/badge.svg?branch=development)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml)
[![Node.js CI](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml) [![Deploy](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml)  
 
  

This is a very simple app that looks like a wireframe for a phone app. The details are available in the README.md file in the project.  
  
I wrote this app to practice testing with React, so here I will simply discuss the testing.  
  
The component tests include a test for the Home view, validating that clicking the buttons brings the user to the correct screen. The LoginComponent test verifies the functionality of each screen with a few simple tests and actions. I added tests for the MPN object into this project as I am including it directly instead of using the library from the npm registry (where these tests would be part of the package, and not our concern here), so I added tests that validate the object for now, until I update the app to use the official library.  

---  
  
## [MPN Lookup Native App](https://github.com/jonathan-gartland/MpnLookupRN) <span style="padding-left: 50px;"> ![React Native](https://img.shields.io/badge/react_native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)</span>  
[![Tests (jest)](https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml/badge.svg?
branch=development)](https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml)  
  
The app above refactored into a native app project. I am implementing tests using tools like Maestro and Appium 
using this practice project.  
  
---  

## [MPN Lookup Flutter](https://github.com/jonathan-gartland/mpn_lookup_flutter) <span style="padding-left: 50px;"> ![Flutter](https://img.shields.io/badge/flutter-%2320232a.svg?style=for-the-badge&logo=flutter&logoColor=%2361DAFB)</span>
[![Flutter](https://github.com/jonathan-gartland/mpn_lookup_flutter/actions/workflows/setup-flutter.yml/badge.svg)](https://github.com/jonathan-gartland/mpn_lookup_flutter/actions/workflows/setup-flutter.yml)   
  
The app above refactored into a native app project. I am implementing tests using tools like Maestro and Appium
using this practice project.
  
---
  
# [Jonny's Bikes](https://jonathan-gartland.github.io/jonnys-bikes) <span style="padding-left: 50px;"> ![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)</span> ![Apache ECharts Badge](https://img.shields.io/badge/Apache%20ECharts-AA344D?logo=apacheecharts&logoColor=fff&style=for-the-badge)
[![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.com/jonathan-gartland/jonnys-bikes)  
[![Playwright Tests](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/playwright.yml) [![Deploy](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/deploy.yml)  


A very simple SPA that started out as a NextJS app using Django as the middleware, and Postgres as the backend datasource. The data set is a list of bikes and a few frames that I have collected over the years. Once I got the initial draft of the app written, I refactored it to be a SPA using a json file in place of PostgreSQL & Django, so I could more easily host it on GitHub Pages and implement some e2e tests for practice.  
  
The interesting tests in this project from my perspective are the tests for the echarts, which were a little tricky to validate, but I found a working pattern to follow and was able to add component tests for the PieCharts. The other testing, relating to Django and PostgreSQL, aren't relevant to this project so not included.  

---
  
## [ApiTestFrameworkMocha](https://github.com/jonathan-gartland/ApiTestFrameworkMocha) <span style="padding-left:50px;">![Mocha](https://img.shields.io/badge/-Mocha-%238D6748?&style=for-the-badge&logo=Mocha&logoColor=white)</span> ![Chai](https://img.shields.io/badge/chai.js-323330?style=for-the-badge&logo=chai&logoColor=red)
[![API tests demo](https://github.com/jonathan-gartland/ApiTestFrameworkMocha/actions/workflows/main.yml/badge.svg)](https://github.com/jonathan-gartland/ApiTestFrameworkMocha/actions/workflows/main.yml)
  
Demonstration of API testing using Mocha, Chai, and TypeScript. The tests are simple, but the framework is set up to 
be easily expanded upon.  
  
## Errata  
Random 'Take Home' projects from sketchy 'QA as a service' companies that are cheapening the value of QA work.

[LoopQA Assessment - Data Driven Testing](https://github.com/jonathan-gartland/playwright-demo-jg) <span
style="padding-left: 50px;">![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=fff&style=for-the-badge)</span>  

This was a technical assessment assignment for an interview. Given a set of detail to validate against a trello like app - which lacked any useful identifiers or test id's fwiw. Tradeoffs were made in implementing as I time boxed it to 4 hours total so it could be easily optimized with some thoughtful refactoring. 

[Playwright example: QA Wolf Take Home](https://github.com/jonathan-gartland/qa_wolf_take_home) <span
style="padding-left: 50px;">![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=fff&style=for-the-badge)</span>  
[![Playwright Tests](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml)

Simple solution to a simple task. I did add some linting and CI/CD so I guess I did do extra, but its 'project value add extra' not 'over-engineered solution extra' so take it for what it is.  
  



---
layout: page
title: Projects
permalink: /projects/
---

## [MPN Lookup](https://jonathan-gartland.github.io/mpn-lookup-nextjs) <span style="padding-left: 50px;"> ![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  
[![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.com/jonathan-gartland/mpn-lookup-nextjs)

[![Playwright Tests](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml/badge.svg?branch=development)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml) 
[![Deploy](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml) 
[![Node.js CI](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml) [![Deploy](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml)  
 
  

This is a very simple app that looks like a wireframe for a phone app. The details are available in the README.md file in the project.  
  
I wrote this app to practice testing with React, so here I will simply discuss the testing.  
  
The component tests include a test for the Home view, validating that clicking the buttons brings the user to the correct screen. The LoginComponent test verifies the functionality of each screen with a few simple tests and actions. I added tests for the MPN object into this project as I am including it directly instead of using the library from the npm registry (where these tests would be part of the package, and not our concern here), so I added tests that validate the object for now, until I update the app to use the official library.  

---  
  
## [MPN Lookup Native App](https://github.com/jonathan-gartland/MpnLookupRN) <span style="padding-left: 50px;"> ![React Native](https://img.shields.io/badge/react_native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  

[//]: # ([![Tests &#40;jest&#41;]&#40;https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml/badge.svg?branch=development&#41;]&#40;https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml&#41;  )

  
The app above refactored into a native app project. I am implementing tests using tools like Maestro and Appium using this practice project.  

  
---  

## [MPN Lookup Flutter](https://github.com/jonathan-gartland/mpn_lookup_flutter) <span style="padding-left: 50px;"> ![Flutter](https://img.shields.io/badge/flutter-%2320232a.svg?style=for-the-badge&logo=flutter&logoColor=%2361DAFB)</span>
[![Flutter CI](https://github.com/jonathan-gartland/mpn_lookup_flutter/actions/workflows/main.yml/badge.svg)](https://github.com/jonathan-gartland/mpn_lookup_flutter/actions/workflows/main.yml)     

  
The app above refactored into a flutter app. Used to get some practice testing Flutter apps. Additional UI tests 
using Appium are in the works.  
  
---
  
# [Jonny's Bikes](https://jonathan-gartland.github.io/jonnys-bikes) <span style="padding-left: 50px;"> ![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)</span> ![Apache ECharts Badge](https://img.shields.io/badge/Apache%20ECharts-AA344D?logo=apacheecharts&logoColor=fff&style=for-the-badge) ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  
[![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.com/jonathan-gartland/jonnys-bikes)  
[![Playwright Tests](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/playwright.yml) [![Deploy](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/jonnys-bikes/actions/workflows/deploy.yml)  


A very simple SPA that started out as a NextJS app using Django as the middleware, and Postgres as the backend datasource. The data set is a list of bikes and a few frames that I have collected over the years. Once I got the initial draft of the app written, I refactored it to be a SPA using a json file in place of PostgreSQL & Django, so I could more easily host it on GitHub Pages and implement some e2e tests for practice.  
  
The interesting tests in this project from my perspective are the tests for the echarts, which were a little tricky to validate, but I found a working pattern to follow and was able to add component tests for the PieCharts. The other testing, relating to Django and PostgreSQL, aren't relevant to this project so not included.  

---
  
## [ApiTestFrameworkMocha](https://github.com/jonathan-gartland/ApiTestFrameworkMocha) <span style="padding-left:50px;">![Mocha](https://img.shields.io/badge/-Mocha-%238D6748?&style=for-the-badge&logo=Mocha&logoColor=white)</span> ![Chai](https://img.shields.io/badge/chai.js-323330?style=for-the-badge&logo=chai&logoColor=red) ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)
  
[![API tests demo](https://github.com/jonathan-gartland/ApiTestFrameworkMocha/actions/workflows/main.yml/badge.svg)](https://github.com/jonathan-gartland/ApiTestFrameworkMocha/actions/workflows/main.yml)  

Demonstration of API testing using Mocha, Chai, and TypeScript. The tests are simple, but the framework is set up to 
be easily expanded upon.  
  
---  

## [Pytest validation of Snowflake database loading](https://github.com/jonathan-gartland/data_validation_test) ![Snowflake](https://img.shields.io/badge/-Snowflake-29B5E8?&style=for-the-badge&logo=snowflake&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest)
I've been doing data validation work for a long time and I wanted to try some of the newer tools on the market.  
This simple example copies the tables from the PostgreSQL sample database dvdrental to a Snowflake instance, hosted on AWS in my case. These tests are just some simple validation used to check that the data was copied correctly.  
  
---  


## Errata & miscellaneous 'take home' projects  

Random 'Take Home' projects from sketchy 'QA as a service' companies that are cheapening the value of QA work and 
other examples I've stubbed out for practice.

[LoopQA Assessment - Data Driven Testing](https://github.com/jonathan-gartland/playwright-demo-jg) <span
style="padding-left: 50px;">![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=fff&style=for-the-badge)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  
[![Playwright Tests](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml)  

This was a technical assessment assignment for an interview. Given a set of detail to validate against a trello like app - which lacked any useful identifiers or test id's fwiw. Tradeoffs were made in implementing as I time boxed it to 4 hours total so it could be easily optimized with some thoughtful refactoring. 

[Playwright example: QA Wolf Take Home](https://github.com/jonathan-gartland/qa_wolf_take_home) <span
style="padding-left: 50px;">![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=fff&style=for-the-badge)</span>  ![JavaScript](https://img.shields.io/badge/-JavaScript-f0db4f?&style=for-the-badge&logo=JavaScript&logoColor=black)
[![Playwright Tests](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/playwright-demo-jg/actions/workflows/playwright.yml)

Simple solution to a simple task. I did add some linting and CI/CD so I guess I did do extra, but its 'project value add extra' not 'over-engineered solution extra' so take it for what it is.  
  



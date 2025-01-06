---
layout: page
title: Projects
permalink: /projects/
---

# Practice with React, NextJS, React Native and associated testing tools.  




### :rocket: [MPN Lookup using NextJS](https://jonathan-gartland.github.io/mpn-lookup-nextjs) - [Project Code](https://github.com/jonathan-gartland/mpn-lookup-nextjs)  

[//]: # (commment example for md so i dont forget) 
  


This is a very simple app that looks like a wireframe for a phone app. The details about the project are available in the README.md file in the project.  
  
I wrote the app to practice testing with React, so here I will simply discuss the testing.  
  
The component tests include a test for the Home view, validating that clicking the buttons brings the user to the correct screen. The LoginComponent test verifies the functionality of each screen with a few simple tests and actions. I added tests for the MPN object which is included directly instead of using the npm library from the npm registry (where tests usually happen), so I added tests that validate the object for now, until I update the app to use the official library.  
  
Bonus ~ React Native version of the app here: [MPN Lookup using React Native](https://github.com/jonathan-gartland/MpnLookupRN)  


### :rocket: [Jonny's Bikes](https://jonathan-gartland.github.io/jonnys-bikes) - [Project Code](https://github.com/jonathan-gartland/jonnys-bikes)

A very simple SPA that started out as a NextJS app using Django as the middleware, and Postgres as the backend datasource. The data set is a list of bikes and a few frames that I gave amassed. Once I got the initial draft of the app written, I refactored it to be a SPA, so I could more easily host it on GitHub Pages and implement some e2e tests.  
  
The interesting tests in this project from my perspective are the tests for the echarts, which were a little tricky to validate, but I found a working pattern to follow and was able to add component tests for the PieCharts. The other testing, relating to Django and PostgreSQL, aren't relevant to this project so not included.

---
&nbsp;
### Some other testing related projects, continuing the tradition of keeping things simple.



### :rocket: [Playwright example: LoopQA Assessment - Data Driven Testing](https://github.com/jonathan-gartland/playwright-demo-jg)

This was a technical assessment assignment for an interview. Given a set of detail to validate against a trello like app - which lacked any useful identifiers or test id's fwiw. Tradeoffs were made in implementing as I time boxed it to 4 hours total so it could be easily optimized with some thoughtful refactoring. 

### :rocket: [Playwright example: QA Wolf Take Home](https://github.com/jonathan-gartland/qa_wolf_take_home)  
Simple solution to a simple task. I did add some linting and CI/CD so I guess I did do extra, but its 'project value add extra' not 'over-engineered solution extra' so take it for what it is.  
  

API Testing

#### :rocket: [Supertest, Mocha, Chai](https://github.com/jonathan-gartland/ApiTestFrameworkMocha)

Simple example demonstrating how to implement API testing with Supertest, Mocha, and Chai. 


---
layout: page
title: Projects
permalink: /projects/
---

## [mpn-lookup (npm library)](https://www.npmjs.com/package/mpn-lookup) <span style="padding-left: 50px;"> ![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  
[![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.com/jonathan-gartland/mpn-lookup)

[![npm version](https://img.shields.io/npm/v/mpn-lookup.svg)](https://www.npmjs.com/package/mpn-lookup)
[![CI](https://github.com/jonathan-gartland/mpn-lookup/actions/workflows/ci.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup/actions/workflows/ci.yml)
[![npm downloads](https://img.shields.io/npm/dm/mpn-lookup.svg)](https://www.npmjs.com/package/mpn-lookup)

A small, typed TypeScript library for Most Probable Number (MPN) lookups on IDEXX Quanti-Tray, Quanti-Tray/2000 and Legiolert water tests. You pass in positive well counts and get back the MPN and its 95% confidence interval, so you don't need the printed reference tables. It's the core of the MPN Lookup apps below.

The tables are the critical part, so the project guards them:

- A checksum test hashes every lookup result and fails the build if any value changes. A separate CI job rejects any PR that touches the table data or that test.
- Inputs are validated: an out-of-range or non-integer count returns `undefined` and never an unrelated table entry. The tables are frozen at runtime so callers can't corrupt them.
- Releases build CJS and ESM bundles with type declarations. They're published from GitHub releases through npm trusted publishing (OIDC, no stored tokens) with provenance, and each version waits for 2FA approval before it goes live.
- Dependabot keeps dependencies current, and a Claude Code agent in GitHub Actions fixes Dependabot PRs whose CI fails, under the same rules: it can't touch the table data, the checksum test or the workflows.

---

## [MPN Lookup](https://jonathan-gartland.github.io/mpn-lookup-nextjs/) <span style="padding-left: 50px;"> ![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  
[![Live Demo](https://img.shields.io/badge/Live%20Demo-0E5A78?style=for-the-badge)](https://jonathan-gartland.github.io/mpn-lookup-nextjs/) [![Project Code](https://img.shields.io/badge/Project%20Code-20B2AA?style=for-the-badge)](https://github.com/jonathan-gartland/mpn-lookup-nextjs)

[![Playwright Tests](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/playwright.yml)
[![Node.js CI](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/test.yml)
[![Deploy](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml/badge.svg)](https://github.com/jonathan-gartland/mpn-lookup-nextjs/actions/workflows/deploy.yml)

A mobile-sized web app built on the `mpn-lookup` library. Choose a test type, enter the positive well counts, and it shows the MPN with its 95% confidence interval. It's a static Next.js export deployed to GitHub Pages, and I built it to practice testing a React app at every layer:

- **Component tests (Jest + React Testing Library):** the Home view's navigation, and the LookupComponent's input handling and results for each test type
- **End-to-end tests (Playwright):** run in Chromium, Firefox and WebKit, covering the menu flows, each calculator screen, and page metadata such as the favicon and link preview tags
- **Data integrity:** a checksum test hashes every lookup the app displays, so a dependency update that changes a published MPN value fails CI

---  
  
## [MPN Lookup Native App](https://github.com/jonathan-gartland/MpnLookupRN) <span style="padding-left: 50px;"> ![React Native](https://img.shields.io/badge/react_native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)</span> ![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?&style=for-the-badge&logo=Typescript&logoColor=black)  

[![Tests (jest)](https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml/badge.svg?branch=development)](https://github.com/jonathan-gartland/MpnLookupRN/actions/workflows/test.yml)
  
The MPN Lookup app refactored into a React Native project, used as the target application for a mobile test automation suite. The project includes a migration from Detox (the original E2E framework) to Appium, implemented in both Python (pytest + Appium Python Client) and TypeScript (WebdriverIO).

The Python suite uses a page object model built on pytest fixtures, covering all three calculator screens (QuantiTray, QuantiTray2000, Legiolert) with data-driven assertions derived from the original Detox test cases. The TypeScript suite implements the same coverage using WebdriverIO with typed page objects. Both suites support Android and iOS via configurable Appium capabilities and are structured for CI integration.

  
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

## [Consumer Driven Contract Testing with Pact](https://github.com/jonathan-gartland/example-consumer) <span style="padding-left: 50px;">![Pact](https://img.shields.io/badge/Pact-E4393C?style=for-the-badge)</span> ![JavaScript](https://img.shields.io/badge/-JavaScript-f0db4f?&style=for-the-badge&logo=JavaScript&logoColor=black)

[![Build](https://github.com/jonathan-gartland/example-consumer/actions/workflows/build.yml/badge.svg)](https://github.com/jonathan-gartland/example-consumer/actions/workflows/build.yml)

Consumer and provider implementations of contract testing using PactV3 and PactFlow. The [consumer](https://github.com/jonathan-gartland/example-consumer) defines interaction contracts — expected requests and responses — which are verified independently against the [provider](https://github.com/jonathan-gartland/example-provider) without requiring both services to be running simultaneously.

This pattern is particularly valuable in microservices and API-driven architectures where provider changes can silently break consumers. The suite uses `given()` state setup, matcher-based response validation, and PactFlow for contract publication and verification in CI.

---

## [Pytest validation of Snowflake database loading](https://github.com/jonathan-gartland/data_validation_test) ![Snowflake](https://img.shields.io/badge/-Snowflake-29B5E8?&style=for-the-badge&logo=snowflake&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest)
I've been doing data validation work for a long time and I wanted to try some of the newer tools on the market.  
This simple example copies the tables from the PostgreSQL sample database dvdrental to a Snowflake instance, hosted on AWS in my case. These tests are just some simple validation used to check that the data was copied correctly.

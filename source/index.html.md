---
title: API Reference

language_tabs:
  - shell
  - ruby

includes:
  - accounts
  - taxonomies
  - errors

search: true
---

# Introduction

Welcome to the Hollar API! This is the official API used by the web interface as well as an iOS application and an Android application.

You will use one of the following API endpoints

* **Prod: [hollar.com/api](http://hollar.com/api)**
* **Staging: TBD**
* **QA: [qa2-web.hollar.com/api](http://qa2-web.hollar.com/api)**
* **Dev: [dev2-web.hollar.com/api](http://dev2-web.hollar.com/api)**

# Making a request

Although the endpoints will probably return `json` responses without setting any headers it is preferable to do so.

* Set the **Content-Type** header to `application/json`.
* Set the **Accept** header to `application/json`.
* Set the **X-Spree-Token** header whenever we need to be authenticated.

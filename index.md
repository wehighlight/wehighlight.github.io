---
title: WeHighlight.com
layout: default
permalink: /
---



# WeHighlight.com

## Project description


(_WeHighlight.com_) is an open source project, with the following goals:

  * demonstrate big data to analyze patterns and relevance in latest news
  * Easy way to summarize and share summaries of articles.

How?

  * as readers find interesting lines in articles, they select/highlight those lines.
  * when other readers open those articles, they will have the option to see the lines other readers find interesting highlighted.
  * as more readers highlight lines, hilits overlap, an aggregation/consessus can be generated of the most important lines.

## Components:

WeHighlight.com consists of the following components:

  * [Chrome Extension](google_chrome_extension)
  * [Rails Backend](ruby_on_rails_backend)
  * [Spark Big data engine](big_data_engine)
  * [Jekyll project description site](jekyll_site)

## Privacy

In order to protect users from accidentaly highlighting sensitive data

 * only HTTP sites are hilitable, HTTPS sites are not hilitable.
 * a list of un hilitable sites will be set, sites like gmail.com,
 * pages are by default un hilitable, until one first user explicitly enables wehighlight.com for this page

## Project RoadMap

### Browser, Chrome Extension

#### Development
 * [x] Chrome options login
   * [x] Chrome options login, link to register
   * [x] Chrome options save login credentials
   * [x] Chrome reload save credentials on load
   * [x] message to indicate login failure
 * [x] Activate wehighlight.com for a page first time.
   * [x] message that no previous hilits
   * [x] logged in user, will have the option to highlight
   * [x] guest given login link
 * [x] hilit text and feed server, second time and later
   * [x] hilit text and 
   * [x] post to server
 * [x] load hilits from server
   * [x] for logged in users
   * [x] for guests
 * [x] highlight text in pages
   * [x] logged in users, show popup with button to highlight
   * [x] guests, can't highlight text
 * [x] mark Chrome page_action icon (blue) to indicate no available hilits, but allowed
 * [x] black out Chrome page_action icon (red) and (stop sign on it) to indicate site non hilitable
   * [x] click on page_actions icon gives message that web-page is non hilightable
 * [x] flash Chrome page_action icon (green) to indicate available hilits
 * [ ] aggreate overlapping hilits to generate consessus hilits

### Hosting
 * [x] Create Google Chrome webstore account (for user: wehighlightapp@gmail.com)
 * [x] Upload first build 0.0.1
 * [ ] write descriction
 * [ ] record video
 * [ ] promotional tile images(440 * 280)
 * [ ] Screenshots

---

## Server, Ruby On Rails 

### Development
 * [x] User management (devise)
   * [x] Login
     * [x] API
     * [x] Web
   * [x] register
     * [x] Web
 * [x] Hilits models
   * [ ] aggregate overlapping hilits 
 * [x] Hilits API 
   * [x] create
   * [x] index/list 
   * [x] show 
 * [x] Deployment
   * [x] Domain name
   * [x] create a RDS db
   * [x] AWS Account, Free Tier
   * [x] AWS code Deployment
  
## Web Interface, stanard HTML
 * [x] setup bootstrap

## Web client, AngularJS
 * [ ] set up Angular2 with Rails

## Mobile client, iOS





---
title: "Creating, Breaking and Fixing a Drupal Module"
author: "Allie Jones"
date: "2016-04-15"
categories: ["Drupal", "Public Speaking"]
featured_image: "/images/insights/creating-breaking-fixing-drupal.png"
youtube_video: "1LlZd-0noiI"
excerpt: "Debugging is more than fixing broken code. Learn how to logically think through steps and use the right tools to solve problems in Drupal 8's object-oriented architecture."
featured_on_homepage: false
priority: 4
draft: false
featured_link: "https://events.drupal.org/neworleans2016/sessions/debugging-during-development-creating-breaking-and-fixing-module"
profile_contributors: []
---

# Creating, Breaking and Fixing a Drupal Module

*April 2016 - DrupalCon New Orleans*

Debugging is more than fixing broken code. It's about logically thinking through steps and using the appropriate tools to solve problems. With Drupal 8's adoption of Symfony and object-oriented architecture, we need to adjust how we debug our code.


## Beyond dpm: New Debugging Approaches

Many of us have relied on the convenient `dpm()` function for debugging. However, `dpm()` can't print protected properties or provide information about methods of an object, making it difficult to debug objects and classes in Drupal 8.

## Modern Debugging Tools

**Xdebug with PHPStorm Configuration**
- Advanced debugging capabilities for object-oriented code
- Step-through debugging and breakpoints

**Devel and WebProfiler Module**
- Enhanced debugging tools for Drupal 8+
- Better object introspection capabilities

**Probo CI Integration**
- Continuous integration for faster testing
- Streamlined approval processes

## Hands-On Learning

In this session, we create a module, intentionally break it, and use modern debugging tools to identify, test, and fix the issues. Whether you're new to object-oriented PHP or an advanced developer, these techniques will help you debug code more efficiently.

The shift to Drupal 8's architecture requires evolving our debugging practices—this session shows you how.

---

*Originally presented at DrupalCon New Orleans 2016. [View session details →](https://events.drupal.org/neworleans2016/sessions/debugging-during-development-creating-breaking-and-fixing-module)*ca
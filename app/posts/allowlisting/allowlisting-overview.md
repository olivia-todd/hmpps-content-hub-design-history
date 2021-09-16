---
tags: false
layout: collection
title: Allowlisting
description: How we created prototypes to test our prioritised hypotheses.
pagination:
  data: collections.allowlisting
  reverse: true
  size: 50
permalink: "allowlisting/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
---

## Overview

### The problem

The Prisoner Content Hub, or “the Hub”, is a website available on in-cell laptops in some UK prisons and Youth Offender Institutions (YOIs). It is accessed via a closed secure network. All other external websites are blocked.

The Hub hosts a variety of educational and distraction content, prison or YOI-specific content such as Governor updates, and personal information.

The Hub hosts a variety of educational and rehabilitative content, local prison or YOI-specific content, and personal information. Our small team work alongside local content managers in each prison. Currently, a significant amount of time is spent searching for and downloading content from the internet to upload into the Hub's CMS. This is manual and time-consuming. It also results in needless duplication of content and creates a maintenance overhead.

As we’re now rolling out into new prisons at scale, we need a smarter way of giving people in prison access to new content. 
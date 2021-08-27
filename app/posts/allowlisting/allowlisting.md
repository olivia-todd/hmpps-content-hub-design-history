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

The Prisoner Content Hub, or “the Hub”, is a website available on in-cell laptops.

It is currently available in HMP Wayland, HMP Berwyn, HMYOI Cookham Wood and HMP Lindholme, with a planned rollout to more establishments. The Hub is accessed via a closed, secure network. Access to other external websites is blocked.

The Hub hosts a variety of educational and distraction content, prison or YOI-specific content such as Governor updates, and personal information.

The Hub has a small team of specialist content authors, working alongside local content authors in each prison. A significant amount of time is spent downloading content from the internet to upload into the Hub's CMS. This is a manual, time-consuming task.
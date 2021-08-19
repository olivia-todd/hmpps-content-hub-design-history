---
tags: false
layout: collection
title: Design principles
description: The values that guide the design of our service.
pagination:
  data: collections.design-principles
  reverse: true
  size: 50
permalink: "design-principles/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
---
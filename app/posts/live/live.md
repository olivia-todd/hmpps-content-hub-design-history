---
tags: false
layout: collection
title: Live
description: How we created prototypes to test our prioritised hypotheses.
pagination:
  data: collections.live
  reverse: true
  size: 50
permalink: "live/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
---
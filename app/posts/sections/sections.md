---
tags: false
layout: collection
title: Public beta
description: How we created prototypes to test our prioritised hypotheses.
pagination:
  data: collections.sections
  reverse: true
  size: 50
permalink: "sections/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
---
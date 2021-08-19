---
tags: false
layout: collection
title: Glossary of terms
description: A glossary of the most common terms used in the Content Hub service.
pagination:
  data: collections.glossary-of-terms
  reverse: true
  size: 50
permalink: "glossary-of-terms/{% if pagination.pageNumber > 0 %}page/{{ pagination.pageNumber + 1 }}{% endif %}/"
eleventyComputed:
  eleventyNavigation:
    key: "{{ title }}"
    excerpt: "{{ description }}"
    parent: home
---
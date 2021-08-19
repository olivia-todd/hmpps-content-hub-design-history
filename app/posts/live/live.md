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

<h2 id="live-overview"><a class="header-anchor" href="#live-overview">#</a> Live overview</h2>

<p>In alpha, we tested different tools and processes that staff can use to prepare and receive a person arriving at prison to:</p>

<ul>
	<li>ensure correct identification</li>
	<li>increase awareness of signs of risk</li>
	<li>create a better arrival experience</li>
</ul>

<p>We created prototypes to test each prioritised hypothesis, not proposed solutions.</p>
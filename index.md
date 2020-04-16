---
layout: home
title: Welcome 
---

Welcome
============

Causal Beast is a primer on causal inference. You can learn more about the course on the [about](about/) page and download the lecture slides and notes in <a href="{{ site.baseurl }}/public/causal-beast.pdf" target="_blank">PDF </a>or<a href="{{ site.baseurl }}/public/causal-beast.pptx" target="_blank"> PPT</a>.

Below is the outline which is subject to weekly updates including but not limited to new lessons, videos, notes and other renovations to improve your learning experience. If there is a particular topic you'd like to visit, please refer to the [search](search/) page.   
<br/>

{% for lesson in site.data.outline %}
{% capture lessonnumber %}{{ forloop.index }}{% endcapture %}
* [Lesson {{ lessonnumber }}: {{ lesson.title }}](lessons/lesson{{ lessonnumber}})
{% for segment in lesson.segments %}
{% capture segmentnumber %}{{ forloop.index }}{% endcapture %}
	 * [{{ lessonnumber }}.{{ segmentnumber }} {{ segment.title }}](lessons/lesson{{ lessonnumber}}/segment{{ segmentnumber }})
{% endfor %}
{% endfor %}
<br/>

Want to learn how to actually do your own causal inference research using statistical software or code? I am very pleased to announce that it's almost done and coming very soon!  :pray::pray:
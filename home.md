---
layout: page
title: Home
nav_order: 1
last_modified_date: "now"
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign overview = site.slides | where: "title", "Overview" | first %}
{{ overview.content }}

This course aims to xxx.

<small>[Read more...]({{ site.baseurl }}{% link syllabus.md %})</small>

[Find Zoom Links, Slides, and Recordings on LumiNUS](https://luminus.nus.edu.sg){: .btn .btn-blue }

{% for module in site.modules %}
{{ module }}
{% endfor %}

![Image of NUS Campus](./assets/images/NUS-campus.svg)

**This website is in progress and all content is subject to change.**{: .text-grey-dk-000 }

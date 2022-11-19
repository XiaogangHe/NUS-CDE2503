---
layout: home
title: CDE2503
nav_exclude: true
last_modified_date: "now" 
seo:
  type: Course
  name: Cities in Nature
---

![Image of Cities-In-Nature](./assets/images/palm-tree.png)

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

**This website is in progress and all content is subject to change.**{: .text-grey-dk-000 }

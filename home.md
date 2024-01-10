---
layout: page
title: Home
nav_order: 1
last_modified_date: "now"
---

![Image of Cities-In-Nature](./assets/images/palm-tree-river.png)

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

This course will provide students with an understanding of the “Sustainable Environment” outcome of the Singapore Liveability Framework (LF) that was developed by the Centre for Liveable Cities (CLC). It will address what sustainability is, and how it affects liveability. Most importantly, students will understand how cities address complex issues.

This course will cover the themes of Climate Resilience and Use of Limited Resources, covering topics such as water, green, waste, food, climate mitigation, climate adaptation, and energy resilience. Using case studies, students will glean insights on how to balance different stakeholders while solving complex urban issues.

<small>[Read more...]({{ site.baseurl }}{% link syllabus.md %})</small>

[Find Zoom Links, Slides, and Recordings on Canvas](https://canvas.nus.edu.sg/courses/52842){: .btn .btn-blue }

{% for module in site.modules %}
{{ module }}
{% endfor %}


{: .note }
This website is a work in progress and all contents are subjected to changes.

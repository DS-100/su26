---
layout: page
title: Schedule
nav_order: 1
permalink: /
seo:
  type: Course
  name: Data 100
---

# Data 100: Principles and Techniques of Data Science
## UC Berkeley, Summer 2026 
{: .mb-2 .fs-6 .text-grey-dk-000 style="margin-top: 0;"  }

[DataHub](https://data100.datahub.berkeley.edu/){:target="_blank" .btn .btn-datahub .mr-1}
[Gradescope](https://www.gradescope.com/courses/1329641){:target="_blank" .btn .btn-pensive .mr-1}
[PrairieLearn](https://us.prairielearn.com/){:target="_blank" .btn .btn-sections .mr-1}
[PrairieTest](https://us.prairietest.com/){:target="_blank" .btn .btn-sections .mr-1}
[EdStem](https://edstem.org/us/courses/99874){:target="_blank" .btn .btn-ed .mr-1}
[Office Hours](https://oh.ds100.org/){:target="_blank" .btn .btn-officehours .mr-1}
<!-- [Discussions & Tutoring](https://sections.ds100.org/){:target="_blank" .btn .btn-sections .mr-1} -->

<!-- [Askademia Livestream](https://www.askademia.org/ds100/sp26/livestream){:target="_blank" .btn .btn-lectures .mr-1}
[Zoom Livestream](https://berkeley.zoom.us/j/91466186973){:target="_blank" .btn .btn-traditional .mr-1}
[Askademia Lecture Recordings](https://www.askademia.org/ds100/sp26){:target="_blank" .btn .btn-lectures .mr-1}
[YouTube Lecture Recordings](https://www.youtube.com/playlist?list=PLQCcNQgUcDfopoa1txbWmAOIrZyx0XoZ7){:target="_blank" .btn .btn-traditional .mr-1} -->


<div>
  {% assign instructors = site.staffers | where: 'role', 'Instructor' | sort: 'order' %}
  <div class="role instructor-grid">
    {% for staffer in instructors %}
      <div class="staffer-container">
        {{ staffer }}
      </div>
    {% endfor %}
  </div>
</div>

<!-- {% assign announcement = site.announcements | where: 'week', site.current_week | first %}
{{ announcement }} -->

<!-- COMMENT THE FOLLOWING OUT WHEN WEBSITE IS READY TO GO!!! -->
<div class="alert" style="background-color: #ffffff; border: 1px solid #fd0000; padding: 12px 16px; border-radius: 4px; margin-bottom: 20px;">
  <strong>⚠️ This website is still under construction!</strong> Content is subject to change and some features of this page may not function properly.
</div>

<h2 class="d-flex align-items-center" id="schedule">
  Schedule
  <a href="#week-{{ site.current_week }}" class="btn btn-currentweek">
    Jump to Current Week
  </a>
</h2>

<div>
{%- include schedule.html -%}
</div>

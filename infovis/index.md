---
layout: archive
title: "可视化"
date: 2018-01-02T11:40:45-04:00
---
<a href="https://public.tableau.com/views/_18388/2_1?:embed=y&:display_count=yes&publish=yes"><img src="/images/Final Project.png" alt="Final Project.png"/></a>
<div class="tiles">
{% for post in site.categories.chart %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

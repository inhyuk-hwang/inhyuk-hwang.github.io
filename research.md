---
layout: page
title: "Research"
permalink: /research/
---

## Publications

{% for pub in site.data.publications %}
### {{ pub.title }}

{{ pub.journal }}{% if pub.note %} ({{ pub.note }}){% endif %}{% if pub.authors %} ({{ pub.authors }}){% endif %}
[\[Link\]]({{ pub.link }})

<details>
<summary>Show abstract</summary>
{{ pub.abstract }}
</details>

{% endfor %}
---

## Working Papers

{% for paper in site.data.papers %}
### {{ paper.title }}

{% if paper.status %}*{{ paper.status }}*{% if paper.authors %} ({{ paper.authors }}){% endif %}{% else %}{% if paper.authors %}({{ paper.authors }}){% endif %}{% endif %}
[\[{{ paper.link_text }}\]]({{ paper.file }}) · *Last updated: {{ paper.updated | date: "%Y-%m-%d" }}*

<details>
<summary>Show abstract</summary>
{{ paper.abstract }}
</details>

{% endfor %}
---

## Work in Progress

{% for paper in site.data.wip %}
### {{ paper.title }}

{% if paper.authors %}({{ paper.authors }}){% endif %}
{% if paper.file %}[\[{{ paper.link_text }}\]]({{ paper.file }}){% if paper.updated %} · *Last updated: {{ paper.updated | date: "%Y-%m-%d" }}*{% endif %}{% endif %}

<details>
<summary>Show abstract</summary>
{{ paper.abstract }}
</details>

{% endfor %}

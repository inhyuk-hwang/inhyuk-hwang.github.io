---
layout: page
title: "Research"
permalink: /research/
---

## Publications

### Race, immunity, and lifespan: Unraveling the effect of early-life exposure to malaria risk on lifespan

*Economics and Human Biology*, 54, 101382. 2024. (with [Sok Chul Hong](https://sites.google.com/site/sokchulhong/))
[\[Link\]](https://www.sciencedirect.com/science/article/abs/pii/S1570677X24000340)

<details>
<summary>Show abstract</summary>
We investigate a historical experience to measure the long-term effect of malaria on lifespan among infected survivors and identify a factor that mitigates malaria's effect. Using a sample of Union Army veterans born during the mid-19th century and their lifetime records, we show that exposure to high risk of malaria at birth or in early life substantially shortened their lifespan. The legacy of exposure to malaria is robust while controlling for lifetime socioeconomic and health conditions, fixed effects, and considering selection bias. Additionally, we include the US Colored Troops sample of black veterans to analyze racial differences in the effect of malaria exposure on lifespan. Exposure to malaria did not lead to a shorter lifespan among black veterans. Evidence suggests that genetic immunity to malaria in black veterans might contribute this heterogeneity.
</details>

### Mortality, Nutrition and Height in Early Colonial Korea

*Review of Economic History*, 67(2), 197–225. 2018. (in Korean)
[\[Link\]](https://kiss.kstudy.com/Detail/Ar?key=3626004)

<details>
<summary>Show abstract</summary>
The determinants of stature can be changed in one country by the change of cultural and economic situation. The cases of western countries in 19th century are good example. Therefore, identifying the determinants is needed to understand the change of stature in colonial Korea. In this study, I used Prisoners' cards made in prisons that provide a lot of information about their characteristic. What I found is that disease environments were important factors to determine people's stature in early colonial Korea. The change of the mortality rate that reflected disease environment explained the statural change.
</details>

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

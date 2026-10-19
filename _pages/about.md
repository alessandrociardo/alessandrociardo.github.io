---
permalink: /
title: "Alessandro Ciardo"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.on_the_market %}
<p class="jm-banner">
  <strong>I am on the {{ site.job_market_year }} economics job market</strong> and will be available for interviews.
</p>
{% endif %}

I am a PhD candidate in Economics at the **University of Barcelona** and a predoctoral researcher at
the **Barcelona Institute of Economics (IEB)**, where I am supervised by
[Jordi Jofre-Monseny](https://sites.google.com/site/jordijofresite/) and
[Andreu Arenas-Jal](https://sites.google.com/view/andreuarenas).

My research is in **urban and housing economics**. I use administrative microdata and quasi-experimental
designs to study how rental market regulation reshapes the housing market — who gets a lease, how long
they keep it, and which landlords stay in. I also work on the **political economy of migration**, asking
how historical population movements shape political preferences generations later.

Research interests
------

* Urban Economics
* Housing Economics
* Political Economy
* Public Economics

{% assign jmp = site.publications | where: "category", "jmp" | first %}
{% if jmp %}
Job market paper
------

<div class="paper paper--featured">
  <h3 class="paper__title"><a href="{{ jmp.url | relative_url }}">{{ jmp.title }}</a></h3>
  {% if jmp.coauthors and jmp.coauthors != "" %}<p class="paper__authors">{{ jmp.coauthors }}</p>{% endif %}
  <div class="paper__abstract">
    {{ jmp.content | markdownify }}
  </div>
  {% if jmp.paperurl %}
    <p class="paper__links"><a class="paper__link" href="{{ jmp.paperurl }}">Download paper</a></p>
  {% elsif jmp.draft_status %}
    <p class="paper__links"><span class="paper__note">{{ jmp.draft_status }}</span></p>
  {% endif %}
</div>
{% endif %}

{% comment %}
REFERENCES — hidden for now. To show them: delete the Liquid comment tag on the line above and the
matching closing tag below, then fill in the names. Add or remove a "refs__item" block per referee.

References
------

<div class="refs">
  <div class="refs__item">
    <strong>Name</strong><br />
    Affiliation<br />
    <a href="mailto:name@example.org">name@example.org</a>
  </div>
  <div class="refs__item">
    <strong>Name</strong><br />
    Affiliation<br />
    <a href="mailto:name@example.org">name@example.org</a>
  </div>
</div>
{% endcomment %}

Contact
------

You can reach me at [alessandro.ciardo@ub.edu](mailto:alessandro.ciardo@ub.edu). My full
[CV]({{ "/cv/" | relative_url }}) and the rest of my [research]({{ "/research/" | relative_url }})
are on this site.

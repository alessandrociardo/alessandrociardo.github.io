---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<p class="cv-download"><a class="paper__link" href="{{ base_path }}/files/cv-alessandro-ciardo.pdf">Download CV (PDF)</a></p>

<h2 class="cv-section">Current position</h2>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Predoctoral Researcher</span><br />
    Barcelona Institute of Economics (IEB)<br />
    PhD student in Economics, University of Barcelona
  </div>
  <div class="cv-entry__date">Oct. 2023 – present</div>
</div>

<h2 class="cv-section">Education</h2>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">University of Barcelona</span> — PhD in Economics<br />
    Research area: urban economics, political economy<br />
    Supervisors: Jordi Jofre-Monseny and Andreu Arenas-Jal
  </div>
  <div class="cv-entry__date">Oct. 2023 – present</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">University of Barcelona</span> — Topics in Applied Economics<br />
    Three courses, 15 ECTS
  </div>
  <div class="cv-entry__date">Jan. – Apr. 2024</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">University of Milan</span> — MSc in Economics and Political Science<br />
    Graduation grade: 110/110
  </div>
  <div class="cv-entry__date">Oct. 2018 – Dec. 2021</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">University of Oslo</span> — Erasmus+ exchange
  </div>
  <div class="cv-entry__date">Jan. – Jun. 2020</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">University of Milan</span> — BSc in Political Science<br />
    Graduation grade: 110/110 <em>cum laude</em>
  </div>
  <div class="cv-entry__date">Oct. 2015 – Jun. 2018</div>
</div>

<h2 class="cv-section">Research</h2>
{% for category in site.publication_category %}
  {% assign papers = site.publications | where: "category", category[0] | sort: "date" | reverse %}
  {% if papers.size > 0 %}
    <h3 class="cv-subsection">{{ category[1].title }}</h3>
    <ul class="cv-list">
      {% for paper in papers %}
        <li>
          <a href="{{ base_path }}{{ paper.url }}">{{ paper.title }}</a>{% if paper.coauthors and paper.coauthors != "" %}, <span class="cv-coauthors">{{ paper.coauthors }}</span>{% endif %}
        </li>
      {% endfor %}
    </ul>
  {% endif %}
{% endfor %}

<h2 class="cv-section">Research experience</h2>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Predoctoral Researcher</span>, Barcelona Institute of Economics (IEB)
  </div>
  <div class="cv-entry__date">Oct. 2023 – present</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Research Assistant</span>, University of Milan —<br />
    Department of Economics, Management and Quantitative Methods
  </div>
  <div class="cv-entry__date">Nov. 2022 – Apr. 2023</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Research Assistant</span>, University of Milan —<br />
    Department of Political Science
  </div>
  <div class="cv-entry__date">Apr. – Oct. 2022</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Research Assistant Internship</span>, University of Milan<br />
    Tutor: G. d'Adda
  </div>
  <div class="cv-entry__date">Feb. – Apr. 2021</div>
</div>

<h2 class="cv-section">Teaching</h2>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Teaching Assistant</span>, Spanish Economy<br />
    University of Barcelona
  </div>
  <div class="cv-entry__date">Fall 2024</div>
</div>

<h2 class="cv-section">Presentations</h2>
<div class="cv-entry">
  <div class="cv-entry__body">15th European Meeting of the Urban Economics Association, Barcelona</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">6th International Workshop on Rent Control, Stockholm</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">ISEG Lisbon Urban and Public Economics Mini Workshop on Housing, Lisbon</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">Housing Matters: How did we get here and where are we going? (CaCHE), Glasgow</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">PhD-Economics Virtual Seminar, online</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">IEB Internal Work in Progress Seminar, Barcelona</div>
  <div class="cv-entry__date">2026</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">BeNA Winter Workshop, Berlin (poster)</div>
  <div class="cv-entry__date">2025</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">UB PhD Workshop, Barcelona</div>
  <div class="cv-entry__date">2025</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">IEB Internal Work in Progress Seminar, Barcelona</div>
  <div class="cv-entry__date">2025</div>
</div>

<h2 class="cv-section">Fellowships and awards</h2>
<div class="cv-entry">
  <div class="cv-entry__body">Joan Oró Predoctoral Scholarship, Generalitat de Catalunya</div>
  <div class="cv-entry__date">2024 – present</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">PhD Scholarship, Barcelona Institute of Economics (IEB)</div>
  <div class="cv-entry__date">2023 – 2024</div>
</div>
<div class="cv-entry">
  <div class="cv-entry__body">College of Merit Scholarship, Italian Ministry of Education &amp; INPS</div>
  <div class="cv-entry__date">2015 – 2021</div>
</div>

<h2 class="cv-section">Skills</h2>
<div class="cv-entry">
  <div class="cv-entry__body">
    <span class="cv-entry__title">Software</span> &nbsp;Stata, R, QGIS, Python (basic)<br />
    <span class="cv-entry__title">Languages</span> &nbsp;Italian (native), English (advanced), Spanish (advanced)
  </div>
</div>

<h2 class="cv-section">References</h2>
<div class="refs">
  <div class="refs__item">
    <strong>Jordi Jofre-Monseny</strong><br />
    Universitat de Barcelona<br />
    <a href="mailto:jordi.jofre@ub.edu">jordi.jofre@ub.edu</a>
  </div>
  <div class="refs__item">
    <strong>Andreu Arenas-Jal</strong><br />
    Universitat de Barcelona<br />
    <a href="mailto:andreu.arenas@ub.edu">andreu.arenas@ub.edu</a>
  </div>
  <div class="refs__item">
    <strong>Mariona Segú</strong><br />
    Université Paris 1 Panthéon-Sorbonne<br />
    <a href="mailto:mariona.segu@univ-paris1.fr">mariona.segu@univ-paris1.fr</a>
  </div>
</div>

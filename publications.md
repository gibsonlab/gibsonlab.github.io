---
layout: default
title: Publications
permalink: /publications/
description: Publications from the Gibson Lab
---
### Selected representative work from the lab (see also <a href="https://scholar.google.com/citations?user=epg4RggAAAAJ&hl=en"><i class="fa fa-graduation-cap"></i> Google Scholar </a>)

<ul>
{% for pub in site.data.publications %}
<li> <p>
{% if pub.link %} <a href="{{ pub.link }}">{{ pub.title }}</a>
{% elsif pub.title %} {{ pub.title }}
{% endif %}
<br>
{{ pub.authors }} <br>
<i>{{ pub.where }}</i>, {{ pub.year }} <br>
{% if pub.pdf %} <button name="button" onclick="window.location.href='{{ pub.pdf }}'"><i class="far fa-file-pdf"></i> paper</button> {% endif %}
{% if sup.pdf %} <button name="button" onclick="window.location.href='{{ sup.pdf }}'"><i class="far fa-file-pdf"></i> supplement</button> {% endif %}
{% if pub.poster %} <button name="button" onclick="window.location.href='{{ pub.poster }}'"><i class="far fa-file-pdf"></i> poster</button> {% endif %}
{% if pub.presentation %} <button name="button" onclick="window.location.href='{{ pub.presentation }}'"><i class="far fa-file-pdf"></i> slides</button> {% endif %}
{% if pub.video %} <button name="button" onclick="window.location.href='{{ pub.video }}'"><i class="fas fa-video"></i> presentation</button> {% endif %}
{% if pub.arxiv %} <button name="button" onclick="window.location.href='{{ pub.arxiv }}'"><i class="ai ai-arxiv"></i>arXiv</button> {% endif %}
{% if pub.biorxiv %} <button name="button" onclick="window.location.href='{{ pub.biorxiv }}'">bioRxiv</button> {% endif %}
{% if pub.medrxiv %} <button name="button" onclick="window.location.href='{{ pub.medrxiv }}'">medRxiv</button> {% endif %}
{% if pub.github %} <button name="button" onclick="window.location.href='{{ pub.github }}'"><i class="fab fa-github"></i> GitHub</button> {% endif %}
{% if pub.news1name %} <button name="button" onclick="window.location.href='{{ pub.news1link }}'"><i class="far fa-newspaper"></i> {{ pub.news1name }}</button> {% endif %}
{% if pub.news2name %} <button name="button" onclick="window.location.href='{{ pub.news2link }}'"><i class="far fa-newspaper"></i> {{ pub.news2name }}</button> {% endif %}
{% if pub.news3name %} <button name="button" onclick="window.location.href='{{ pub.news3link }}'"><i class="far fa-newspaper"></i> {{ pub.news3name }}</button> {% endif %}
{% if pub.custom1name %} <button name="button" onclick="window.location.href='{{ pub.custom1link }}'">{{ pub.custom1name }}</button> {% endif %}
{% if pub.custom2name %} <button name="button" onclick="window.location.href='{{ pub.custom2link }}'">{{ pub.custom2name }}</button> {% endif %}
{% if pub.custom3name %} <button name="button" onclick="window.location.href='{{ pub.custom3link }}'">{{ pub.custom3name }}</button> {% endif %}

 </p>
</li>
{% endfor %}
</ul>

---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<ol class="bibliography">
{% for publication in site.data.publications %}
  <li>
    <div class="pub-row">
      <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
        <img src="{{ publication.image }}" class="teaser img-fluid z-depth-1">
        <abbr class="badge">arXiv</abbr>
      </div>
      <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
        <div class="title"><a href="{{ publication.paperurl }}">{{ publication.title }}</a></div>
        <div class="author"><strong>{{ publication.authors | join: ', ' }}</strong></div>
        <div class="periodical"><em>{{ publication.venue }}</em>, {{ publication.date | date: "%b. %Y" }}</div>
        <div class="links">
          <a href="{{ publication.paperurl }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        </div>
      </div>
    </div>
  </li>
{% endfor %}
</ol>

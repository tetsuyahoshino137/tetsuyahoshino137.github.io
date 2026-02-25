---
layout: default
title: Home
---

<!-- Profile -->
<div class="profile">
  <img src="photo.jpg" alt="{{ site.name }}">
  <div class="profile-info">
    <h1>{{ site.name }}</h1>
    <p>{{ site.position }}</p>
    <ul>
      <li>
        <span class="icon">@</span>
        <span>
          {{ site.email | replace: "@", "[at]" }}
          <button class="copy-btn" onclick="navigator.clipboard.writeText('{{ site.email }}')">Copy</button>
        </span>
      </li>
      <li>
        <span class="icon">📍</span>
        <span>{{ site.location }}</span>
      </li>
      <li>
        <span class="icon">📄</span>
        <a href="{{ site.cv }}">CV (December 2025)</a>
      </li>
    </ul>

    {% if site.seminars %}
    <strong>Upcoming Seminars/Conferences:</strong>
    <ul class="upcoming-list">
      {% for s in site.seminars %}
      <li>{{ s }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </div>
</div>

<hr>

<!-- Working Papers -->
<h2>Working Papers</h2>
<ul class="papers">
  {% for p in site.working_papers %}
  <li>
    {% if p.pdf %}<a href="{{ p.pdf }}">{{ p.title }}</a>{% else %}{{ p.title }}{% endif %}
    {% if p.coauthors %}({{ p.coauthors }}){% endif %}
    {% if p.slides or p.replication %}
    <br><span class="meta">{% if p.slides %}<a href="{{ p.slides }}">Slides</a>{% endif %}{% if p.slides and p.replication %} and {% endif %}{% if p.replication %}<a href="{{ p.replication }}">Replication codes</a>{% endif %}</span>
    {% endif %}
    {% if p.rnr %}<br><span class="meta journal">{{ p.rnr }}</span>{% endif %}
    {% if p.note %}<br><span class="meta">{{ p.note }}</span>{% endif %}
  </li>
  {% endfor %}
</ul>

<hr>

<!-- Publications -->
<h2>Publications</h2>
<ul class="papers">
  {% for p in site.publications %}
  <li>
    {% if p.pdf %}<a href="{{ p.pdf }}">{{ p.title }}</a>{% else %}{{ p.title }}{% endif %}
    {% if p.coauthors %}({{ p.coauthors }}){% endif %}
    <br><span class="meta journal">{% if p.journal_url %}<a href="{{ p.journal_url }}">{{ p.journal }} {{ p.year }}</a>{% else %}{{ p.journal }} {{ p.year }}{% endif %}</span>
  </li>
  {% endfor %}
</ul>

---
layout: page
title: Publications
permalink: /publications/
---

<!--
  Edit _data/publications.yml to add, remove, or reorder publications.
  Each entry there automatically appears in the list below — no need to
  touch this file for routine updates.
-->

{%- assign pubs = site.data.publications | sort: "year" | reverse -%}
{%- if pubs.size > 0 -%}
<ul class="posts">
  {%- for pub in pubs -%}
  <li>
    <div class="post-meta">
      <h2 class="post-title">{{ pub.title }}</h2>
      <div class="post-date">{{ pub.year }} · {{ pub.venue }}</div>
    </div>
    <div class="post">
      <p>{{ pub.authors }}</p>
      {%- if pub.note and pub.note != "" -%}
      <p><em>{{ pub.note }}</em></p>
      {%- endif -%}
      <p>
        {%- if pub.link and pub.link != "" -%}
          <a href="{{ pub.link }}">Link</a>
        {%- endif -%}
        {%- if pub.pdf and pub.pdf != "" -%}
          {%- if pub.link and pub.link != "" %} · {% endif -%}
          <a href="{{ pub.pdf | relative_url }}">PDF</a>
        {%- endif -%}
      </p>
    </div>
  </li>
  {%- endfor -%}
</ul>
{%- else -%}
<p>Publications coming soon.</p>
{%- endif -%}

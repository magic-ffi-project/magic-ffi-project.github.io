---
layout: page
title: Publications
description: Research outputs, reports, and deliverables from the MAGIC project.
---

The MAGIC project (2025–2028) is actively producing research results. This page will be updated as publications, deliverables, and datasets are released.

## Project Deliverables

<table class="info-table">
  <thead>
    <tr>
      <th>Deliverable</th>
      <th>Title</th>
      <th>WP</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    {% for d in site.data.deliverables %}
    <tr>
      <td>{{ d.id }}</td>
      <td>{{ d.title }}</td>
      <td>{{ d.wp }}</td>
      <td>
        {% if d.pdf %}
          <a class="btn-pdf" href="{{ '/publications/' | relative_url }}{{ d.pdf }}" target="_blank" rel="noopener">Completed &#x2197;</a>
        {% else %}
          <span class="tag">Planned ({{ d.due }})</span>
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>

---

## Peer-Reviewed Publications

<div class="pub-list">
{% for pub in site.data.publications %}
  <div class="pub-item"{% if pub.pdf %} data-pdf="{{ '/publications/' | relative_url }}{{ pub.pdf }}"{% endif %}>
    <p class="pub-ref"></p>
    <div class="pub-actions"></div>
    <pre class="bibtex-content" hidden>{{ pub.bibtex }}</pre>
  </div>
{% endfor %}
</div>

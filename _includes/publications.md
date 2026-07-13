<h2 id="publications" style="margin: 2px 0 15px;">Selected Publications</h2>

<p><strong>* denotes equal contribution. Shijing Wang is highlighted in bold.</strong></p>

<div class="publications">
{% for paper in site.data.publications.selected %}
  <div class="pub-entry" style="margin-bottom: 16px;">
    <div><strong>[{{ paper.venue }}]</strong> <a href="{{ paper.pdf }}" target="_blank">{{ paper.title }}</a></div>
    <div style="margin-top: 3px;">{{ paper.authors }}</div>
    <div style="margin-top: 3px;"><em>{{ paper.status }}</em>{% if paper.note %} · <strong style="color:#b23b2a;">{{ paper.note }}</strong>{% endif %}</div>
  </div>
{% endfor %}
</div>

<details>
  <summary><strong>Additional collaborative work</strong></summary>
  <div class="publications" style="margin-top: 12px;">
  {% for paper in site.data.publications.additional %}
    <div class="pub-entry" style="margin-bottom: 14px;">
      <div><strong>[{{ paper.venue }}]</strong> <a href="{{ paper.pdf }}" target="_blank">{{ paper.title }}</a></div>
      <div style="margin-top: 3px;">{{ paper.authors }}</div>
      <div style="margin-top: 3px;"><em>{{ paper.status }}</em>{% if paper.note %} · <strong style="color:#b23b2a;">{{ paper.note }}</strong>{% endif %}</div>
    </div>
  {% endfor %}
  </div>
</details>

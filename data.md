---
title: Data
permalink: data/
profile: true
---

<table>
    <thead>
      {% for row in site.data.google_sheet limit:1 %}
        <tr>
          {% for col in row %}<th>{{col}}</th>{% endfor %}
        </tr>
      {% endfor %}
    </thead>
    <tbody>
      {% for row in site.data.google_sheet offset:1 %}
        <tr>
          {% for col in row %}<td>{{col}}</td>{% endfor %}
        </tr>
      {% endfor %}  
    </tbody>
  </table>
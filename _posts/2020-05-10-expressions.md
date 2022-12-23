---
last_modified_at: 2022-02-06
layout: single
title: "English expressions"
---
Some everyday English expressions and idioms which I heard in my everyday working life and noted them down.

<table>
  {% for row in site.data.Expressions %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
{% endfor %}
</table>
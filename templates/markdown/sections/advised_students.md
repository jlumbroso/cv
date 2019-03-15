{% extends "section.md" %}

{% block body %}
{% for p in items %}

<table class="table table-hover">
{% for student in p.students %}
<tr>
  <td class='col-md-2'>{{ student.period }}</td>
  <td>
    {{ student.name }}, <em>{{ student.topic }}</em>
    <!-- {% if student.details %} -->
    <!-- <ul><li>{{ student.details }}</li></ul> -->
    <!-- {% endif %} -->
  </td>
</tr>
{% endfor %}
</table>
{% endfor %}
{% endblock body %}

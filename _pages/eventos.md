---
layout: page
title: Eventos
permalink: /eventos/
image: '/images/RetroCorner.JPG'

---

<div class="table-container">
  <table>
    <tr><th>Nome Evento</th><th>Descricao</th><th>Data Inicio</th><th>Data Fim</th><th>Localidade</th><th>Url</th></tr>
    {%  for item in site.data.events %}
        <tr><td>{{item.title}}</td><td>{{item.description}}</td><td>{{item.date_start}}</td><td>{{item.date_end}}</td><td>{{item.local}}</td> <td> <a href="{{item.url}}" target="_new">link </a> </td></tr>
    {% endfor %}
  </table>
</div>

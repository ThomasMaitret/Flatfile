---
title: Equipe
layout: default
ordre: 3
---

<ul class="listequipe">
  {% for partner in site.data.partners %}
    <li>
      <h3>{{ partner.nom }}</h3>
      <p>Age : {{ partner.age }}</p>
      <p>Hobby : {{ partner.hobbies }}</p>
    </li>
    <hr style="background:#999; border:0; height:2px; width:auto;" />
  {% endfor %}
</ul>
  
<ul class="club">
    {% for ligue in site.data.clubs %}
        {% for club in ligue[1] %}   
            <li>
                <p>{{ club.name }}</p>
            </li>
        {% endfor %}
    {% endfor %}
</ul>
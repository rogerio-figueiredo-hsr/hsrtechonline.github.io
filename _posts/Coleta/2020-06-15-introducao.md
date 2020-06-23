---
layout: post
title:  "Introdução"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/introducao
---	
# Introdução

O **FastQuest Coleta** é um produto da [HSRTECH](http://hsrtech.com.br/) empresa do grupo [HSR](https://hsr.specialistresearchers.com.br/), que tem por objetivo aplicar os questionários formulados na ferramenta [FastQuest Admin](https://hsrtechonline.github.io/fastQuestAdmin/introducao) de maneira fluída por meio de entrevistadores por telefone, pessoalmente, e sem entrevistador através da internet do entrevistado.

---

### Índice

<div>    
    {% assign sorted_posts = site.posts | sort: 'section' | where_exp: "item", "item.title != 'Introdução'" %}
    {% for post in sorted_posts %}
        {%if post.projeto == "fastQuestColeta" %}            
            {%if post.pasta %}{%else%}
                    <ul>
                        <li>
                            <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                        </li>
                    </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>   
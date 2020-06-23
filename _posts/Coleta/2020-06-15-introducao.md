---
layout: post
title:  "Introdução"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/introducao
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
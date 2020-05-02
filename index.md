---
title: About Me
feature_text: |
  ## Nguyễn Hoàng Anh 
  Welcome to my blog.
feature_image: "https://picsum.photos/1300/400?image=777"
excerpt: "My name is Nguyen Hoang Anh. I am currently working at ZaloPay as a Data Scientist. This blog is a place for me to organize and share the knowledge that I know."
layout: page
---
My name is Nguyen Hoang Anh. I am currently working at ZaloPay as a Data Scientist. This blog is a place for me to organize and share the knowledge that I know.
 <div class="content">

    <article class="article  article--page  typeset">

      {% if paginator.posts %}
        {% assign collectiondata = site.collections | where: "label", page.collectionpage | first %}
        <h1>{{ collectiondata.title }}</h1>
        {{ collectiondata.description | markdownify }}

      {% else %}
        <h1>{{ page.title }}</h1>
        {{ content }}
        
      {% endif %}

    </article>

    {% include post-list.html %}

  </div>
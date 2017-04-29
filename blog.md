---
layout: page
title: Blog
permalink: /Blog/
--- 
<div class="home">

<br>
<br>
 

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
      <center>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h2>
        </center>
        {{ post.excerpt }}
       
        <p>&#187; <a href="{{ site.baseurl }}{{ post.url }}" class="button button-primary">Leer post</a></p>
        
         {% include page_divider.html %} 
        
      </li>
    {% endfor %}
  </ul>
<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>



</div>
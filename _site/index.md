---
title: Welcome
date: Created
layout: base
tags:
  - welcome
  - info
  - hello
---
<nav class="site-main">
        
  <div class="intro-image">
      <img src="images/images/hi.png"  class="me" alt="" >
  </div>

  <div class="intro">
    
  </div>



</nav>    
<section class="grid">
  {% for page in collections.home %}      
  <article class="card">
    <div class="card__img"><img src="/images/images/{{ page.data.img }}" alt=""></div>
    <div class="card__content">
      <h1 class="card__header">{{page.data.name}}</h1>
      <p class="card__text">{{page.data.description}}</p>
      <a href="{{page.url}}" class="card__btn"><strong>View</strong></a> 
    </div>
  </article>
  {% endfor %}
</section>




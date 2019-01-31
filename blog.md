---
layout: default
title: Blog
---
<section class="space--sm bg--secondary">
      <div class="container">
      <h1 class="text-center">Marching Bytes Blog</h1>
          <div class="row justify-content-center">
              <div class="col-md-10 col-lg-8">
                  <div class="massonry masonry-blog-list">
                  {% for post in site.posts %}
                      <div class="masonry__container masonry--active">
                          <article class="masonry__item voh vnn " >
                              <div class="article__title text-center">
                                  <a href="{{post.url}}">
                                      <h2>{{post.title}}</h2>
                                  </a> <span>{{post.date | date_to_string}} </span></div>
                              <div class="article__body">
                                  <p> {{ post.excerpt }}</p> <a href="{{ post.url }}">Continue reading »</a> </div>
                          </article>
                          
                      </div>
                      {% endfor %}
                  </div>
              </div>
          </div>
      </div>
  </section>

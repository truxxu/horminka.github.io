---
layout: default
title: Blog
permalink: /blog/
lang: es
---

<!-- Intro Section -->
<section class="seccion-contacto">
  <div class="container">
    <div class="row">
      <div class="col-md-11">
        <h1 >Posts</h1>
        <ul class="post-list">
          {% for post in site.posts %}
          <li>
            <h3>
              <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
              <small class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</small>
            </h3>
            <p>
              {{ post.excerpt }}
            </p>
          </li>
          {% endfor %}
        </ul>
      </div>
    </div>
  </div>
</section>

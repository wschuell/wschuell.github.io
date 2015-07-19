---
layout: page
title: Research
permalink: /research/
---

My research interests are centered on Complex Systems approaches and models, applied mainly to these (sometimes overlapping) fields:

 * Computationnal linguistics
 * Development and Learning
 * Population dynamics in Biology


<div class="home">

  <h2 class="page-heading">Publications</h2>

  <ol class="post-list">
    {% for post in site.categories.publication %}
      <li>
        <h3>
          <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
        </h3>
        <span class="post-meta">{% if post.author %} {{ post.author }}{% endif %}{% if post.shortwhere %} • {{ post.shortwhere }}{% endif %}</span>
        <span class="post-meta">{% for link in post.links %} <a class="page-link" href="{{ link.lk | prepend: site.baseurl }}"> [{{ link.type }}]</a> {% endfor %}</span>


      </li>
    {% endfor %}
  </ol>

</div>

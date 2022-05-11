---
layout: page
title: Research
permalink: /research/
---

<current research>

I am currently involved in two projects:


**Project 1: Systemic Risk in Open Source Software Ecosystems**

How likely is it for me to get a bug in a software I just downloaded? With growing complexity in the network of software dependencies, relying on numerous open-source developers who sometimes are maintaining packages in their free time, the risk of bugs happening and propagating to a large amount of people is a growing concern.

By studying collaboration networks in specific ecosystems (e.g. around the languages Rust or Julia), we explore how to define relevant measures to quantify this kind of risk.

**Project 2: Systemic Risk in the Austrian Food Supply Chain**

By collecting data at the national level -- in collaboration with many actors--, we aim at reconstructing the food supply chain from production (e.g. farms) to consumers, and define proper risk measure, and build interactive tools for policy makers. How would the population be impacted by a lockdown of a given part of the country? What would be the result of closing certain borders?

We successfully built a prototype for the pork meat supply chain, and aim at extending this to all basic products.



**Reproducibility in Science**

I am trying to promote better habits in science concerning reproducibility, through improving better coding habits and learning from concepts existing in the software engineering community. I put as much of my work as possible on my [github account][gh].

I am still a learning developer, and potentially better solutions have been implemented by others by now, but my intents lead to:
 - a library to manage experiments and deploy them easily on clusters https://github.com/wschuell/experiment_manager
 - a template for python library repositories: https://github.com/wschuell/pylib_template
 - a library to construct modular datasets around git repositories: https://github.com/wschuell/repodepo


**PhD work**
My PhD work aimed at connecting those 2 fields: study the dynamics of language as a cultural phenomenon. Previous work on multi-agents models of language emergence and evolution (called Language Games) showed that it is possible for a population to agree on a common language while following simple rules. However, some features of the model stay non-realistic: there is a burst in complexity of what agents have to memorize, before reaching consensus.
In individual learning, some behaviors can be the key to an active control of complexity growth: active learning mechanisms, driven by curiosity and intrinsic motivation. My PhD work consisted in adapting this class of mechanisms to Language Games. We designed principled and cognitively plausible algorithms that effectively addressed the complexity issue. More generally, this also shows that individual intrinsic motivation can improve the efficiency of collective behavior and solve problems at population level. As final part of my PhD, we are currently running a user-experiment in the form of a web application, to test whether our algorithms are related to the performance level of humans put in the same conditions.

I benefited from the supervision of Pierre-Yves Oudeyer, my PhD advisor and Vittorio Loreto, who I visited in Rome for 6 months. Pierre-Yves Oudeyer is well-known for his work on curiosity and intrinsic motivation, but also on language emergence. Vittorio Loreto studied the Language Games from a physics point of view, and more recently has been working on computational models of creativity and innovation.

Another contribution I made during my PhD is a Python framework for computational simulations, aimed at non-computer science researchers wanting to quickly prototype and analyze computational models while keeping as low as possible the hassle of debugging and scaling to run the simulations on a computing cluster. This framework also makes it easy to share code and allows reproduction of experimental results. The framework is functional but under-documented and I am not actively maintaining it, but I would happily dive back into it if interested users contact me.

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

[gh]: https://github.com/wschuell
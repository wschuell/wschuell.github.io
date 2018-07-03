---
layout: page
title: Research
permalink: /research/
---


I am currently a PhD student at INRIA Bordeaux Sud-Ouest, under the supervision of Pierre-Yves Oudeyer. My PhD work focuses on the introduction of active learning mechanisms in computational models of language emergence and evolution. I am interested in computational models of social phenomena and cultural evolution; as well as individual learning strategies, especially in the domain of language.


This can be done using 3 approaches: building theoretical models to better understand existing phenomena; building algorithms based on this knowledge to solve computational problems (consensus dynamics,), and finally designing algorithms interacting with humans (such as educational applications or recommender systems).

**Background**
Individuals interacting in a group with simple rules can give rise to complex patterns: being the self-organization of a flock of birds, of ants finding the shortest path to their food, or a population collectively building a language. My master studies focused on the modelling of these phenomena, using multi-agent computational models, network science and statistical physics. For my masters' thesis, I conducted research with Jean-Louis Deneubourg in the Université Libre de Bruxelles, studying food policies in an anthill. I had previously built a strong knowledge about social insects behavior thanks to the teachings of my cousin Vincent Dietemann, entomologist at the Swiss Bee Research Center. Earlier in my studies, observing his experiments led me to design a computational model of a specific host/parasite relationship between 2 african honeybee species.

Language is a fantastic tool not only to communicate, but to teach and learn knowledge in general. Among existing languages and grammars, a great variety of strategies can be found, splitting conceptual spaces in many different ways, but also keeping the language easily learnable and understandable. During my studies I had the opportunity to do an internship with Ramon Ferrer i Cancho at the Polytechnic University of Catalonia on theoretical models of language, using tools from statistical physics and information theory. In parallel, his advice led me to learn catalan, and later get interested in various foreign languages, from persian to tagalog, including the whistled turkish of Kusköy.

**PhD work**
My PhD work aims at connecting those 2 fields: study the dynamics of language as a cultural phenomenon. Previous work on multi-agents models of language emergence and evolution (called Language Games) showed that it is possible for a population to agree on a common language while following simple rules. However, some features of the model stay non-realistic: there is a burst in complexity of what agents have to memorize, before reaching consensus.
In individual learning, some behaviors can be the key to an active control of complexity growth: active learning mechanisms, driven by curiosity and intrinsic motivation. My PhD work consisted in adapting this class of mechanisms to Language Games. We designed principled and cognitively plausible algorithms that effectively addressed the complexity issue. More generally, this also shows that individual intrinsic motivation can improve the efficiency of collective behavior and solve problems at population level. As final part of my PhD, we are currently running a user-experiment in the form of a web application, to test whether our algorithms are related to the performance level of humans put in the same conditions.

I benefited from the supervision of Pierre-Yves Oudeyer, my PhD advisor and Vittorio Loreto, who I visited in Rome for 6 months. Pierre-Yves Oudeyer is well-known for his work on curiosity and intrinsic motivation, but also on language emergence. Vittorio Loreto studied the Language Games from a physics point of view, and more recently has been working on computational models of creativity and innovation.

Another contribution I made during my PhD is a Python framework for computational simulations, aimed at non-computer science researchers wanting to quickly prototype and analyze computational models while keeping as low as possible the hassle of debugging and scaling to run the simulations on a computing cluster. This framework also makes it easy to share code and allows reproduction of experimental results. The framework is still under development, but already functional.

**Future work**
Concept exploration and innovation are studied in a series of computational models, but at individual level. Because it is also a collective phenomena, I aim at working on multi-agent versions with a social dimension, and study the impact of intrinsically motivated behavior at this level. Such a model could be useful to improve existing recommender systems, by understanding better the dynamics of advice-driven exploration. Another development of the model, following previous work on Language Games, would be about the co-evolution of knowledge and language, the latter being the necessary vector for spreading ideas efficiently. A particularly interesting aspect found in those models is the link between curiosity (as a drive for exploration) and creativity (exploring at the edge of what is known by the population, and possibly creating knowledge).

Language can also be seen as not only a vector to share knowledge, but also as having an influence on our conceptual perceptions. With this point of view, shaping language in a certain way can shape cognitive abilities, hence the notion of language-augmented thought. One of my goals is to show that this is not only limited to language but includes other phenomena like synesthesia. Understanding this process and finding efficient strategies could be useful for machine learning, education, cross-cultural studies, but also art: Exploring new ways of connecting different concepts or expressing them is at the core of the artistic work. Of course, such strategies could be heavily linked to intrinsic motivation, and collective behavior in the form of cultural evolution.

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

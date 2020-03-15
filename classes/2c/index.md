---
layout: page
title: Mathématiques 2ndes C
pagination: 
  enabled: true
  category: 2c
paginate: 5
paginate_path: "/2c/page:num/"
---

# Derniers billets

<div class="posts-list">
  {% for post in site.categories['2c'] %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
      <h2 class="post-title">{{ post.title }}</h2>

      {% if post.subtitle %}
      <h3 class="post-subtitle">
        {{ post.subtitle }}
      </h3>
      {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }} {% assign excerpt_word_count = post.excerpt
        | number_of_words %} {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
        <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a> {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tags#{{- tag -}}">{{- tag -}}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

  </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %} {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}


# Derniers billets
<div>
<ul class="posts">
  {% for post in site.categories['2c'] %}
    <li><span class="f1">{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
  {% endfor %}
</ul></div>

# Progression

## du 4 Sep au 18 Oct 2019
- [x] **Chapitre 1 Ensembles de nombres** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/18sIlFwGjF4q-eolaWihJXrGybE5fE4sK/view), 31/12/2019    
    **objectif maitriser les notations standards** [c.f. <i class="fab fa-wikipedia-w"></i>](https://en.wikipedia.org/wiki/ISO_31-11)  
- [x] **Chapitre 2 Automatismes**
- [x] **Chapitre 3 Information chiffrée**
- [x] **Algorithmie**
    - TP0 Parties A,B et C, boucles ```for``` et ```while```. Notions de listes et instruction ```range(debut,fin,pas)```. [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1xDKNHDa1OpkRUOIWac2EctvBMBfMMGbP/view)
    - Fonction `def return` et instructions conditionnelles ```if else``` et exercices [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1aLggkTDihTREXk9dPjlLisU5fnzFPRi_/view)
- [x] **Intérrogations et DS** 
	- DS 1 [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1XUq4s8k_Fgyu66FjlkpaUOM1wFl08rBz/view) 
	- Intérrogation racines carrées et puissances [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1D5JFdRE9JV4E6Q2v5j9fzOrM-jyY_nXa/view)
	- Intérrogation information chiffrée [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/15TfwWCX1_gI9mRcc3PT_Ol0QJuL5Fc0R/view)
## du 4 Nov au 20 Déc 2019
- [x] **Chapitre 2 Automatismes** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1aGfmUChKAvxm8R9gfyTih5IXmGCfLWro/view)
  - Factorisation Méthode 2 à l'aide d'identités remarquables
  - Racines carrées
- [x] **Chapitre 3 Information chiffrée** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/14Zak4LHb3k1ZSVaP9juqV-IQDW_EjHTo/view)  
- [x] **Chapitre 4 Repères et Vecteurs** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1VhDrMoAkHtze4JEHpLSJosuWdEj0W68K/view), 21/12/2019
- [x] **Chapitre 5 Équations et définition d'inéquations**  [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1trealkV9e8fDK8DcMXorqS9oxzhTX72M/view), 21/12/2019
- [x] **Algorithmie** 
	- TP1 Arithmétique et nombres entiers [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1T26MgRWu6omdnHSTNml7hATOlwSOxuJt/view)
	- Instruction conditionnelles ```if elif else``` [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1_p0MRbXAuharU-1045aaef9du1hd917n/view)  

## du 6 Jan au 21 Fév 2020
- [x] **Chapitre 6 Généralités sur les fonctions** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1Eg55zarmNretTjQPfhqtirAZWkJvVsD3/view)  
	Un article [Wikipedia <i class="fab fa-wikipedia-w"></i>](https://en.wikipedia.org/wiki/History_of_the_function_concept) en anglais sur l'évolution du concept de fonction.
- [x] **Chapitre 7 Relation d'ordre dans \\(\mathbb{R}\\) et résolution d'inéquations** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/17Oz3YsTiNMPSlOdWE89cey8A89NrJxqI/view), 
- [x] **Algorithmie** 
	- TP2 Principe d'accumulateur [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1YbW__48RrP63z6j0nI_JJ9uJgcFfXjEe/view)
	- TP3 Intérêts simples ou composés [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1D6Y5VRk06KYuMMGoMu-srNZMEB7jXuIk/view)
	- TP4 Simulation d'une expérience aléatoire [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1E6u9HM60J9OXILPQ3IDJia3qXeOcZ05A/view)
- [x] **Intérrogations et DS**  
	- Intérrogation vecteurs [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1oztvYjcc6UbfVCEYpn_NqNgX4Qn3JY1C/view)
	- DS 2 [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1DLFyJAs1yPkiTEXGyYke_R9c3STOx6ZR/view)
	- Flash Tests [01-Inéquations <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1j4Vk4Hs07MPTY0Vd30EfvPwZJ_kmK61n/view), [02-Fonctions <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1Zt5I5n1P4O-axYONrKrti6EHvEeHV7Rh/view).
	- Intérrogation Inéquations et fonctions : le [sujet <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1gy5ZWSzKldKVJHg4-owqRXJ4Fyq7ONrL/view) et la [correction <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/15-LkimIoOAy9dzbbaKcwHhKOiFLW8Jgg/view).
	
## du 9 Mar au 17 Avril 2020
- [x] **Chapitre 8 Probabilités** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1OrL_zmB1Tmj8sOxBOXrmcaktsD0fS3SF/view), 10/03/2019
	- AP Arbres de probabilité et application à un modèle génétique (Loi de Hardy-Weinberg) [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1jwBae4ynJtT_hR551sdaGZOdmuxngQSB/view) 
	- Échantillonnage [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1OIsTQ50aR9Mx0XRqwyrrFhZ0O0NxTogk/view)
- [ ] **Chapitre 9 Vecteurs(2)** [Cours <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1kka2Ui7xIrhUYfWfR_i5kyYBTQp5Md96/view) et [exercices <i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/13xPyTgqbMfu5svtRahe6ssyRnLUXe3m-/view).
- [ ] **Chapitre 10 Équations de droites** [<i class="far fa-file-pdf"></i>](https://drive.google.com/file/d/1bctJvsG3FXpszmO-vgv0w6llwjgM1x2g/view)
- [ ] **Chapitre 11 Fonctions de références** 
- [ ] **Intérrogations et DS**   
	- DS 3 [<i class="far fa-file-pdf"></i>]( )
	
## du 5 Mai au 3 Juillet 2020
- [ ] **Statistiques**
- [ ] **Géométrie**
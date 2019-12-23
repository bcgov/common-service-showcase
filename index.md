---
layout: default
name: HOME
---
<main role="main">
  {% assign intro = site.cards | where: 'type', 'intro' | first %}  
  {% assign services = site.cards | where: 'type', 'service' | sort: 'order' %}  
  {% assign showcases = site.cards | where: 'type', 'showcase' | sort: 'order' %}  
  {% assign allcards = services | concat: showcases %}  
  
  <!-- Main jumbotron for a primary marketing message or call to action -->
  <div class="jumbotron">
    <div class="container-fluid">
      <h1 class="display-3">{{ intro.title }}</h1>
      {{ intro.content }}
    </div>
  </div>

  <div class="container-fluid">
    {% for card in allcards %}
    <div class="card mb-1">
        <h5 class="card-header">{{ card.title }}</h5>        
        {% if card.img %}
            <img src="{{ site.baseurl }}{{card.img.path }}" class="card-img-top" alt="{{ card.img.alt }}">
        {% endif %}
        <div class="card-body">
            <div>{{ card.content }}</div>
            <a href="{{ card.urls.github }}" target="_blank" class="btn btn-primary">
                <i class="fab fa-2x fa-github align-middle" aria-hidden="true"></i>
                <span class="align-middle">Github</span>
            </a>
            <a href="{{ card.urls.prod }}" target="_blank" class="btn btn-link">
                <i class="align-middle fa-2x fa-external-link-alt fa-external-link-square-alt fas" aria-hidden="true"></i>
                <span class="align-middle">Try it out</span>
            </a>
           </div>
    </div> 
    {% endfor %}
    <hr class="mb-1" />
  </div>
</main>

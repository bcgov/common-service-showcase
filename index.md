---
layout: default
name: HOME
---
<main role="main">
  {% assign allcards = site.cards | sort: 'order' %}  
  
  <!-- Main jumbotron for a primary marketing message or call to action -->
  <div class="jumbotron">
    <div class="container-fluid">
      <h1 class="display-3">{{ site.title }}</h1>
      <p>{{ site.intro }}</p>
    </div>
  </div>

  <div class="container">
    {% for card in allcards %}
    <div class="card mb-1">
      <h5 class="card-header"><a id="{{ card.name }}"></a>{{ card.title }}</h5>        
      {% if card.img %}
      <img src="{{ site.baseurl }}{{card.img.path }}" class="card-img-top" alt="{{ card.img.alt }}">
      {% endif %}
      <div class="card-body">
        <div>{{ card.content }}</div>
        <div class="text-right">
          {% if card.urls.github %}
          <a href="{{ card.urls.github }}" target="_blank" class="btn btn-primary">
            <i class="fab fa-2x fa-github align-middle" aria-hidden="true"></i>
            <span class="align-middle">Github</span>
          </a>
          {% endif %}
          {% if card.urls.app %}
          <a href="{{ card.urls.app }}" target="_blank" class="btn btn-link">
            <i class="align-middle fa-2x fa-external-link-alt fa-external-link-square-alt fas" aria-hidden="true"></i>
            <span class="align-middle">Try it out</span>
          </a>
          {% endif %}
          {% if card.urls.docs %}
          <a href="{{ card.urls.docs }}" target="_blank" class="btn btn-link">
            <i class="align-middle fa-2x fa-external-link-alt fa-external-link-square-alt fas" aria-hidden="true"></i>
            <span class="align-middle">Review the API</span>
          </a>
          {% endif %}
        </div>
      </div>
    </div>
    {% endfor %}
    <hr class="mb-1" />
  </div>
</main>

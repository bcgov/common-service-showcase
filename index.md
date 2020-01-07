---
layout: default
name: HOME
---
<main role="main">
  {% assign allcards = site.cards | sort: 'order' %}  

  <!-- Main jumbotron for a primary marketing message or call to action -->
  <div class="jumbotron">
    <div class="container-fluid">
      <h3 class="display-4">{{ site.bannertitle }}</h3>
      <p>{{ site.intro }}</p>
    </div>
  </div>

  <div class="container">
    {% for card in allcards %}
    <div class="card mb-3">
      <div class="row no-gutters card-header">
        <div class="col-lg-8 col-md-6">
          <h5><a class="pt-6" id="{{ card.name }}"></a>{{ card.title }}</h5>
        </div>
        <div class="col-lg-4 col-md-6 text-right">
          {% if card.urls.onboarding %}
          <a href="{{ card.urls.onboarding }}" target="_blank" class="btn btn-link">
            <i class="align-middle fa-2x fa-external-link-alt fa-external-link-square-alt fas" aria-hidden="true"></i>
            <span class="align-middle">Create an account</span>
          </a>
          {% endif %}
          {% if card.urls.getstarted %}
          <a href="{{ card.urls.getstarted }}" class="btn btn-link">
            <i class="align-middle fa-2x fa-external-link-alt fa-external-link-square-alt fas" aria-hidden="true"></i>
            <span class="align-middle">Get started today</span>
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
      <div class="card-body">
        <div>{{ card.content }}</div>
        <div class="text-right">
          {% if card.urls.github %}
            <a href="{{ card.urls.github }}" target="_blank" class="btn btn-link">
            <i class="fab fa-2x fa-github align-middle" aria-hidden="true"></i>
            <span class="align-middle">Github</span>
          </a>
          {% endif %}
        </div>
      </div>
    </div>
    {% endfor %}
    <hr class="mb-1" />
  </div>
</main>

---
layout: default
name: HOME
---
<main role="main mb-5">
  {% assign carouselCards = site.overview | where: "type", "carousel" | sort: 'order' %}
  {% assign iconCards = site.overview | where: "type", "icon" | sort: 'order' %}
  {% assign checkerboardCards = site.overview | where: "type", "checkerboard" | sort: 'order' %}

  <div class="container">
    <div id="overviewCarousel" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        {% for card in carouselCards %}
          <li data-target="#overviewCarousel" data-slide-to="{{ forloop.index | minus: 1 }}" class="{% if forloop.index == 1 %} active{% endif %}"></li>
        {% endfor %}
      </ol>
      <div class="carousel-inner">
        {% for card in carouselCards %}
        <div class="carousel-item {% if forloop.index == 1 %} active{% endif %}">
          <div class="row">
            <div class="col-sm-5">
              <h4 class="carousel-card-header">{{ card.title }}</h4>
              <p>{{ card.content }}</p>
            </div>
            <div class="col-sm-7">
              <img class="img-fluid" src="{{ site.baseurl }}{{card.img.path }}" alt="{{ card.img.alt }}">
            </div>
          </div>
        </div>
        {% endfor %}
      </div>
      <a class="carousel-control-prev" href="#overviewCarousel" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="carousel-control-next" href="#overviewCarousel" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
    <div class="my-3 px-5">
      <p>Common Components are a set of reusable digital building blocks that solve common problems across government. We aim to promote, curate, develop, and make it easy to onboard to implement common components which will <strong><em>reduce costs, accelerate development, and promote consistency</em></strong> and supportability of BC Gov digital services</p>
      <div class="row">
        {% for card in iconCards %}
        <div class="icon-list col-sm-4">
            <img class="img-fluid" src="{{ site.baseurl }}{{card.img.path }}" alt="{{ card.img.alt }}">
            {{ card.content}}
        </div>
        {% endfor %}
      </div>
    </div>
    <div class="checkerboard mb-5">
      {% for card in checkerboardCards %}
      <div class="row">
        <div class="col-sm-4 check-title d-flex justify-content-center align-items-center">
            {{ card.title }}
        </div>
        <div class="col-sm-8 check-content">
            {{ card.content }}
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</main>

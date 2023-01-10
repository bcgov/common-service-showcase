---
layout: default
name: HOME
---
{% assign carouselCards = site.overview | where: "type", "carousel" | sort: 'order' %}
{% assign iconCards = site.overview | where: "type", "icon" | sort: 'order' %}
{% assign checkerboardCards = site.overview | where: "type", "checkerboard" | sort: 'order' %}
{% assign commonServices = site.services | sort: 'order' %}

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
          <div class="col-sm-5 carousel-card-text">
            <h4 class="carousel-card-header">{{ card.title }}</h4>
            <p>{{ card.content }}</p>
          </div>
          <div class="col-sm-7">
            <img class="img-fluid " src="{{ site.baseurl }}{{ card.img.path }}" alt="{{ card.img.alt }}">
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

  <div class="mb-3 mt-5 px-5">
    <p>This website provides information relating to a range of services and open-source software components created by the Common Service Showcase team. We aim to promote, curate, develop, and make it easy to onboard to our hosted services or integrate our micro-services and common components into your own applications. The goal is to <strong>reduce costs, accelerate development, and promote consistency</strong> and supportability of BC Gov digital services.</p>
    <div class="row">
      {% for card in iconCards %}
      <div class="icon-list col-sm-4">
          <img class="img-fluid" src="{{ site.baseurl }}{{ card.img.path }}" alt="{{ card.img.alt }}">
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
  <div class="text-center my-5">
    <h3 class="title-text" id="home-component-cards"> <img class="img-fluid mr-3" src="{{ site.baseurl }}/assets/images/developer_board.svg" alt="components"> <strong>Available Common Components</strong></h3>
  </div>
  <div class="mb-5 service-card-list">
    <div class="row">
      {% for card in commonServices %}
      <div class="col-md-6">
        <a class="linked-card" href="{{ site.baseurl }}{{ card.url }}.html">
          <div class="card">
            <div class="card-body">
              <div class="row">
                <div class="col-10 col-xl-11">
                  <h3 class="card-title">{{ card.title }} ({{ card.name }}) {{ card.version }}</h3>
                </div>
                <div class="col-2 col-xl-1 text-right">
                  <i class="fa fa-lg fa-arrow-circle-right"></i>
                </div>
              </div>
              <strong>Onboarding Options:</strong>
              <br />
              <ul class="service-onboard">
                {% for onb in card.onboard %}
                  <li>{{ onb }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </a>
      </div>
      {% endfor %}
    </div>
  </div>
</div>

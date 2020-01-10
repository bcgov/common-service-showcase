---
name: reuse  
title: Why do the work when we've done it for you?  
type: info  
order: 2  
permalink: /reuse.html  
img:
  - name: getok
    path: /assets/images/tokey.svg 
    alt: "Get Access Tokens" 
    url: "#GETOK"
  - name: ches
    path: /assets/images/missy.svg 
    alt: "Email Messaging" 
    url: "#CHES"
  - name: cdogs
    path: /assets/images/sam.svg 
    alt: "Doc Generation" 
    url: "#CDOGS"
---
<div class="row">
  <div class="col-lg-5 col-xs-12">
    <p>There is a set common services ready for you to use today. </p>
    <p>These services are reliable, highly available, and supported by an experienced team of developers on an Agile team in IITD. </p>
    <p><strong>Check out the APIs and showcase applications below to continue with the onboarding process</strong></p>
  </div>
  <div class="col-lg-7 col-xs-12">
       <div class="row">
          {% for item in page.img %}
            <div class="col-sm-4">{{ item.alt }}<br/>
            <a href="{{item.url}}">
            <img class="img-fluid my-3" src="{{ site.baseurl }}{{item.path }}" alt="{{ item.alt }}">
            </a>
            </div>
          {% endfor %} 
        </div>  
  </div>
</div>
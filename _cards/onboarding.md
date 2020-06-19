---
name: Onboarding
title: Getting access is simple and the services are free
type: info
order: 23
permalink: /onboarding.html
urls:
  onboarding: "https://getok.pathfinder.gov.bc.ca/getok"
---

The following onboarding process has been tested and we are looking for feedback to make it even better

1. A developer on your team must create an account by using their IDIR credentials to Login to [GetOK](#GETOK)
  a. In the navigation bar, go to _Request Account_ or _My Applications_ and click the _Add a new Application_ button, fill out the form with **_your_** application acronym (short name) and any additional comments.
  b. The GETOK support team will receive your request and confirm that approval to use the NRS Common Services.
1. After you are notified about your registration being completed, start a new GetOK session ([log out](#GETOK) and log in) and find your new application under _My Applications_.
1. Follow the steps in GETOK to promote a client and get credentials in a new environment or reset your client password.
1. **IMPORTANT:** Securely store your newly created client id and secret.  For example, create an Openshift secret to store the client's credentials.
1. Test your client's access to the Common Service API(s).
1. We encourage you to download our <a href="assets/files/common_services_postman_collection.json" download="common_services_postman_collection.json">Postman collection</a> and <a href="assets/files/common_services_postman_readme.md" download="common_services_postman_readme.md">instructions</a> to test your credentials and get familiar with the API usage. 
1. <a href="" data-toggle="modal" data-target="#exampleModal">Setup your Postman collection</a>
1. Write REST calls in your application to get a token and call the Common Services

<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel"
  aria-hidden="true">
  <div class="modal-dialog mw-100 w-50" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Setup your Postman collection</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img class="d-block w-100" src="assets/images/postman_guide/step1.png"
                alt="Import the collection">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step2.png"
                alt="Edit collection variables">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step3.png"
                alt="Enter your Service Client and Password and email">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step4.png"
                alt="Open collection runner">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step5.png"
                alt="Run the collection">
            </div>
          </div>
          <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
      <div class="modal-footer">
        <ul>
          <li>Import the collection</li>
          <li>Edit the collection variables</li>
          <li>Enter your Service Client and Password and email</li>
          <li>Open the collection runner</li>
        </ul>
      </div>
    </div>
  </div>
</div>

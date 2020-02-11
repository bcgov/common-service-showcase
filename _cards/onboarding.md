---
name: Onboarding
title: Getting access is simple and the services are free
type: info
order: 23
permalink: /onboarding.html
urls:
  onboarding: "https://getok-master-k8vopl-prod.pathfinder.gov.bc.ca/api/auth/login"
---

The following onboarding process has been tested and we are looking for feedback to make it even better

1. A developer on your team must create an account by using their IDIR credentials to Login to [GetOK](#GETOK)
	a. Click the _Register New App_ button to send the GETOK an email with your application acronym (short name) and your IDIR account name.
	b. The GETOK support team will receive your request and confirm that approval to use the NRS Common Services.
1. After you are notified about your registration being completed, start a new GetOK session ([log out](#GETOK) and log in) and see that you are authorized to configure the requested application.
1. Follow the steps in GETOK to create a client and get credentials.
1. **IMPORTANT:** Securely store your newly created client id and secret.  For example, create an Openshift secret to store the client's credentials.
1. Test your client's access to the Common Service API(s).
1. We have put all our API calls into a [Postman collection](assets/files/common_services_postman_collection.json), making it easier to test with your data and get familiar with the API usage. <a href="" data-toggle="modal" data-target="#exampleModal">Authorize your Postman requests with an Access Token</a>
1. Write REST calls in your application to get a token and call the Common Services

<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel"
  aria-hidden="true">
  <div class="modal-dialog mw-100 w-50" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Authorize your Postman requests with an Access Token</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img class="d-block w-100" src="assets/images/postman_guide/step1.png"
                alt="Edit the Common Services collection">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step2.png"
                alt="Get a new Access Token">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step3.png"
                alt="Enter your Service Client and Password">
            </div>
            <div class="carousel-item">
              <img class="d-block w-100" src="assets/images/postman_guide/step4.png"
                alt="Inherit auth from parent">
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
					<li>Edit the top-level Common Services collection</li>
					<li>Click 'Get a new Access Token'</li>
					<li>Enter your Service Client and Password and use this token</li>
					<li>Make sure each of the API calls have Authorization as 'Inherit auth from parent'</li>
				</ul>
			</div>
    </div>
  </div>
</div>

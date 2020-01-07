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
1. Utilize the Postman collection(s) and test data to get familiar with the API usage.  
1. Write REST calls in your application to get a token and call the Common Services 

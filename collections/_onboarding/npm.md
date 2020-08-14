---
layout: onboarding

name: NPM
title: NPM
order: 3
---
#### NPM @bcgovimage

The purpose of NPM is to share independently usable packages of code for teams to achieve a variety of capabilities in their systems. This depends on how they choose to use each package. For example, our Common Service Showcase Team is using a few of these packages to delivery the functionality contained in the Document Generation API image which we published to DockerHub. We are also hosting that doc-gen image as an API that teams, who do not want to host their own instance of, can make webservice calls to.

##### Packages

<!-- TODO: Consider iterating over the collections here to dynamically build this.
For each service that has npm packages as an onboard type. Figure out how... -->
{% assign cdogs = site.services
| where_exp:"service", "service.name == 'CDOGS'"
| first %}
{% include common/npmTable.html param=cdogs %}

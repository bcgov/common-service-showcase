---
layout: service
type: service

name: COMS
title: Common Object Management Service
order: 5
description: >-
  Using COMS, take advantage of more cost-effective storage solutions for your new or existing business applications.
  COMS is a secure REST API that lets you connect your application to an S3 bucket.
  In S3, you can store and share files, images, and documents with co-workers, partners, or the public.

onboard:
  - 'Hosted Service'
  - 'DockerHub'
onboardDescription: >-
  COMS is now available as a shared hosted service as well as an application that you can customise and deploy
  in your own infrastructure.
  See our documentation of <a href="https://github.com/bcgov/common-object-management-service/wiki/Hosting-Considerations" target="_blank">hosting
   considerations</a> and <a href="https://github.com/bcgov/common-object-management-service/wiki/Deployment-Guide" target="_blank">deployment
   guide</a> in the COMS wiki.<br /><br />
  We have also launched <a href=" https://bcbox.nrs.gov.bc.ca/" target="_blank">BCBox</a>, a user-interface for managing files,
  integrated with the hosted COMS service.
urls:
  hosted: https://coms.api.gov.bc.ca
  github: https://github.com/bcgov/common-object-management-service/
  docs: https://coms.api.gov.bc.ca/api/v1/docs
  guide: https://github.com/bcgov/common-object-management-service/wiki
  ui: https://bcbox.nrs.gov.bc.ca/
showcaseDescription: >-
  BCBox (test) implements the COMS API to manage and share files within government or with the public.

dockerImages:
  - name: Common Object Management Service
    url: https://hub.docker.com/r/bcgovimages/common-object-management-service/
    description: This image provides a fast way to set up an object management API with a range of features focusing on object management, permission control, and object discovery.
    badges:
      - https://img.shields.io/docker/v/bcgovimages/common-object-management-service.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/common-object-management-service.svg
      - https://img.shields.io/docker/image-size/bcgovimages/common-object-management-service.svg

---
- Upload, download, manage and delete objects
- Discover, update and manage object versions
- Toggle general public access to objects
- Grant and manage refined user object permissions
- Add, update, and remove object metadata and tags
- Flexible search and filter capabilities based on objects and user permissions

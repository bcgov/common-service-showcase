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
  - 'Self Hosted Service'
  - 'DockerHub'
onboardDescription: We provide <em>Docker Images</em> for hosting your own Common Object Management Storage Service.
urls:
  github: https://github.com/bcgov/common-object-management-service/
  docs: https://coms-dev-master.apps.silver.devops.gov.bc.ca/api/v1/docs
  showcase: https://comss-dev-master.apps.silver.devops.gov.bc.ca/app/

showcaseDescription: >-
  The Common Object Management Service Showcase (COMSS) is a demonstration of how an application can use S3 to manage and share objects within government or with the public.

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

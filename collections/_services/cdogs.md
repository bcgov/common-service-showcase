---
layout: service
type: service

name: CDOGS
title: Common Document Generation Service
order: 2
description: >-
  Leverage your structured datasets and your business templates to automatically populate printable documents, spreadsheets, presentations, or PDFs using the Common Document Generation Service.

onboard: ['API Access', 'DockerHub']
onboardDescription: We provide <em>API Access, Docker Images, and NPM Packages</em> for the Common Document Generation Service.
urls:
  github: https://github.com/bcgov/common-document-generation-service
  guide: https://github.com/bcgov/common-document-generation-service/wiki
  docs: https://cdogs.api.gov.bc.ca/api/v2/docs
  showcase: https://dgrsc-prod-master.apps.silver.devops.gov.bc.ca
pictures:
  icon: sam.svg
  header: cdogs.svg

showcaseDescription: >-
  The Document Generation Showcase demonstrates the capabilities of the Common Document Generation Service API (CDOGS).
  You will also find example templates you can download to get you started within this demo app.

dockerImages:
  - name: Common Document Generation Service
    url: https://hub.docker.com/r/bcgovimages/common-document-generation-service
    description: This image provides a fast way to set up a container (Alpine Linux, NodeJS, the LibreOffice library).
    badges:
      - https://img.shields.io/docker/v/bcgovimages/common-document-generation-service.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/common-document-generation-service.svg
      - https://img.shields.io/docker/image-size/bcgovimages/common-document-generation-service.svg

  - name: Alpine Node LibreOffice
    url: https://hub.docker.com/r/bcgovimages/alpine-node-libreoffice
    description: The main CDOGS image (above) is built on this dependency image that contains the open source LibreOffice application running on Alpine Node. Alpine Node is a minimal Node.js built on Alpine Linux.
    badges:
      - https://img.shields.io/docker/v/bcgovimages/alpine-node-libreoffice.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/alpine-node-libreoffice.svg
      - https://img.shields.io/docker/image-size/bcgovimages/alpine-node-libreoffice.svg

---
The API can generate any PDF or XML-based documents such as docx, xlsx, pptx, odt, ods, odp, and html. Examples of XML-based editors include Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;.

- Merge complex datasets into document templates
- Supports any XML-based document templates including but not limited to Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;
- Rich templating library support leveraging the Carbone JS library

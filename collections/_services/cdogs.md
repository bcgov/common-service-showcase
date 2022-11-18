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
  docs: https://cdogs.api.gov.bc.ca/api/v2/docs
  showcase: https://dgrsc.apps.silver.devops.gov.bc.ca/dgrsc/
  postman: /common-service-showcase/assets/files/CDOGS.postman_collection.json
  postmanHelp: /common-service-showcase/assets/files/common_services_postman_readme.md
pictures:
  icon: sam.svg
  header: cdogs.svg

showcaseDescription: >-
  The Document Generation Showcase demonstrates the capabilities of the Common Document Generation Service API (CDOGS).

dockerImages:
  - name: Alpine Node LibreOffice
    url: https://hub.docker.com/r/bcgovimages/alpine-node-libreoffice
    description: This Docker image contains the open source LibreOffice application running on Alpine Node. Alpine Node is a minimal Node.js built on Alpine Linux.
    badges:
      - https://img.shields.io/docker/v/bcgovimages/alpine-node-libreoffice.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/alpine-node-libreoffice.svg
      - https://img.shields.io/docker/image-size/bcgovimages/alpine-node-libreoffice.svg
  - name: Common Document Generation Service
    url: https://hub.docker.com/r/bcgovimages/common-document-generation-service
    description: This image provides a fast way to set up a document generation API with a range of features like template caching, support for a wide range of file formats and file type conversions (including PDF).
    badges:
      - https://img.shields.io/docker/v/bcgovimages/common-document-generation-service.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/common-document-generation-service.svg
      - https://img.shields.io/docker/image-size/bcgovimages/common-document-generation-service.svg
  - name: "[Deprecated] Document Generation API"
    url: https://hub.docker.com/r/bcgovimages/doc-gen-api
    description: "[Deprecated] This image provides a fast way to set up a document generation API with a range of features like template caching, support for a wide range of file formats and file type conversions (including PDF). Succeeded by Common Document Generation Service."
    badges:
      - https://img.shields.io/docker/v/bcgovimages/doc-gen-api.svg?sort=semver
      - https://img.shields.io/docker/pulls/bcgovimages/doc-gen-api.svg
      - https://img.shields.io/docker/image-size/bcgovimages/doc-gen-api.svg

npmPackages:
  - name: "[Deprecated] Carbone Copy API"
    url: https://www.npmjs.com/package/@bcgov/carbone-copy-api
    description: "[Deprecated] Express library that provides and interface for generating documents from templates and data. It provides a local file storage cache that means callers do not have to upload the template for each render. Callers should should store cache keys/hashes and check if templates exist before generation. This is a wrapper around carbone, please refer to their documentation for more detail. The API follows their recommendations."
    badges:
      - https://img.shields.io/npm/v/@bcgov/carbone-copy-api.svg
      - https://img.shields.io/npm/dm/@bcgov/carbone-copy-api.svg
  - name: "[Deprecated] Carbone Render"
    url: https://www.npmjs.com/package/@bcgov/carbone-render
    description: "[Deprecated] Library to generate a document from an existing template and JSON data. This is a wrapper around carbone, please refer to their documentation for more detail."
    badges:
      - https://img.shields.io/npm/v/@bcgov/carbone-render.svg
      - https://img.shields.io/npm/dm/@bcgov/carbone-render.svg
  - name: "[Deprecated] File Cache"
    url: https://www.npmjs.com/package/@bcgov/file-cache
    description: "[Deprecated] Library to store files locally identified by a hash of the file contents. A sub-directory is created and identified by a hash of the file, the original file is then stored under the hash sub-directory. The hash is created when writing the binary contents to disk. Each file will generate a unique hash."
    badges:
      - https://img.shields.io/npm/v/@bcgov/file-cache.svg
      - https://img.shields.io/npm/dm/@bcgov/file-cache.svg

---
The API can generate any PDF or XML-based documents such as docx, xlsx, pptx, odt, ods, odp, and html. Examples of XML-based editors include Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;.

- Merge complex datasets into document templates
- Supports any XML-based document templates including but not limited to Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;
- Rich templating library support leveraging the Carbone JS library

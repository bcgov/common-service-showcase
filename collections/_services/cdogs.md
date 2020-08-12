---
layout: service
type: service

name: CDOGS
title: Common Document Generation Service
order: 2
description: >-
  Leverage your structured datasets and your business templates to automatically populate printable documents, spreadsheets, presentations, or PDFs using the Common Document Generation Service.

onboard: ['API Access', 'DockerHub', 'NPM']
onboardDescription: We provide <em>API Access, Docker Images, and NPM Packages</em> for the Common Document Generation Service.
urls:
  github: https://github.com/bcgov/common-document-generation-service
  docs: https://cdogs-master-idcqvl-prod.pathfinder.gov.bc.ca/api/v2/docs
  showcase: https://dgrsc.pathfinder.gov.bc.ca/dgrsc/

showcaseDescription: >-
  The Document Generation Showcase demonstrates the capabilities of the Common Document Generation Service API (CDOGS).

dockerImages:
  - name: Document Generation API image
    url: https://hub.docker.com/r/bcgovimages/doc-gen-api
  - name: Libre Office Image for generating PDFs
    url: https://hub.docker.com/r/bcgovimages/alpine-node-libreoffice

npmPackages:
  - name: File Cache
    url: https://www.npmjs.com/package/@bcgov/file-cache
    description: Library to store files locally identified by a hash of the file contents. A sub-directory is created and identified by a hash of the file, the original file is then stored under the hash sub-directory. The hash is created when writing the binary contents to disk. Each file will generate a unique hash.
  - name: Carbone Render
    url: https://hub.docker.com/r/bcgovimages/alpine-node-libreoffice
    description: Library to generate a document from an existing template and JSON data. This is a wrapper around carbone, please refer to their documentation for more detail.
  - name: Carbone Copy API
    url: https://www.npmjs.com/package/@bcgov/carbone-copy-api
    description: Express library that provides and interface for generating documents from templates and data. It provides a local file storage cache that means callers do not have to upload the template for each render. Callers should should store cache keys/hashes and check if templates exist before generation. This is a wrapper around carbone, please refer to their documentation for more detail. The API follows their recommendations.
---
The API can generate any PDF or XML-based documents such as docx, xlsx, pptx, odt, ods, odp, and html. Examples of XML-based editors include Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;.

- Merge complex datasets into document templates
- Supports any XML-based document templates including but not limited to Microsoft Office&#x2122;, LibreOffice&#x2122; or OpenOffice&#x2122;
- Rich templating library support leveraging the Carbone JS library



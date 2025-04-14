---
layout: service
type: service

title: BCBox
order: 1
description: >-
  <a href="https://bcbox.nrs.gov.bc.ca/" target="_blank">BCBox</a> is a website that uses the <a href="https://bcgov.github.io/common-service-showcase/services/coms.html" target="_blank">Common Object Management Service</a> and your S3 Bucket so <a href="https://www2.gov.bc.ca/gov/content/governments/services-for-government/information-management-technology/id-services/idir" target="_blank">IDIR</a> and <a href="https://www.bceid.ca/" target="_blank">BCeID</a> users can upload and share files with each other or the public.
youtubeEmbed: https://www.youtube.com/embed/uu-C9oua6uc
descriptionExt: >-
  Using BCBox, you can use a website to access cost-effective storage and easily share files with coworkers, partners, or the public. All you need is an S3 bucket to get started.
onboard:
  - 'Hosted Service'
onboardDescription: >-
  Simply go to <a href="https://bcbox.nrs.gov.bc.ca/" target="_blank">BCBox</a> to get started. <br><br>We also offer <a href="https://bcgov.github.io/common-service-showcase/services/coms.html" target="_blank">Common Object Management Service (COMS)</a> as a shared hosted service or application you can customize and deploy in your own infrastructure.
urls:
  hosted: https://bcbox.nrs.gov.bc.ca
  github: https://github.com/bcgov/bcbox
  guide: https://github.com/bcgov/bcbox/wiki/User-Manual
  apiLink:
    text: Common Object Management Service (COMS)
    link: https://bcgov.github.io/common-service-showcase/services/coms.html
  support:
   url: https://teams.microsoft.com/l/channel/19%3A4e700366d8aa46479a7998ffa7c86a6a%40thread.tacv2/COMS%20and%20BCBox?groupId=bef8086f-20c7-43a4-bd07-29ce764e818c&tenantId=6fdb5200-3d0d-4a8a-b036-d3685e359adc
   text: MS Teams channel
button: true
pictures:
  icon: bcbox.svg
  header: bcbox_header.svg

---
- A web interface to upload and download files
- File access control and permission management
- Secure file sharing with BCeID/IDIR users and the public
- File search and ability to add tags and metadata to your files
- File versioning
- Connects to any S3-compatible object-storage service (eg: Dell ECS or AWS S3)
- Integrates with other apps using the SSO 'Standard' Keycloak realm

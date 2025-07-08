---
layout: service
type: service

title: BCBox
order: 1
description: >-
  <a href="https://bcbox.nrs.gov.bc.ca/" target="_blank">BCBox</a> is a web interface for managing files in object storage. With its fine-grained user permissions and invite features, it's easy to share files within government or with contactors and citizens.
youtubeEmbed: https://www.youtube.com/embed/uu-C9oua6uc
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
- Secure file sharing within government and with citizens using <a href="https://id.gov.bc.ca/account/" target="_blank">BC Services Card</a> and <a href="https://www.bceid.ca/" target="_blank">BCeID</a> accounts
- File search and ability to add tags and metadata to your files
- File versioning and restoring deleted files (if supported by object storage)
- Connects to any S3-compatible object-storage service (eg: Dell ECS, Minio or AWS S3)
- Integrates with other apps using the SSO 'Standard' Keycloak realm

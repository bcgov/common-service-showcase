---
layout: service
type: service

name: CAVMS
title: ClamAV Mirror Service
order: 4
description: >-
  A lightweight containerized ClamAV Mirror Service using CVD-Update and Caddy.
  Use this mirror service for your ClamAV definition updates to reduce external network traffic.
  Made simple and maintained by the Common Service Showcase team and available for your antivirus definition needs.
onboard:
  - 'Hosted Service'
onboardDescription: We provide a <em>Hosted Service</em> as well as documented <em>open-source code</em> for hosting your own ClamAV Mirror service.
button: true
urls:
  hosted: https://clamav-mirror.apps.silver.devops.gov.bc.ca
  github: https://github.com/bcgov/clamav-mirror
  docs: https://github.com/bcgov/clamav-mirror/blob/master/README.md
  guide: https://github.com/bcgov/clamav-mirror/blob/master/README.md
pictures:
  icon: clamav.webp
#   header: ???.svg
---
- Keep your ClamAV instance up to date with freshclam
- Intelligently update definitions using differential data
- Secure and accessible only from within the OCP4 Silver cluster

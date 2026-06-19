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
  support:
   url: https://teams.microsoft.com/l/channel/19%3AqztmPpuePgw_2JUN20Q41vhFSP0RNuu1aSal0br0WxY1%40thread.tacv2/General?groupId=bef8086f-20c7-43a4-bd07-29ce764e818c&tenantId=6fdb5200-3d0d-4a8a-b036-d3685e359adc
   text: Microsoft Teams channel
pictures:
  icon: clamav.webp
#   header: ???.svg
---
- Keep your ClamAV instance up to date with freshclam
- Intelligently update definitions using differential data
- Accessible and secure exclusively from within three tiers of the OpenShift platform

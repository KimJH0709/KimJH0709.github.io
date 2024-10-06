---
title: Multi-PC environment monitoring and remote chat technology
authors:
  - admin
date: "2024-10-01"
doi: ""
publication_types: ["article"]
summary: Frontend Project
tags:
  - React
  - Firebase
  - Mantine UI
featured: true
links:
url_code: "https://github.com/jbnu-capstone-jjinjjin/project"
image:
  caption: "Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)"
  focal_point: ""
  preview_only: false
---

# Feature Summary

## Web Browser(admin-page)

1. Inquire HW information, SDK information, and RESOURCE information of the client.
2. Based on the client's RESOURCE information, obtain the PID of the program running on the client, using that PID to forcefully terminate the program running on the client.
3. Capture and query the current screen of the ClientClient.

## Server(backend)

1. Store HW information, SDK information, and RESOURCE information of the client.
2. Save the screenshot sent by the client.
3. Forward the command from admin-page to the Client.
4. Forward the client's information to the admin-page so that it can be viewed.

## Client(collector)

1. Collect and send HW information, SDK information, and RESOURCE information of the currently installed device to the server. Of these, RESOURCE information is sent in a user-defined time cycle (default 5 minutes).
2. When the server receives a command and receives a PID, it terminates that PID. After that, update the RESOURCE information once again and send it to the server.
3. Take the command from the server, capture the screenshot, and forward it to the server.

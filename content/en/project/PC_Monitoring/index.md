---
title: 다중 PC 환경 모니터링 및 원격 채팅 기술
authors:
  - admin
date: "2024-10-01"
doi: ""
publication_types: ["article"]
summary: 프론트앤드 프로젝트
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

# 기능 요약

## Web Browser(admin-page)

1.  Client의 HW정보, SDK정보, RESOURCE 정보를 조회합니다.
2.  Client의 RESOURCE 정보를 토대로 Client에서 실행중인 프로그램의 PID를 얻습니다. 해당 PID를 이용해 Client에 실행중인 프로그램을 강제로 종료합니다.
3.  Client의 현재 화면을 캡처하여 조회합니다.

## Server(backend)

1.  Client의 HW정보, SDK정보, RESOURCE 정보를 저장합니다.
2.  Client가 전송한 Screenshot을 저장합니다.
3.  admin-page에서 내린 명령을 Client에 전달합니다.
4.  admin-page에 Client의 정보를 전달하여 조회할 수 있도록 합니다.

## Client(collector)

1.  현재 설치된 기기의 HW정보, SDK정보, RESOURCE 정보를 수집하여 서버에 보냅니다. 이중 RESOURCE 정보는 사용자가 정의한 시간(기본 5분)주기로 전송합니다.
2.  서버에서 명령을 받아 PID를 전달받으면 해당 PID를 종료시킵니다. 이후 RESOURCE 정보를 다시한번 갱신하여 서버에 전송합니다.
3.  서버에서 명령을 받아 Screenshot를 캡처하여 서버로 전달합니다.

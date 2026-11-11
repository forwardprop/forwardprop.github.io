---
title: "바이낸스 63억 달러 해킹 분석 — 블록체인이 아니라 개발자 노트북에서 시작됐다"
date: 2026-11-11 12:00:00 +0900
categories: [사건 분석, 암호화폐 거래소]
tags: [binance, 공급망, 사회공학, 가짜채용, macos, homebrew, eip-7702, 북한, tradertraitor, att&ck]
---

> **초안** — 2026년 11월 3일 바이낸스 예비 보고서와 언론 보도를 바탕으로 정리했다. 외부 검증 전 단계라 세부 내용은 바뀔 수 있다.
{: .prompt-info }

## 한 줄 요약

2026년 10월 29일 바이낸스 핫월렛에서 약 63억 달러가 빠져나갔다. 공격자는 개인키를 훔치지 않았다. 약 다섯 달에 걸쳐 지갑 인프라 팀 엔지니어들의 노트북을 차례로 장악한 뒤, **바이낸스 내부 서명 시스템이 스스로 출금에 서명하게** 만들었다.

## 타임라인

| 시기 | 무슨 일이 있었나 | 공격자가 얻은 것 |
|---|---|---|
| 2026년 6월 | 지갑 DevOps 엔지니어(A)가 AI 코딩 도구를 설치하려고 검색하다가 **변조된 Homebrew 설치본**을 받아 설치. 바이낸스가 탐지해 기기 교체·자격증명 교체 | **누가 지갑 인프라를 다루는지**(팀 구성) |
| 2026년 9월 | 다른 엔지니어(B)에게 가짜 채용 담당자가 접근. 가짜 HR·가짜 CEO 면접 뒤 **과제 저장소**를 실행하게 함 → 백신이 못 잡은 새 악성코드 감염 | 장기 거점(노트북 B) |
| 2026년 10월 20일 | B의 노트북에서 **사내 AI 도구**를 악용해 A와 지갑 소프트웨어 엔지니어(C)의 컴퓨터까지 장악, **컨테이너 배포 토큰** 확보 | 내부 배포 권한 |
| 2026년 10월 29일 | 컨테이너를 배포해 내부 **지갑 서명 서비스**에 접근, 출금 시작 | 정상 서명이 붙은 출금 |

바이낸스는 노트북 외에도 추가 침투 지점이 있었다고 밝혔지만, 아직 세부 내용은 공개하지 않았다.

<!-- 여기부터 직접 작성: 방어 관점의 교훈, 내 생각, 출처 목록 -->

## 방어 관점에서 배운 점

(작성 예정)

## 출처

- [SOCRadar – Binance Hack: Inside the $6.3B Hot Wallet Theft](https://socradar.io/blog/binance-hack-6-3b-hot-wallet-theft/)
- [BleepingComputer – Binance says fake job interview led to $6.3 billion crypto heist](https://www.bleepingcomputer.com/news/security/binance-says-fake-job-interview-led-to-63-billion-crypto-heist/)
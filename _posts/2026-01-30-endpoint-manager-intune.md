---
title: "[MS-900] 엔드포인트 관리 A to Z: Intune, MAM, 그리고 Autopatch"
date: 2026-01-30
categories: [Study, Security]
tags: [Intune, MDM, MAM, Autopatch, WindowsUpdate, MS-900]
---

# 📱 PC와 모바일을 관리하는 모든 기술 총정리

M365 관리자의 핵심 업무는 직원들의 **PC와 모바일 기기(Endpoint)**를 안전하고 효율적으로 관리하는 것이다.
단순히 기기를 등록하는 것부터, 윈도우 업데이트를 자동화하는 것까지 **Microsoft Endpoint Manager**의 핵심 기술들을 한 번에 정리한다.

## 1. Microsoft Intune (클라우드 관리의 핵심)
- **정의:** 클라우드 기반의 모바일 기기 관리(MDM) 및 모바일 앱 관리(MAM) 서비스.
- **역할:** 직원이 어디에 있든 보안 정책을 내리고, 앱을 설치하고, 설정을 변경할 수 있다.
- **Co-management (공동 관리):** 기존의 서버 방식(Configuration Manager)과 클라우드 방식(Intune)을 **동시에** 사용하여, 천천히 클라우드로 넘어가는 과도기 기술.

## 2. MDM vs MAM (시험 필수 구분!)
개인 폰과 회사 폰을 관리하는 방식은 달라야 한다.

| 구분 | **MDM (Mobile Device Management)** | **MAM (Mobile Application Management)** |
| :--- | :--- | :--- |
| **관리 대상** | **기기 전체** (Device) | **특정 앱** (Application) |
| **주 사용처** | 회사 지급 기기 (Corporate-owned) | 개인 소유 기기 (BYOD - 내 폰) |
| **관리 권한** | 기기 초기화, 암호 강제, 카메라 차단 | 앱 데이터 복사 방지, 앱 암호 설정 |
| **핵심** | **"기기를 통제"** | **"데이터만 통제"** |

## 3. 배포 자동화: Windows Autopilot
- **Zero Touch Deployment:** IT 관리자가 PC 포장을 뜯어서 세팅할 필요가 없다.
- 직원은 새 PC를 배송받아 로그인만 하면, 자동으로 와이파이, 앱, 보안 정책이 설치된다.

## 4. 업데이트 자동화: Windows Autopatch (최신 트렌드)
관리자가 밤새워 업데이트 버튼을 누르던 시절은 지났다.
- **기능:** Windows 품질/기능 업데이트, 드라이버, M365 앱 업데이트를 **자동화**.
- **원리:** **배포 링(Ring)**을 자동으로 나누어, 소수 그룹에 먼저 테스트하고 안전하면 전사로 배포.
- **조건:** Windows Enterprise E3 이상 라이선스 + Intune 등록 필수.

## 💡 관리자 노트
> **"엔드포인트 관리의 3단계 진화"**
> 1.  **Intune**으로 기기를 클라우드에 연결하고 (MDM/MAM)
> 2.  **Autopilot**으로 신규 입사자 PC 지급을 자동화하며
> 3.  **Autopatch**로 윈도우 업데이트 스트레스에서 해방되는 것.
>
> 이것이 모던 워크플레이스(Modern Workplace) 관리자가 가야 할 길이다.
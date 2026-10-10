# KEEPING Rebuild

> 선결제 포인트 공유 플랫폼 **KEEPING**을 다시 설계하고 개선하는 개인 프로젝트

<br>

## 프로젝트 소개

**KEEPING**은 고객이 매장에 포인트를 미리 충전하고, 개인 지갑 또는 그룹 지갑으로 공유해 사용할 수 있는 선결제 플랫폼입니다.

이 저장소는 SSAFY 13기 핀테크 프로젝트로 개발한 KEEPING을 기반으로, 프론트엔드·백엔드·데이터베이스·인프라 전반을 분석하고 다시 설계합니다.

<br>

## 목표

| 영역 | 내용 |
|---|---|
| 설계 | 기존 코드와 아키텍처를 분석하고 리팩토링 |
| 도메인 | 외부 금융망 의존성을 제거하고 가상 포인트 시스템으로 대체 |
| 데이터 | 트랜잭션, 동시성 제어, 데이터 정합성을 학습하고 적용 |
| 프론트엔드 | 성능과 사용자 경험 개선 |
| 인프라 | Docker, CI/CD, 클라우드 배포와 운영 |
| 기록 | 기술 선택과 문제 해결 과정을 블로그에 정리 |

<br>

## 기존 기술 스택

| 영역 | 기술 |
|---|---|
| Frontend | Next.js 15, React 19, TypeScript, Zustand, Tailwind CSS |
| Backend | Java 17, Spring Boot 3.5, Spring Security, Spring Data JPA |
| Database | MySQL 8.0, Redis 7 |
| Messaging | Kafka, SSE, Firebase Cloud Messaging |
| Infrastructure | Docker Compose, Nginx, AWS S3 |

> 기술 스택은 재설계 과정에서 바뀔 수 있습니다.

기존 시스템 아키텍처와 실행 방법은 [`exec/README.md`](exec/README.md)에 있습니다.

<br>

## 디렉토리 구조

```
.
├── backend/              # Spring Boot API 서버
├── frontend/             # Next.js 웹 클라이언트 (PWA)
├── infra/                # Nginx, Redis 설정
├── env/                  # 환경 변수 예시 파일
├── exec/                 # 기존 프로젝트 산출물 (DB 덤프, 시나리오, 아키텍처)
└── docker-compose.yml
```

<br>

## 로드맵

- [ ] 기존 프로젝트 구조 및 아키텍처 분석
- [ ] 핵심 기능과 금융망 의존성 파악
- [ ] 시스템 아키텍처 재설계
- [ ] 가상 지갑 및 결제 시스템 구현
- [ ] 프론트엔드 리팩토링
- [ ] 테스트 및 성능 개선
- [ ] 인프라 구성 및 배포

<br>

## 개발 기록

학습한 개념, 기술적 의사결정, 실험과 개선 과정을 블로그에 기록합니다.

**Blog** · https://nunnong.pages.dev/

<br>

---

<p align="center"><i>동작하는 코드를 넘어, 왜 이렇게 설계했는지 설명할 수 있는 개발자를 목표로 합니다.</i></p>

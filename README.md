## Branch Strategy

| 브랜치명          | 용도                           | 비고                                                    |
|------------------|--------------------------------|----------------------------------------------------------|
| `main` (또는 `release`) | 최종 배포본                       | 프로덕션 서버와 동기화                                     |
| `develop`        | 기능 통합용 개발 브랜치              | QA 및 스테이징 서버 대상                                   |
| `develop-internal` | 추가 기능 개발 브랜치                | 기업 연계와 무관한 기능 개발. 사용 방식은 `develop`과 동일          |
| `feature/*`      | 기능 단위 구현 브랜치                | 예: `feature/login-api`                                  |
| `fix/*`          | 버그 수정 브랜치                   | 예: `fix/invalid-token`                                  |
| `qa`             | QA 전용 브랜치                   | QA 팀에서 테스트 시 사용                                  |
| `staging`        | 시연/컨펌 전용 중간 서버용 브랜치        | 클라이언트/내부 시연에 사용                                |
| `hotfix/*`       | 운영 긴급 수정 브랜치                | 바로 `main`에 머지됨                                     |

-----
## 생성된 브랜치 리스트 (2025-06-18)
  - * main : 최종 배포본
  - develop : RFP를 기반으로 개발한 기능 통합용 개발 브랜치
    - feature/TTASUM-84-org-chart-chatbot : 챗봇 AI 기능 / API 개발
    - feature/TTASUM-83-donationLetters : 기증후 스토리 API 개발
    - feature/TTASUM-88-heavenLetters-service : 하늘나라 편지 API 개발
    - feature/TTASUM-95-donor-notice-view : 기증자 추모관 & 공지사항 API 개발
    - feature/TTASUM-114-FE-main : 홈 화면 API 개발
    - feature/TTASUM-117-recipientLetters-service : 수혜자 편지 API 개발
    - feature/TTASUM-111-logging-mysql : 로그 DB 저장

  - develop-internal : 필수 기능과 추가적인 기능 통합용 개발 브랜치
    - feature/TTASUM-112-admin-blameText : 글 의도 감정 AI 기능 / AOP 개발
    - feature/TTASUM-86-forbidden-word-check-service : 비난 글 판단 AI 기능 / AOP 개발 **(deprecated)**
    - feature/TTASUM-121-git-action-CI-CD : Git-Action Ci/CD 파이프라인
    - feature/TTASUM-116-profanity-filtering : 비난 단어 필터링 **(deprecated)**
    - feature/TTASUM-108-flower-service : 편지 감정 분석 AI 기능 / 감정에 맞는 꽃 추천 기능 / API 개발 
    - feature/TTASUM-106-logging : 로깅 ELK 파이프라인

  - hotfix : 개발 도중 설정/운영 관련 전체적인 수정 브랜치
    - hotfix/TTASUM-115-env-security : DB URL, ID 환경설정 보안
    - hotfix/TTASUM-118-donation-package-renaming : 패키지명 Donation -> donation 으로 변경
    - hotfix/TTASUM-119-donation-conflict-solve : 기증자 관련 conflict 해결 **(deprecated)**
    - hotfix/TTASUM-87-update-DB-properties : DB pw 환경설정 보안
    - hotfix/TTASUM-96-change-root-directory : repository root 경로 변경



  
  
  
  











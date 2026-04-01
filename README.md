# 김희수 | Back-end Developer

  처음 보이는 문제를 그대로 믿지 않았어요.
  같은 문제도 어떻게 보느냐에 따라 접근 방식이 달라질 수 있기 때문이에요.

  배포 지연은 단순 서버 성능 문제가 아니라 서버에서 직접 빌드하던 구조의 병목으로 봤어요.
  파일 업로드 부하는 서버 최적화 문제가 아니라 서버를 경유하는 구조의 비효율로 판단했어요.

  지금의 구현보다 다음 변경의 비용을 먼저 봤어요.
  개인의 코드보다 팀 전체가 다루기 쉬운 구조를 만드는 데 더 관심을 두고 개발했어요.

  <p>
    <a href="mailto:huisukim9905@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
    <a href="https://github.com/Tarte12"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" /></a>
    <a href="https://velog.io/@emprimula/posts"><img src="https://img.shields.io/badge/Blog-20C997?style=flat-square&logo=velog&logoColor=white" /></a>
  </p>

  ---

  ## Skills
  ### Backend
  <p>
    <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" />
    <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" />
    <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" />
    <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white" />

  ### Frontend
  <p>
    <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
    <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
    <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" />
  </p>

  ### Database & Infra
  <p>
    <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
    <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
    <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
    <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" />
    <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
    <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  </p>

  ---

  ## 최근에 이런 걸 했어요

  ### [Cohi-Chat](https://github.com/CheHyeonYeong/cohi-chat)
  > 개발자 간 1:1 커피챗 예약 서비스

  풀스택으로 참여하면서 인증/보안과 예약 도메인 쪽을 주로 맡았어요.
  최근에는 채팅 기능 구현과 배포 구조 개선까지 함께 다뤘어요.

  #### 핵심 경험
  - 리프레시 토큰 재사용 감지 한계를 보완하기 위해 일회성 토큰 회전 구조를 설계했어요.
  - 재사용 감지 시 전체 세션을 즉시 강제 종료하는 체계를 구성했어요.
  - 전체 데이터 조회 후 애플리케이션에서 후처리하던 구조를 DB 단계 필터링으로 재배치했어요.
  - 불필요한 데이터 전송과 메모리 사용을 줄이고 조회 로직 확장 비용을 낮췄어요.
  - EC2 현장 빌드로 20분+ 걸리던 채팅 서버 배포를 GitHub Actions 사전 빌드 + S3 이미지 전달 구조로 재
  설계했어요.
  - 부분 캐시를 적용해 운영 배포 시간을 **3분 내**로 단축했어요.
  - 코드 컨벤션, lint 자동화, AI 병렬 실행 프로세스를 도입해 인당 주간 PR 처리량 평균을 **2개 → 5개+**
  로 개선했어요.

  #### 관련 키워드
  `Spring Boot` `Spring Security` `JWT` `OAuth2` `Redis` `JPA` `GitHub Actions` `Docker` `NestJS`

  ---

  ### [Carhartt](https://github.com/woonkim0413/Carhartt_used_transactions_backend)
  > 브랜드 의류 중고 거래 서비스

  주문/결제 도메인 중심의 백엔드를 구현했어요.

  #### 핵심 경험
  - 파일 업로드가 애플리케이션 서버를 직접 경유하던 구조를 Presigned URL 기반 직접 업로드로 전환했어
  요.
  - 서버 네트워크 부하를 **50%+** 줄였고, 커넥션 점유 시간을 **P99 90%+** 단축했어요.
  - 결제 수단별 규격 차이로 분기와 검증 비용이 누적되던 구조를 전략 패턴 기반으로 재설계했어요.
  - 기능별로 달랐던 API 응답 형식과 예외 처리 방식을 공통 응답 구조와 에러 처리 기준으로 정리했어요.

  #### 관련 키워드
  `Spring Boot` `JPA` `AWS S3` `Presigned URL` `Strategy Pattern` `API Design`

  ---

  ### [CodingTestStudy](https://github.com/Tarte12/CodingTestStudy)
  > 꾸준한 코딩테스트 풀이 저장소

  구현력과 문제 해결 감각을 유지하려고 꾸준히 문제를 풀었어요.

  ---

  ## 오픈소스에도 기여했어요

  - [Spring Cloud Gateway](https://github.com/spring-cloud/spring-cloud-gateway/pull/4118) 문서 기여를
  했어요.
    글로벌 CORS 설정 경로 오류를 수정하는 PR이 머지됐어요.

  - [Valkey](https://github.com/valkey-io/valkey/pull/3419) 문서 기여를 했어요.
    `valkey.conf`의 listpack threshold 설명을 보강하는 PR이 머지됐어요.

  ---

  ## 최근 이런 것에 관심을 두고 있어요

  - AI Agent를 실제 개발 흐름에서 더 잘 쓰는 방법에 관심을 두고 있어요.
  - MSA와 분산 서버 환경에서의 장애 감지와 대응에 관심을 두고 있어요.
  - Kafka, 메시징 구조, 비동기 처리 방식에 관심을 두고 계속 공부하고 있어요.
  - 검색, 데이터 흐름, 성능 병목처럼 구조를 다시 정의해야 풀리는 문제에 관심을 두고 있어요.

  ---

  ## 이런 걸 공부했어요

  - [Kafka 스터디](https://velog.io/@emprimula/kafka1) | `2026.03 - 진행 중`
  - [돼드락(데이터 중심 애플리케이션 설계) 스터디](https://velog.io/@emprimula/ddia6) | `2025.12 - 진
  행 중`
  - [빅설기(대규모 시스템 설계 기초) 스터디](https://velog.io/@emprimula/big12) | `2025.11 - 2025.12`
  - [릴마큐(Real MySQL 8.0) 스터디](https://velog.io/@emprimula/realmysql42) | `2025.11 - 2026.01`
  - 자바/스프링 스터디 | `2025.04 - 2025.08`

  ---

  ## AI-Driven Development

  - AI를 단순 코드 생성기가 아니라, 작업 규칙과 병렬 흐름을 함께 설계하는 보조 도구로 활용했어요.
  - Claude Code, CodeRabbit, Git Worktree를 조합해 리뷰 부담을 줄이고 병렬 작업 흐름을 정리해 봤어요.
  - AI가 만든 결과를 그대로 쓰기보다, 검증 기준과 수정 기준을 먼저 세운 뒤 반영했어요.

  ---

  ## Stats & Activity

  <div align="center">
    <a href="https://www.gitanimals.org/en_US?utm_medium=image&utm_source=Tarte12&utm_content=farm">
      <img src="https://render.gitanimals.org/farms/Tarte12" width="600" height="300" />
    </a>
  </div>

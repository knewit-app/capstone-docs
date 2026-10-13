# meeting-log

수업(회의) 1회차당 1엔트리. 팀 리더 주도하에 **돌아가며** 작성하고, 이 파일 **하단에 append** 한다.
기록 목적: 강의 시간 동안 수행한 일 + 시행착오·의사결정 → 추후 보고서 작성 시 참고자료.

<details>
<summary>✍️ 작성 규칙 · 템플릿 (복붙용)</summary>

**규칙**

- 새 엔트리는 항상 파일 **맨 아래**에 추가한다. 기존 엔트리 수정/삭제 금지 (오타 수정은 예외).
- 분량은 엔트리당 **200단어(한글 어절 기준) 이내**. 서술형 문장 대신 명사형으로 끊는다.
- 해당 회차에 진행 사항이 없는 파트 줄은 **지운다** (`-` 만 남기지 않기).
- 시행착오는 `T-YYMMDD-n`, 의사결정은 `D-YYMMDD-n` 으로 번호를 붙인다.
  → 보고서에서 `D-260904-1` 처럼 인용 가능.
- 링크는 문서 원문보다 **커밋 / PR / 이슈 / 리포트 파일** 링크를 우선한다.
- 커밋 메시지: `docs(meeting-log): YYYY-MM-DD 회의록 추가`

**템플릿**

````markdown
<details>
<summary><b>YYYY-MM-DD (요일)</b> · 기록 이름 · 참석 N/N</summary>

**한 일**

- 🍎 기획 ·
- 💛 디자인 ·
- 🎾 FE ·
- 💎 BE ·
- 🟪 AI ·

**시행착오**

- `T-YYMMDD-1` 문제 → 시도 → 결과

**의사결정**

- `D-YYMMDD-1` 안건 → 채택안 (근거) / 폐기안 (사유)

**다음 회의까지**

- [ ] @이름 —
- [ ] @이름 —

</details>
````

</details>

---

<!-- ↓ 이 아래로 회차별 엔트리를 append 합니다. 최신 회차가 파일 맨 아래에 오도록. -->

<details>
<summary><b>2026-09-03 (목)</b> · 겨레 · 참석 3/3</summary>

**한 일**

- 🐈‍⬛ 공통 · 9/10 발표(4번째 팀, 5분+질의 1분) 준비 착수 — 주제·배경, 지난 학기, 이번 학기 계획.
- 🍎 기획 · ICT/SW 구체화 방향. 거리 비례 추천 ↔ "동네 정하고 간다" 가설 충돌, 거점 복수 가정 필요. new/knew 기준에 "오랜만에 방문" 포함. 페르소나별(프랜차이즈 술집) 검토.
- 🎾 FE · [knewit-fe](https://github.com/knewit-app/knewit-fe) 초기 의존성 세팅 완료. PR·이슈 템플릿은 `.github` main 머지 후.
- 💎 BE · [poc-place-attributes](https://github.com/knewit-app/poc-place-attributes) 5단계 구현(원장 적재 → 표본 50곳 → 카카오 교차검증 → 네이버 스니펫 수집 → Haiku 4.5 속성 추출), 채점 단계 미구현. [poc-taste-profile](https://github.com/knewit-app/poc-taste-profile) v5 푸시, 선호 정보 긍정 평가.

**시행착오**

- `T-260903-1` 속성 추출 정확도 미달 → 스니펫 + LLM 판정 → 영업시간 50% 이하, 콘센트·와이파이 저조. 원천 커버리지 부족 판단, 쿼리 개선 필요.
- `T-260903-2` 채점 셋 자동 구축 불가(LLM 네이버 지도 검색 정책 차단) → 지도 수기 확인해 GT 15곳 라벨링으로 전환.
- `T-260903-3` 프랜차이즈 지점 식별 실패(`스타벅스 아현점` → 타 지점 매칭) → 미해결.

**의사결정**

- `D-260903-1` 반려동물 `N` 처리 → `X`로 간주 채택 (동반 불가 명시 리뷰 희소) / 3값 유지 폐기 (N 편중).
- `D-260903-2` PoC 발표 범위 → 현 결과 보류, 채점 셋 수기 구축 → 재채점 → 쿼리 디벨롭 순.
- `D-260903-3` 진행 계획안 형식 → md 표 vs 노션 타임라인 뷰 미정, 차기 확정.

**다음 회의까지**

- [ ] @겨레 — poc-taste-profile 푸시 마무리
- [ ] @지인 — 채점 셋 수기 구축 + 재채점, poc-place-attributes 정리
- [ ] @민지인 — `.github` 레포 PR 리뷰·승인
- [ ] @전원 — 파트별 이번 학기 진행 계획안, 계획발표 PPT(디스코드 서면회의)

</details>

<details>
<summary><b>2026-09-03 (목)</b> · 겨레 · 참석 3/3</summary>

**한 일**

- 🐈‍⬛ 공통 · 9/10 발표(4번째 팀, 5분+질의 1분) 준비 착수 — 주제·배경, 지난 학기, 이번 학기 계획.
- 🍎 기획 · ICT/SW 구체화 방향. 거리 비례 추천 ↔ "동네 정하고 간다" 가설 충돌, 거점 복수 가정 필요. new/knew 기준에 "오랜만에 방문" 포함. 페르소나별(프랜차이즈 술집) 검토.
- 🎾 FE · [knewit-fe](https://github.com/knewit-app/knewit-fe) 초기 의존성 세팅 완료. PR·이슈 템플릿은 `.github` main 머지 후.
- 💎 BE · [poc-place-attributes](https://github.com/knewit-app/poc-place-attributes) 5단계 구현(원장 적재 → 표본 50곳 → 카카오 교차검증 → 네이버 스니펫 수집 → Haiku 4.5 속성 추출), 채점 단계 미구현. [poc-taste-profile](https://github.com/knewit-app/poc-taste-profile) v5 푸시, 선호 정보 긍정 평가.

**시행착오**

- `T-260903-1` 속성 추출 정확도 미달 → 스니펫 + LLM 판정 → 영업시간 50% 이하, 콘센트·와이파이 저조. 원천 커버리지 부족 판단, 쿼리 개선 필요.
- `T-260903-2` 채점 셋 자동 구축 불가(LLM 네이버 지도 검색 정책 차단) → 지도 수기 확인해 GT 15곳 라벨링으로 전환.
- `T-260903-3` 프랜차이즈 지점 식별 실패(`스타벅스 아현점` → 타 지점 매칭) → 미해결.

**의사결정**

- `D-260903-1` 반려동물 `N` 처리 → `X`로 간주 채택 (동반 불가 명시 리뷰 희소) / 3값 유지 폐기 (N 편중).
- `D-260903-2` PoC 발표 범위 → 현 결과 보류, 채점 셋 수기 구축 → 재채점 → 쿼리 디벨롭 순.
- `D-260903-3` 진행 계획안 형식 → md 표 vs 노션 타임라인 뷰 미정, 차기 확정.

**다음 회의까지**

- [ ] @겨레 — poc-taste-profile 푸시 마무리
- [ ] @지인 — 채점 셋 수기 구축 + 재채점, poc-place-attributes 정리
- [ ] @민지인 — `.github` 레포 PR 리뷰·승인
- [ ] @전원 — 파트별 이번 학기 진행 계획안, 계획발표 PPT(디스코드 서면회의)

</details>

<details>
<summary><b>2026-09-15 (화)</b> · 겨레 · 참석 3/3</summary>

**한 일**

- 🐈‍⬛ 공통 · 계획 발표 준비.

</details>

<details>
<summary><b>2026-09-17 (목)</b> · 지인 · 참석 3/3</summary>

**한 일**

- 🐈‍⬛ 공통 · 계획 발표 준비.

</details>

<details>
<summary><b>2026-09-22 (화)</b> · 민지인 · 참석 3/3</summary>

**한 일**

- 🎾 FE · 프로토타입 디자인 토큰 이식, 공용 UI, 모달·다단 detent 바텀시트, 3탭 IA 재정렬, 목데이터 typed service 계층. 지도 셸·마커(방향 콘), 로그인·초대 랜딩, 약관, 카드사 선택·로그인, 동기화·첫 방문 요약, 홈 지도·추천 시트. Sentry 연결.
- 💎 BE · CodeRabbit, Terraform + S3 원격 상태, VPC·EC2·EIP·S3·EBS 스냅샷·CloudWatch, OIDC 배포 역할. 테스트 베이스·프로파일(local/prod/web/worker/scheduler), Flyway V1, CI(GHCR 푸시).

**시행착오**

- `T-260922-1` detekt Java 25 비호환 → CI에서 임시 제외 → 미해결.
- `T-260922-2` refactor-scan 이슈 닫히면 중복 억제 풀림 → 억제 로직 수정, 기준점 레포 변수 → git ref.
- `T-260922-3` 방문 확인 후 방문 목록 갱신 안 됨 → 캐시 무효화 누락 수정. orval 하위 js-yaml 취약점 → override 고정.

**의사결정**

- `D-260922-1` 초기 스택 → Redis→Caffeine, ShedLock→Spring Modulith, PG16→PostGIS 17, Java 21→25 ([#27](https://github.com/knewit-app/knewit-be/pull/27)).
- `D-260922-2` DNS → 가비아 A 레코드 채택 / Route 53 폐기 ([#26](https://github.com/knewit-app/knewit-be/pull/26)).
- `D-260922-3` FE 서비스 계약 → mock 의존 역전 (API 교체 시 화면 수정 없음, [#67](https://github.com/knewit-app/knewit-fe/pull/67)).

**다음 회의까지**

- [ ] @하늘 — 나머지 화면 목업
- [ ] @겨레 — EC2 부트스트랩·compose 스택
- [ ] @지인 — CD/롤백 워크플로

</details>

<!-- 2026-09-24 (목) 추석 연휴. 9/23 ~ 9/28 작업은 9/29 엔트리에 합침 -->

<details>
<summary><b>2026-09-29 (화)</b> · 겨레 · 참석 3/3</summary>

**한 일**

- 🎾 FE · 전 화면 목업 완료(세부 조건·방문 확인·장소 상세·내 장소·내 취향·친구·설정·검색·빈 상태), 저장 목록 매칭 확인 큐. 네이버 지도 SDK, 위치 권한, 딥링크, 공유·길찾기, 앱 잠금, PostHog, EAS. API 연결 1차: 소셜 로그인, 401 재발급, `/me`·동의, 카드 연결(quick-crypto 비밀번호 암호화), 푸시. 브랜치 이름 검사.
- 💎 BE · EC2 compose, CD/롤백 + E2E 검증, Discord 알림. ERD v2(기능명세서 v3.3). 소셜 로그인, 약관, 푸시 토큰, CODEF 카드 연결, 초기·증분 동기화, 탈퇴, 내 장소·저장 API. 상가정보 원장 적재.

**시행착오**

- `T-260929-1` Jib Java 25 미지원 → 3.5.4. SSM AccessDenied → 경로 읽기 권한.
- `T-260929-2` Jest 종료 후 5분 대기(`gcTime` 타이머) → 공용 헬퍼([#116](https://github.com/knewit-app/knewit-fe/pull/116)). MMKV 평문 저장 → `expo-crypto` 키.
- `T-260929-3` 토큰 한쪽만 저장된 채 실패 → 반쪽 세션 → 순차 저장. Android 빌드 지도·카카오 SDK 저장소 누락 → 추가.

**의사결정**

- `D-260929-1` 브랜드 별칭 22종 → 2~3글자 영문 규칙 (HIT 511→520, [#97](https://github.com/knewit-app/knewit-be/pull/97)).
- `D-260929-2` PR 라인 리뷰 → 자체 LiteLLM 봇 / CodeRabbit 라인 리뷰 폐기 (private 유료).
- `D-260929-3` 로그인 → iOS 네이티브 SDK, Android 인가 코드.
- `D-260929-4` FE 기준 명세 → Swagger UI.

**다음 회의까지**

- [ ] @겨레 — 결제→방문 변환 워커, PURGER
- [ ] @지인 — 장소 검색·상세, 방문 확인·추천 API
- [ ] @하늘 — 장소·탈퇴·동기화 API 연동

</details>

<details>
<summary><b>2026-10-01 (목)</b> · 지인 · 참석 3/3</summary>

**한 일**

- 🎾 FE · 카드사 비밀번호 찾기, 앱 실행 시 동기화, 탈퇴, 푸시 on/off, 저장·방문 장소·상세 API 연동(좌표 없는 장소는 길찾기 검색 전환). dev → main 첫 반영, iOS 수출 규정 선언.
- 💎 BE · 장소 검색·상세(카카오 로컬 프록시). 결제→방문 변환 워커([#107](https://github.com/knewit-app/knewit-be/pull/107)), 72시간 만료 결제 삭제(PURGER), 영업 중 부분 인덱스([#112](https://github.com/knewit-app/knewit-be/pull/112)).

**시행착오**

- `T-261001-1` 카드 연결 15초 타임아웃으로 대부분 실패, 거절 동기화 무한 폴링 → `POST /cards`만 150초 + `GET /cards` 복구([#170](https://github.com/knewit-app/knewit-fe/pull/170)).
- `T-261001-2` quick-crypto 팟 산출물이 빌드 fingerprint 흔듦 → 제외. brace-expansion 취약점 → 교체.
- `T-261001-3` jackson-databind CVE로 전 PR CI 실패 → 2.21.7 고정. `gradlew.bat` CRLF → 재정규화.

**의사결정**

- `D-261001-1` 매칭 Kotlin 이식 → PoC와 판정 일치 확인 후 채택 (확정 487 / 확인 40 / 미해소 138).
- `D-261001-2` 확인 요청 기준(후보 50+·0.95 미만) → 유지, 실사용 데이터로 재조정.
- `D-261001-3` 부분 인덱스 채택 (61MB vs 67MB).

**다음 회의까지**

- [ ] @지인 — 방문 확인·첫 방문 요약·추천 API
- [ ] @하늘 — API 연결 2차

</details>

<details>
<summary><b>2026-10-06 (화)</b> · 민지인 · 참석 3/3</summary>

**한 일**

- 🎾 FE · API 연결 2차: 방문 확인 큐·카카오 직접 찾기, 첫 방문 요약, 홈 추천, 내 취향. 인증 가드, 실 API 모드 기본값, orval 8.39.0. EAS Workflows로 main 머지 시 TestFlight/OTA 자동 배포([#235](https://github.com/knewit-app/knewit-fe/pull/235)), Android 빌드 캐시·ABI 축소.
- 💎 BE · 방문 확인, 첫 방문 요약, 추천 3곳(CARD/WATCHING) API. 자동 배포 compose·.env 갱신, 필수 설정 누락 시 기동 차단, 워커 지표·Discord 임베드.

**시행착오**

- `T-261006-1` 추천 항상 빔 → 원장에 없는 `카페`/`음식점` 값으로 분류 → 대분류 `음식`·중분류 `비알코올` 기준([#127](https://github.com/knewit-app/knewit-be/pull/127)).
- `T-261006-2` CODEF 토큰 400 → Java 25 빈 chunked 요청 거부, Sentry 인터셉터가 가림 → form 본문([#136](https://github.com/knewit-app/knewit-be/pull/136)).
- `T-261006-3` 인증 가드 부재로 로그인 우회 → `Stack.Protected`([#194](https://github.com/knewit-app/knewit-fe/pull/194)). 동의 시트 닫히기 전 이동, 진행률 바 미표시 → 수정.

**의사결정**

- `D-261006-1` API 모드 → 목 구현 제거, BE 없는 기능(친구·검색) 숨김 ([#237](https://github.com/knewit-app/knewit-fe/pull/237)).
- `D-261006-2` 패치 없는 취약점 → audit 예외 목록 관리.
- `D-261006-3` 알림 권한 → 카드사 선택 전 안내 시트와 함께 요청. 동기화 찾은 장소 목록 → 플래그로 숨김.

**다음 회의까지**

- [ ] @겨레 — 카카오 장소 ID 일괄 연결, resolve API, 일일 지표 요약

</details>

<details>
<summary><b>2026-10-08 (목)</b> · 겨레 · 참석 3/3</summary>

**한 일**

- 🐈‍⬛ 공통 · 중간 발표.

</details>

<details>
<summary><b>2026-10-13 (화)</b> · 지인 · 참석 3/3</summary>

**한 일**

- 💎 BE · poc-place-attributes v6([#7](https://github.com/knewit-app/poc-place-attributes/pull/7)), v7([#8](https://github.com/knewit-app/poc-place-attributes/pull/8)) 머지, v8 공공데이터 조인 진행 중. knewit-be `place_popularity`·`taste_profile` 배치, 추천 성과 귀속, 초대 API 이슈 생성. 일일 지표 Discord 요약 PR 리뷰 대기.

**시행착오**

- `T-261013-1` 5라운드 연속 게이트 미달 → 5속성 전체 일치율 게이트 문제로 판단 → 속성별 정밀도 재채점, 와이파이 8/8.
- `T-261013-2` 콘센트 오답 2건 → 세브란스 내 지점에 상위시설 글이 붙은 동명 오염 → 미해결.

**의사결정**

- `D-261013-1` 게이트 → 속성별 정밀도 채택 / 전체 field 일치율 폐기.
- `D-261013-2` 콘센트 → 인허가 면적·층 대리 신호 (정밀도 87.0%, 커버리지 31/43), 칩 "오래 앉기 좋은". 브랜드 사전 기각.
- `D-261013-3` 영업시간 → 다음 수집 라운드에서 제외 (정밀도 31.2%).

**다음 회의까지**

- [ ] @겨레 — v8 공공데이터 키 확보 후 재판정, 인허가 원장 서버 적재
- [ ] @지인 — taste_profile 배치, 초대 API

</details>

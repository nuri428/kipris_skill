# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 프로젝트 개요

KIPRIS Plus Open API를 활용한 **한국 지식재산 검색 Claude Code Skill** 저장소. 한국 특허청(KIPRIS)의 52개 서비스(564개 오퍼레이션) API 명세를 문서화하고, `/kipris` 스킬로 실시간 검색을 수행합니다.

## 파일 역할

| 파일 | 역할 |
|------|------|
| `SKILL.md` | 스킬 본체 — 오퍼레이션 매핑, URL 구성, XML 파싱, 실행 워크플로우 |
| `docs/README.md` | API 명세 인덱스 — 52개 서비스 목록, 공통 호출 정보 |
| `docs/services/*.md` | 서비스별 상세 명세 (52개 파일) — 오퍼레이션별 IN/OUT 파라미터 |
| `CLAUDE.md` | 이 파일 — 프로젝트 컨텍스트 |

## API 아키텍처

### 두 가지 게이트웨이

| 게이트웨이 | URL 패턴 | 인증 키 |
|-----------|---------|---------|
| OpenAPI (패턴 A) | `http://plus.kipris.or.kr/openapi/rest/{ServicePath}/{operation}` | `accessKey` (KIPRIS Plus 발급) |
| KIPO API (패턴 B) | `http://plus.kipris.or.kr/kipo-api/kipi/{ServicePath}/{operation}` | `ServiceKey` (공공데이터 포털 발급) |

동일 서비스라도 오퍼레이션에 따라 게이트웨이가 다를 수 있음. 각 오퍼레이션 문서의 Endpoint를 반드시 확인할 것.

### 응답 형식

- XML 응답 → JSON 변환 후 파싱
- 응답 데이터 루트 키가 오퍼레이션마다 다름 (예: `response.body.items.PatentUtilityInfo` vs `response.body.items.item`)

### 확인된 서비스 경로

| 서비스 | ServicePath | 상태 |
|--------|-------------|------|
| 특허·실용 공개·등록공보 | `patUtiModInfoSearchSevice` | 검증됨 |
| 해외특허 | `ForeignPatentAdvencedSearchService` | 검증됨 |
| 디자인 공보 | `designInfoSearchService` | 미검증 |
| 상표 출원 속보 | `trademarkInfoSearchService` | 미검증 |
| 특허 패밀리 | `patFamInfoSearchService` | 미검증 |
| 특허·실용 인용문헌 | `CitationService` | 미검증 |
| 특허·실용 피인용문헌 | `CitingService` | 미검증 |
| 출원인 법인 | `CorpBsApplicantService` | 미검증 |
| 의견제출통지서 | `IntermediateDocumentOPService` | 미검증 |
| 거절결정서 | `IntermediateDocumentREService` | 미검증 |
| 상표 분류코드 | `TradeMarkClassificationInfoService` | 미검증 |

> "미검증" 경로는 GitHub 공개 코드에서 추출. API 키로 실제 호출 검증 필요.
> 나머지 38개 서비스의 ServicePath는 KIPRIS Plus 포털에서 개별 확인 필요.

## 구현 현황

12개 오퍼레이션이 Tier 1으로 즉시 사용 가능 (SKILL.md 참조):
- **특허·실용 (7개)**: `getAdvancedSearch`, `freeSearchInfo`, `applicationNumberSearchInfo`, `applicantNameSearchInfo`, `rightHolerSearchInfo`, `getBibliographyDetailInfoSearch`, `getBibliographySumryInfoSearch`
- **해외특허 (5개)**: `freeSearch`, `applicationNumberSearch`, `internationalOpenNumberSearch`, `applicantSearch`, `internationalApplicationNumberSearch`

나머지 552개 오퍼레이션은 `docs/services/` 문서를 참조하여 동적으로 호출 가능.

## 환경 변수

- `KIPRIS_API_KEY` — API 인증 키

## 스킬 설치

설치 방법은 `README.md`를 참조하세요.

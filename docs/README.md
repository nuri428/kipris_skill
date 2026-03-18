# KIPRIS Plus Open API 명세 인덱스

> Excel 원본: `docs/KIPRISPlus Open API 입출력값 정보.xlsx`에서 자동 생성
> 생성일: 2026-03-18

## 공통 API 호출 정보

### 인증

모든 API 호출 시 쿼리 파라미터로 API 키를 전달합니다. 키 필드명은 게이트웨이에 따라 다릅니다:

| 게이트웨이 | 키 파라미터 | 발급처 |
|-----------|-----------|--------|
| OpenAPI (`/openapi/rest/`) | `accessKey` | [KIPRIS Plus](https://plus.kipris.or.kr) 회원가입 후 발급 |
| KIPO API (`/kipo-api/kipi/`) | `ServiceKey` | [공공데이터 포털](https://www.data.go.kr) 활용 신청 후 발급 |

> **주의**: API 키는 절대 소스코드/문서에 하드코딩하지 마세요. 환경변수(`KIPRIS_API_KEY`)로 관리하세요.

### URL 패턴

KIPRIS API는 두 가지 게이트웨이를 사용합니다:

```
# 패턴 A — KIPRIS OpenAPI 게이트웨이
http://plus.kipris.or.kr/openapi/rest/{ServicePath}/{operationName}?accessKey={API_KEY}&param1=value1

# 패턴 B — 공공데이터 포털 연계 (KIPO API)
http://plus.kipris.or.kr/kipo-api/kipi/{ServicePath}/{operationName}?ServiceKey={API_KEY}&param1=value1
```

### 서비스 경로 매핑

#### 확인된 경로 (실제 구현/테스트 완료)

| 서비스명 | ServicePath | 게이트웨이 |
|---------|-------------|-----------|
| 특허·실용 공개·등록공보 | `patUtiModInfoSearchSevice` | A + B (오퍼레이션별 상이) |
| 해외특허 | `ForeignPatentAdvencedSearchService` | A |

#### GitHub 코드 검색으로 확인된 경로 (미검증)

| 서비스명 (추정) | ServicePath | 게이트웨이 (추정) |
|---------------|-------------|-----------------|
| 디자인 공보 | `designInfoSearchService` | A + B |
| 상표 출원 속보 | `trademarkInfoSearchService` | A + B |
| 특허 패밀리 | `patFamInfoSearchService` | B |
| 특허·실용 인용문헌 | `CitationService` | A |
| 특허·실용 피인용문헌 | `CitingService` | A |
| 출원인 법인 | `CorpBsApplicantService` | A |
| 의견제출통지서 | `IntermediateDocumentOPService` | A |
| 거절결정서/등록결정서 | `IntermediateDocumentREService` | A |
| 특허 관련 문서 | `RelatedDocsonfilePatService` | A |
| 상표 관련 문서 | `RelatedDocsonfileTMService` | A |
| 상표 분류코드 | `TradeMarkClassificationInfoService` | A |
| (미확인) | `PatentSearchService` | A |

> **주의**: "미검증" 경로는 GitHub 공개 코드에서 추출한 것으로, API 키로 실제 호출 검증이 필요합니다.
> 나머지 38개 서비스의 ServicePath는 KIPRIS Plus 포털의 [API 활용 가이드(PDF)](https://plus.kipris.or.kr/portal/bbs/view.do?nttId=638&bbsId=B0000001&menuNo=210149)에서 확인 가능합니다.

### 응답 형식

- **응답 포맷**: XML (내부적으로 JSON 변환 후 파싱)
- **데이터 위치**: 응답 XML 내 중첩 경로로 접근 (오퍼레이션별 상이)
- **공통 구조**:

```xml
<response>
  <header>
    <resultCode>00</resultCode>
    <resultMsg>NORMAL SERVICE</resultMsg>
  </header>
  <body>
    <items>
      <PatentUtilityInfo>...</PatentUtilityInfo>  <!-- 또는 item, searchResult 등 -->
    </items>
  </body>
</response>
```

### 응답 데이터 루트 키 (확인된 것)

| 서비스 / 오퍼레이션 | 응답 루트 키 |
|-------------------|------------|
| 특허·실용 / 자유검색, 출원번호검색, 출원인정보, 등록권자정보 | `response.body.items.PatentUtilityInfo` |
| 특허·실용 / 전체검색, 서지요약정보 | `response.body.items.item` |
| 특허·실용 / 서지상세정보 | `response.body.item` |
| 해외특허 / 전체 | `response.body.items.searchResult` |

### curl 호출 예시

```bash
# 특허·실용 자유검색 (OpenAPI 게이트웨이)
curl "http://plus.kipris.or.kr/openapi/rest/patUtiModInfoSearchSevice/freeSearchInfo?accessKey=${KIPRIS_API_KEY}&word=인공지능&patent=true&utility=true"

# 특허·실용 전체검색 (KIPO API 게이트웨이)
curl "http://plus.kipris.or.kr/kipo-api/kipi/patUtiModInfoSearchSevice/getAdvancedSearch?ServiceKey=${KIPRIS_API_KEY}&word=인공지능&patent=true&utility=true&numOfRows=10&pageNo=1"

# 해외특허 자유검색 (OpenAPI 게이트웨이)
curl "http://plus.kipris.or.kr/openapi/rest/ForeignPatentAdvencedSearchService/freeSearch?accessKey=${KIPRIS_API_KEY}&free=artificial+intelligence&collectionValues=US"
```

## 전체 현황

| 항목 | 수치 |
|------|------|
| 서비스 수 | 52개 |
| 전체 오퍼레이션 | 564개 |
| 구현 완료 | 12개 (2.1%) |
| 폐기예정 | 30개 |
| 미구현 (활성) | 522개 |

## 서비스 목록

| # | 서비스명 | 오퍼레이션 | 구현 | 상세 |
|---|---------|-----------|------|------|
| 1 | 특허·실용 공개·등록공보 | 61개 | ✅ 7/61 | [상세](services/patent_utility.md) |
| 2 | 특허·실용 인용문헌 | 5개 | ❌ 0/5 | [상세](services/patent_citation.md) |
| 3 | 특허·실용 행정처리 이력 | 3개 | ❌ 0/3 | [상세](services/patent_admin_history.md) |
| 4 | 특허·실용 분류코드 변동 이력 | 3개 | ❌ 0/3 | [상세](services/patent_classification_history.md) |
| 5 | 디자인 공보 | 51개 | ❌ 0/51 | [상세](services/design.md) |
| 6 | 디자인 행정처리 이력 | 2개 | ❌ 0/2 | [상세](services/design_admin_history.md) |
| 7 | 상표 행정처리 이력 | 2개 | ❌ 0/2 | [상세](services/trademark_admin_history.md) |
| 8 | 상표 출원 속보 | 54개 | ❌ 0/54 | [상세](services/trademark.md) |
| 9 | 법적 상태 이력 | 5개 | ❌ 0/5 | [상세](services/legal_status.md) |
| 10 | 특허·실용 통지서 마감기한 | 6개 | ❌ 0/6 | [상세](services/patent_notice_deadline.md) |
| 11 | 등록사항 | 12개 | ❌ 0/12 | [상세](services/registration.md) |
| 12 | 권리자 변동 이력 | 3개 | ❌ 0/3 | [상세](services/right_holder_history.md) |
| 13 | 분류코드 | 8개 | ❌ 0/8 | [상세](services/classification_code.md) |
| 14 | 심판사항 | 31개 | ❌ 0/31 | [상세](services/trial.md) |
| 15 | 대표 출원인 | 4개 | ❌ 0/4 | [상세](services/representative_applicant.md) |
| 16 | 시소러스 | 2개 | ❌ 0/2 | [상세](services/thesaurus.md) |
| 17 | 한국특허영문초록(KPA) | 26개 | ❌ 0/26 | [상세](services/kpa_english_abstract.md) |
| 18 | 기계번역용 국문초록 | 1개 | ❌ 0/1 | [상세](services/machine_translation_abstract.md) |
| 19 | 해외특허 | 81개 | ✅ 5/81 | [상세](services/foreign_patent.md) |
| 20 | 공통 | 10개 | ❌ 0/10 | [상세](services/common.md) |
| 21 | 특허 패밀리 | 5개 | ❌ 0/5 | [상세](services/patent_family.md) |
| 22 | 다인용 선행문헌 | 2개 | ❌ 0/2 | [상세](services/multi_citation.md) |
| 23 | 국유특허 | 2개 | ❌ 0/2 | [상세](services/government_patent.md) |
| 24 | 특허 기탁 미생물 | 4개 | ❌ 0/4 | [상세](services/patent_microorganism.md) |
| 25 | 인터넷 기술공지 | 2개 | ❌ 0/2 | [상세](services/internet_tech_notice.md) |
| 26 | 공모전 아이디어 | 1개 | ❌ 0/1 | [상세](services/contest_idea.md) |
| 27 | IP-Biz 하나로 서비스 기술분류 | 1개 | ❌ 0/1 | [상세](services/ipbiz_hanaro.md) |
| 28 | 디자인맵 형태분류 | 2개 | ❌ 0/2 | [상세](services/design_map.md) |
| 29 | 의견제출통지서 | 12개 | ❌ 0/12 | [상세](services/opinion_notice.md) |
| 30 | 거절결정서 | 12개 | ❌ 0/12 | [상세](services/rejection_decision.md) |
| 31 | 정정공보 | 24개 | ❌ 0/24 | [상세](services/amendment_gazette.md) |
| 32 | 출원인 법인 | 5개 | ❌ 0/5 | [상세](services/applicant_corporation.md) |
| 33 | 디자인 분류코드 변동 이력 | 3개 | ❌ 0/3 | [상세](services/design_classification_history.md) |
| 34 | 상표 분류코드 변동 이력 | 2개 | ❌ 0/2 | [상세](services/trademark_classification_history.md) |
| 35 | 해외디자인 | 31개 | ❌ 0/31 | [상세](services/foreign_design.md) |
| 36 | 해외상표 | 22개 | ❌ 0/22 | [상세](services/foreign_trademark.md) |
| 37 | 출원인 명칭 변동 이력 | 3개 | ❌ 0/3 | [상세](services/applicant_name_history.md) |
| 38 | 출원인 기술분야 | 2개 | ❌ 0/2 | [상세](services/applicant_tech_field.md) |
| 39 | 등록결정서 | 9개 | ❌ 0/9 | [상세](services/registration_decision.md) |
| 40 | 청구항 변동 이력 | 3개 | ❌ 0/3 | [상세](services/claim_history.md) |
| 41 | 특허 염기서열 | 7개 | ❌ 0/7 | [상세](services/patent_sequence.md) |
| 42 | 특허 합금조성비 | 2개 | ❌ 0/2 | [상세](services/patent_alloy.md) |
| 43 | TM5 공통상태 지표 | 2개 | ❌ 0/2 | [상세](services/tm5_indicator.md) |
| 44 | 특허·실용 피인용문헌 | 3개 | ❌ 0/3 | [상세](services/patent_cited.md) |
| 45 | 특허권 존속기간 연장등록 공보 | 4개 | ❌ 0/4 | [상세](services/patent_extension.md) |
| 46 | 의약품 국제일반명칭 | 3개 | ❌ 0/3 | [상세](services/inn_medicine.md) |
| 47 | 상표 원산지 명칭 | 3개 | ❌ 0/3 | [상세](services/trademark_origin.md) |
| 48 | 품종보호권 등록 식물 명칭 | 3개 | ❌ 0/3 | [상세](services/variety_protection.md) |
| 49 | 일본 특허 합금조성비 | 5개 | ❌ 0/5 | [상세](services/japan_patent_alloy.md) |
| 50 | 특허 중한 코퍼스 | 1개 | ❌ 0/1 | [상세](services/patent_cn_kr_corpus.md) |
| 51 | 특허·실용 권리자 변동 이력 | 5개 | ❌ 0/5 | [상세](services/patent_right_transfer.md) |
| 52 | 특허·실용 법적 상태 이력(ST.27) | 9개 | ❌ 0/9 | [상세](services/patent_legal_status_st27.md) |

## 구현된 오퍼레이션 요약

| 서비스 | 오퍼레이션 | 영문명 | 구현 클래스 |
|--------|-----------|--------|-----------|
| 특허·실용 공개·등록공보 | 전체검색 | `getAdvancedSearch` | `KoreanPatentSearchTool` |
| 특허·실용 공개·등록공보 | 자유검색 | `freeSearchInfo` | `KoreanPatentFreeSearchTool` |
| 특허·실용 공개·등록공보 | 출원번호 검색 | `applicationNumberSearchInfo` | `KoreanPatentApplicationNumberSearchTool` |
| 특허·실용 공개·등록공보 | 출원인정보 | `applicantNameSearchInfo` | `KoreanPatentApplicantSearchTool` |
| 특허·실용 공개·등록공보 | 등록권자정보 | `rightHolerSearchInfo` | `KoreanPatentRighterSearchTool` |
| 특허·실용 공개·등록공보 | 서지상세정보(공공데이터 포털 연계) | `getBibliographyDetailInfoSearch` | `KoreanPatentDetailSearchTool` |
| 특허·실용 공개·등록공보 | 서지요약정보 | `getBibliographySumryInfoSearch` | `KoreanPatentSummarySearchTool` |
| 해외특허 | 자유검색 | `freeSearch` | `ForeignPatentFreeSearchTool` |
| 해외특허 | 출원번호 | `applicationNumberSearch` | `ForeignPatentApplicationNumberSearchTool` |
| 해외특허 | 국제공개번호 | `internationalOpenNumberSearch` | `ForeignPatentInternationalOpenNumberSearchTool` |
| 해외특허 | 출원인 | `applicantSearch` | `ForeignPatentApplicantSearchTool` |
| 해외특허 | 국제출원번호 | `internationalApplicationNumberSearch` | `ForeignPatentInternationalApplicationNumberSearchTool` |

## 디렉토리 구조

```
docs/api_spec/
├── README.md              # 이 파일 (인덱스)
└── services/              # 서비스별 상세 명세
    ├── patent_utility.md
    ├── patent_citation.md
    ├── patent_admin_history.md
    ├── patent_classification_history.md
    ├── design.md
    ├── design_admin_history.md
    ├── trademark_admin_history.md
    ├── trademark.md
    ├── legal_status.md
    ├── patent_notice_deadline.md
    ├── registration.md
    ├── right_holder_history.md
    ├── classification_code.md
    ├── trial.md
    ├── representative_applicant.md
    ├── thesaurus.md
    ├── kpa_english_abstract.md
    ├── machine_translation_abstract.md
    ├── foreign_patent.md
    ├── common.md
    ├── patent_family.md
    ├── multi_citation.md
    ├── government_patent.md
    ├── patent_microorganism.md
    ├── internet_tech_notice.md
    ├── contest_idea.md
    ├── ipbiz_hanaro.md
    ├── design_map.md
    ├── opinion_notice.md
    ├── rejection_decision.md
    ├── amendment_gazette.md
    ├── applicant_corporation.md
    ├── design_classification_history.md
    ├── trademark_classification_history.md
    ├── foreign_design.md
    ├── foreign_trademark.md
    ├── applicant_name_history.md
    ├── applicant_tech_field.md
    ├── registration_decision.md
    ├── claim_history.md
    ├── patent_sequence.md
    ├── patent_alloy.md
    ├── tm5_indicator.md
    ├── patent_cited.md
    ├── patent_extension.md
    ├── inn_medicine.md
    ├── trademark_origin.md
    ├── variety_protection.md
    ├── japan_patent_alloy.md
    ├── patent_cn_kr_corpus.md
    ├── patent_right_transfer.md
    ├── patent_legal_status_st27.md
```
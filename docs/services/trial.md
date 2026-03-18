# 심판사항

- **API 유형**: REST
- **오퍼레이션 수**: 31개 (구현: 0, 폐기예정: 2)

---

## 단어(폐기예정)
`getWordSearch`

- **분류**: 일반검색
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchString` | 검색어 |  |
| `searchYear` | 검색년도범위 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |
| `count` |  |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 번호(폐기예정)
`getNumberSearch`

- **분류**: 일반검색
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchJudhment` | 심판분류 | (100 0=전체) |
| `searchNumber` | 검색번호 |  |
| `searchYear` | 검색년도범위 | (2009 0=전체) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `item` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `defendant` | 피청구인 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `plaintiff` | 청구인 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `trialDesc` | 심판종류 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialNumber` | 심판번호 |  |
| `trialStatus` | 심판상태 |  |
| `count` |  |  |
| `numOfRows` |  |  |
| `pageNo` | 페이지번호 | (검색 페이지 번호) |
| `totalCount` | 전체건수 |  |

---

## 전체검색
`getAdvancedSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `free` | 검색어 |  |
| `trialDesc` | 심판종류 | (JM) |
| `trialNumber` | 심판번호 | (JG) |
| `trialNumberNm` | 심판번호문자 | (JC) |
| `registerNumber` | 등록번호 | (RN) |
| `applicationNumber` | 출원번호/국제등록번호 | (AN) |
| `trialRequestDate` | 심판청구일자 | (RD) |
| `trialDate` | 심결일자 | (DD) |
| `plaintiff` | 청구인 | (DP) |
| `plaintiffAgent` | 청구대리인 | (DG) |
| `defendant` | 피청구인 | (PP) |
| `defendantAgent` | 피청구대리인 | (PG) |
| `eventindication` | 사건의표시 | (EI) |
| `title` | 발명의명칭/물품명칭/상표명칭 | (IT) |
| `patent` | 특허 | (포함 : true, 미포함 : false) |
| `practical` | 실용 | (포함 : true, 미포함 : false) |
| `design` | 디자인 | (포함 : true, 미포함 : false) |
| `tradeMark` | 상표 | (포함 : true, 미포함 : false) |
| `patentTrial` | 특허심판원 | (포함 : true, 미포함 : false) |
| `patentCourt` | 특허법원 | (포함 : true, 미포함 : false) |
| `supremeCourt` | 대법원 | (포함 : true, 미포함 : false) |
| `summaryCourt` | 심판소 | (포함 : true, 미포함 : false) |
| `appealCourt` | 항고심판소 | (포함 : true, 미포함 : false) |
| `exParte` | 결정계 | (포함 : true, 미포함 : false) |
| `interParties` | 당사자계 | (포함 : true, 미포함 : false) |
| `pageNo` | 페이지번호 |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Items` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 심결일자
`trialdecisionDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialDate` | 심결일자 |  |
| `patentTrial` | 특허심판원 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `patentCourt` | 특허법원 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `supremeCourt` | 대법원 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `summaryCourt` | 심판소 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `appealCourt` | 항고심판소 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `exParte` | 결정계 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `interParties` | 당사자계 | (포함 : true, 미포함 : false)?※기본값(default) : true |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 | (JG:심판번호, JM:심판종류, DP:청구인, IT:발명명칭, AN:출원번호, RN:등록번호, PP:피청구인)?※기본값(default) : JG |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Items` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 자유검색
`freeSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `free` | 검색어 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 심판종류
`trialDescSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialKind` | 심판종류 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 심판번호숫자
`trialNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 | (숫자) |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 심판번호문자
`trialNumberNmSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumberNm` | 심판번호문자 | (문자) |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 등록번호
`registerNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registerNumber` | 등록번호 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 출원(국제등록)번호
`applicationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 심판청구일자
`trialRequestDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialRequestDate` | 심판청구일자 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 청구인
`plaintiffSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `plaintiff` | 청구인 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 청구대리인
`plaintiffAgentSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `plaintiffAgent` | 청구대리인 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 피청구인
`defendantSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `defendant` | 피청구인 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 피청구대리인
`defendantAgentSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `defendantAgent` | 피청구대리인 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 사건의 표시
`eventindicationSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `eventindication` | 사건의표시 |  |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 명칭
`titleSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `title` | 발명의명칭/물품명칭/상표명칭 | (IT) |
| `appealCourt` | 항고심판소 |  |
| `patentCourt` | 특허법원 |  |
| `patentTrial` | 특허심판원 |  |
| `summaryCourt` | 심판소 |  |
| `supremeCourt` | 대법원 |  |
| `exParte` | 결정계 |  |
| `interParties` | 당사자계 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TrialInfo` |  |  |
| `trialNumber` | 심판번호 |  |
| `trialFlag` | 심판구분 | 심급구분 |
| `trialDesc` | 심판종류 |  |
| `trialStatus` | 심판상태 |  |
| `plaintiff` | 청구인 |  |
| `title` | 발명의명칭/물품명칭/상표명칭 |  |
| `trialDecisionDoc` | 심(판)결문 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `registrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `InternationalRegisterNumber` | 국제등록번호 |  |
| `defendant` | 피청구인 |  |

---

## 서지상세정보
`getBibliographyDetailInfoSearch`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `bibliographicSummaryInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `appealFg` | 상고여부 |  |
| `applicationNumber` | 출원번호 |  |
| `buCd` | 심판부코드 |  |
| `cdDesc` | 심판종류 |  |
| `conclusiveDate` | 심판확정일자 |  |
| `conclusiveResultCode` | 심판확정결과 |  |
| `conclusiveStatusCode` | 심판확정상태 |  |
| `conclusiveTrialDivision` | 확정심결주문내용 |  |
| `eventindication` | 사건의표시 |  |
| `evtNo` | 사건번호 |  |
| `instanceDivision` | 심판구분 | 심급구분 |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `inventionTitle` | 발명의명칭/물품명칭/상표명칭 |  |
| `offcAppealFg` | 청상고여부 |  |
| `oppositionDate` | 병합일자 |  |
| `oppositionTrialNumber` | 병합심판번호 |  |
| `originalTrialNumber` | 원심판번호 |  |
| `path` | 파일경로 |  |
| `regReferenceNumber/` | 등록참조번호 |  |
| `registerNumber` | 등록번호 |  |
| `rightDivisionCode` | 권리종류 |  |
| `trialDecision` | 심결주문내용 |  |
| `trialDecisionCode` | 심결주문 |  |
| `trialDecisionDate` | 심결일자 |  |
| `trialFlag` |  | ※해당 데이터 사용금지 |
| `trialNumber` | 심판번호 |  |
| `trialNumberNm` | 심판문자번호 |  |
| `trialRequestCount` | 심판청구항수 |  |
| `trialRequestDate` | 심판청구일자 |  |
| `trialRequestPurpose` | 청구의취지 |  |
| `trialStatusCode` | 심판상태 |  |
| `claimAgentTypeArray` |  |  |
| `claimAgentType` |  |  |
| `address` | 청구대리인주소 |  |
| `agentCode` | 청구대리인번호 |  |
| `country` | 청구대리인국가 |  |
| `name` | 청구대리인명 |  |
| `claimTypeArray` |  |  |
| `claimType` |  |  |
| `address` | 청구인주소 |  |
| `country` | 청구인국가 |  |
| `name` | 청구인명 |  |
| `defendantAgentTypeArray` |  |  |
| `defendantAgentType` |  |  |
| `address` | 피청구대리인주소 |  |
| `agentCode` | 피청구대리인번호 |  |
| `country` | 피청구대리인국가 |  |
| `name` | 피청구대리인명 |  |
| `defendantTypeArray` |  |  |
| `defendantType` |  |  |
| `address` | 피청구인주소 |  |
| `country` | 피청구인국가 |  |
| `name` | 피청구인명 |  |
| `legalStatusInfoArray` |  |  |
| `legalStatusInfos` |  |  |
| `documentsNumber` | 접수서류명/발송서류명 |  |
| `receiptDate` | 접수일자/발송일자 |  |
| `receiptNumber` | 접수번호/발송번호 |  |
| `status` | 서류처리상태 |  |
| `relatedTrialNumberArray` |  |  |
| `relatedTrialNumber` |  |  |
| `trialNumber` | 심판번호 |  |
| `specifyCtegoryCodeInfoArray` |  |  |
| `specifyCtegoryCodeInfo` |  |  |
| `clssCd` | 지정분류코드 |  |
| `specifyCtegoryCodeInfoArray` |  |  |
| `supplementaryDecisionInfo` | 파일경로 |  |

---

## 서지요약정보
`trialBibliographicSummaryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `TrialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialBibliographicSummaryInfo` |  |  |
| `TrialNumber` | 심판번호 |  |
| `TrialTypeCodeName` | 심판종류 |  |
| `RightTypeCodeName` | 권리종류 |  |
| `TrialStatusCodeName` | 심판상태 |  |
| `EventIndicationContent` | 사건의표시 |  |
| `TrialDemandDate` | 심판청구일자 |  |
| `TrialSubCode` | 심판부코드 |  |
| `DemandObject` | 청구의취지 |  |
| `TrialdecisionPrincipleclauseCodeName` | 심결주문 |  |
| `TrialdecisionDate` | 심결일자 |  |
| `TrialConfirmationStatusCodeName` | 심판확정상태 |  |
| `TrialConfirmationDate` | 심판확정일자 |  |
| `ConfirmationResultCodeName` | 심판확정결과 |  |
| `ApplicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `Titleofinvention` | 발명의명칭/물품명칭/상표명칭 |  |
| `OriginalTrialNumber` | 원심판번호 |  |
| `EventNumber` | 사건번호 |  |
| `AppealtothesupremecourtYesorno` | 상고여부 |  |
| `OfficeAppealtothesupremecourtYesorno` | 청상고여부 |  |
| `TrialdecisionPrincipleclauseContent` | 심결주문내용 |  |
| `ConfirmationTrialdecisionPrincipleclauseContent` | 확정심결주문내용 |  |
| `AnnexationTrialNumber` | 병합심판번호 |  |
| `AnnexationDate` | 병합일자 |  |
| `TrialNumberName` | 심판번호문자 |  |
| `TrialgradeType` | 심판구분 | 심급구분 |
| `TotalPetitionclauseCount` | 총청구항수 |  |
| `InternationalRegistrationNumber` | 국제등록번호 |  |
| `TrialcourtdecisionFilePath` | 파일경로 |  |

---

## 심판이력사항
`trialHistoryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `TrialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialHistoryInfo` |  |  |
| `ReceiptSendNumber` | 접수번호/발송번호 |  |
| `ReceiptSendDocumentName` | 접수서류명/발송서류명 |  |
| `ReceiptSendDate` | 접수일자/발송일자 |  |
| `ProcessStatusCodeName` | 서류처리상태 |  |

---

## 관련심판번호
`trialRelatedTrialNumberInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialRelatedTrialNumberInfo` |  |  |
| `trialNumber` | 심판번호 |  |

---

## 지정분류코드
`trialSpecifyCtegoryCodeInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialSpecifyCtegoryCodeInfo` |  |  |
| `clssCd` | 지정분류코드 |  |

---

## 청구인
`trialPlaintiffInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialPlaintiffInfo` |  |  |
| `name` | 청구인명 |  |
| `address` | 청구인주소 |  |
| `country` | 청구인국가 |  |

---

## 청구대리인
`trialPlaintiffAgentInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialPlaintiffAgentInfo` |  |  |
| `name` | 청구대리인명 |  |
| `address` | 청구대리인주소 |  |
| `country` | 청구대리인국가 |  |
| `agentCode` | 청구대리인번호 |  |

---

## 피청구인
`trialDefendantInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialDefendantInfo` |  |  |
| `name` | 피청구인명 |  |
| `address` | 피청구인주소 |  |
| `country` | 피청구인국가 |  |

---

## 피청구대리인
`trialDefendantAgentInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialDefendantAgentInfo` |  |  |
| `name` | 피청구대리인명 |  |
| `address` | 피청구대리인주소 |  |
| `country` | 피청구대리인국가 |  |
| `agentCode` | 피청구대리인번호 |  |

---

## 변동정보
`getChangeInfoSearch`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `date` | 변동일자 |  |

---

## 변동정보2
`trialTransferInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | (BIB-서지, ADM-심판이력, DP-청구인/피청구인, PP-청구대리인/피청구대리인, TDC-심판결문, TDCDEL-심판결문삭제) |
| `transferDate` | 변동일자 | ※입력방식(ex : 20160713) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialTransferInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 심판번호리스트 | (ex : 심판번호1&#124;심판번호2) |

---

## 심판(결)문
`getJudDocumentInfoSearch`

- **분류**: 심판(결)문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Item` |  |  |
| `path` | 파일경로 |  |
| `fileName` | 파일명 |  |
| `kind` | 파일종류 |  |
| `openYN` | 공개여부 |  |

---

## 경정결정문
`trialSupplementaryDecisionInfo`

- **분류**: 심판(결)문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialSupplementaryDecisionInfo` |  |  |
| `path` | 파일경로 |  |
| `fileName` | 파일명 |  |
| `kind` | 파일종류 |  |

---

## 모든 전문 유무
`trialFullTextCheckInfo`

- **분류**: 심판(결)문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trialFullTextCheckInfo` |  |  |
| `judgmentDocumentCheckResult` | 심판결문유무 | (있음:Y, 없음:N) |
| `supplementaryDecisionCheckResult` | 경정결정문유무 | (있음:Y, 없음:N) |

---

# 특허·실용 통지서 마감기한

- **API 유형**: REST
- **오퍼레이션 수**: 6개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `DueDateService` (포털 확인)
- **게이트웨이**: OpenAPI (`/openapi/rest/`)
- **인증 키**: `accessKey`

---

## 출원통지서기한정보(출원번호)
`dueDateApplicationNoticeApplnoInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dueDateApplicationNoticeApplnoInfoList` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `Mailingnumber` | 발송번호 |  |
| `DocNm` | 문서명칭 |  |
| `ExpirationDuedateDate` | 마감기한일자 |  |

---

## 출원통지서기한정보(발생원인발송번호)
`dueDateApplicationNoticeMlnoInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `mailingnumber` | 발송번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dueDateApplicationNoticeMlnoInfoList` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `Mailingnumber` | 발송번호 |  |
| `DocNm` | 문서명칭 |  |
| `ExpirationDuedateDate` | 마감기한일자 |  |

---

## 등록통지서기한정보(등록번호)
`dueDateRegistratioNoticeRgstnoInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dueDateRegistratioNoticeRgstnoInfoList` |  |  |
| `Mailingnumber` | 발송번호 |  |
| `DocNm` | 문서명칭 |  |
| `ExpirationDuedateDate` | 마감기한일자 |  |

---

## 심판통지서기한정보(심판번호)
`dueDateTrialNoticeTrlnoInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dueDateTrialNoticeTrlnoInfoList` |  |  |
| `TrialNumber` | 심판번호 |  |
| `Mailingnumber` | 발송번호 |  |
| `DocNm` | 문서명칭 |  |
| `ExpirationDuedateDate` | 마감기한일자 |  |

---

## 심판통지서기한정보(발생원인발송번호)
`dueDateTrialNoticeMlnoInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trialNumber` | 심판번호 |  |
| `mailingnumber` | 발송번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dueDateTrialNoticeMlnoInfoList` |  |  |
| `TrialNumber` | 심판번호 |  |
| `Mailingnumber` | 발송번호 |  |
| `DocNm` | 문서명칭 |  |
| `ExpirationDuedateDate` | 마감기한일자 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | AP-출원통지서기한정보, RG-등록통지서기한정보, TR-심판통지서기한정보 |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : [AP]출원번호(발송번호)1&#124;출원번호(발송번호)2, [RG]등록번호1&#124;등록번호2, [TR]심판번호(발송번호)&#124;심판번호(발송번호)) |

---

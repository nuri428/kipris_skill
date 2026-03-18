# 특허·실용 인용문헌

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `CitationService` (포털 확인)
- **게이트웨이**: OpenAPI (`/openapi/rest/`)
- **인증 키**: `accessKey`

---

## 인용문헌V2(폐기 예정)
`citationInfoV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `citationInfoV2` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `CitationLiteratureTypeSerialnumber` | 인용문헌구분일련번호 |  |
| `CitationLiteratureTypeCode` | 인용문헌구분코드 |  |
| `StandardCitationLiteratureNumber` | 표준인용문헌번호 |  |
| `StandardCitationLiteratureCountryCode` | 표준인용문헌국가코드 |  |
| `StandardCitationLiteratureIdentificationCode` | 표준인용문헌식별코드 |  |
| `StandardCitationLiteraturePublicationDate` | 표준인용문헌발행일자 |  |
| `StandardProcessStatusCode` | 표준처리상태코드 |  |

---

## 인용문헌(폐기 예정)
`citationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `citationInfoV2` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `CitationLiteratureTypeSerialnumber` | 인용문헌구분일련번호 |  |
| `CitationLiteratureTypeCode` | 인용문헌구분코드 |  |
| `StandardCitationLiteratureNumber` | 표준인용문헌번호 |  |
| `StandardCitationLiteratureCountryCode` | 표준인용문헌국가코드 |  |
| `StandardCitationLiteratureIdentificationCode` | 표준인용문헌식별코드 |  |
| `StandardCitationLiteraturePublicationDate` | 표준인용문헌발행일자 |  |
| `StandardProcessStatusCode` | 표준처리상태코드 |  |

---

## 인용문헌V3
`citationInfoV3`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `citationInfoV3` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `OriginalcitationLiteraturenumber` | 원인용문헌번호 |  |
| `OriginalcitationLiteraturenumberDate` | 원인용문헌번호일자 |  |
| `StandardCitationLiteraturenumber` | 표준인용문헌번호 |  |
| `StandardCitationLiteratureCountryCode` | 표준인용문헌국가코드 |  |
| `StandardCitationLiteratureCountryCodeName` | 표준인용문헌국가코드명 |  |
| `StandardCitationIdentificationCode` | 표준인용식별코드 |  |
| `StandardCitationLiteraturePublicationDate` | 표준인용문헌발행일자 |  |
| `StandardStatusCode` | 표준상태코드 |  |
| `StandardStatusCodeName` | 표준상태코드명 |  |
| `CitationLiteratureTypeCode` | 인용문헌구분코드 |  |
| `CitationLiteratureTypeCodeName` | 인용문헌구분코드명 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

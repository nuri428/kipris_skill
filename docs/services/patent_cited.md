# 특허·실용 피인용문헌

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `CitingService` ⚠️ 미검증
- **게이트웨이**: OpenAPI (`/openapi/rest/`) (추정)

---

## 피인용문헌
`citingInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `standardCitationApplicationNumber` | 출원번호 | (선행기술) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `citingInfo` |  |  |
| `StandardCitationApplicationNumber` | 출원번호 | (선행기술) |
| `ApplicationNumber` | 출원번호 | (피인용문헌, 후행기술) |
| `StandardStatusCode` | 표준화처리상태코드 | (20001-표준화, 20002-비특허문헌) |
| `StandardStatusCodeName` | 표준화처리상태코드 | (20001-표준화, 20002-비특허문헌) |
| `CitationLiteratureTypeCode` | 인용문헌구분코드 | (E0801-발송문서, E0802-선행기술조사보고서, E0805-선행기술조사문헌, E0806-출원서인용문헌이력정보) |
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
| `standardCitationApplicationNumber` | 출원번호 | (선행기술) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

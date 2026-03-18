# 출원인 명칭 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 기본정보
`applicantBasicInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `patentCustomerNumber` | 특허고객번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantBasicInfo` |  |  |
| `patentCustomerNumber` | 특허고객번호 |  |
| `patentCustomerRegistrationDate` | 특허고객등록일자 |  |
| `patentCustomerNameKR` | 특허고객명 | 한글 |
| `patentCustomerNameEN` | 특허고객명 | (영문) |
| `businessRegistrationNumber` | 사업자등록번호 |  |
| `corporationNumber` | 법인번호 |  |
| `corporationTypeCode` | 개인법인구분코드 |  |
| `corporationTypeCodeName` | 개인법인구분코드명 |  |

---

## 이력정보
`applicantNmChHistoryInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `patentCustomerNumber` | 특허고객번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantNmChHistoryInfo` |  |  |
| `changeHistoryOrder` | 변경이력순서 |  |
| `patentCustomerNumber` | 특허고객번호 |  |
| `receiptNumber` | 접수번호 |  |
| `changeDate` | 변경일자 |  |
| `patentCustomerNameKR` | 특허고객명 | 한글 |
| `patentCustomerNameEN` | 특허고객명 | (영문) |
| `krNameChangeYN` | 국문명칭변경여부 |  |
| `enNameChangeYN` | 영문명칭변경여부 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 특허고객번호1&#124;특허고객번호2) |

---

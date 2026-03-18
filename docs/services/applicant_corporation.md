# 출원인 법인

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)

---

## 출원인 법인 및 사업자 번호(특허고객번호)
`corpBsApplicantInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `ApplicantNumber` | 특허고객번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `corpBsApplicantInfo` |  |  |
| `ApplicantNumber` | 특허고객번호 |  |
| `ApplicantName` | 출원인명 |  |
| `CorporationNumber` | 법인번호 |  |
| `BusinessRegistrationNumber` | 사업자등록번호 |  |

---

## 출원인 법인 및 사업자 번호(법인번호)
`corpBsApplicantInfoV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `corporationNumber` | 법인번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `corpBsApplicantInfoV2` |  |  |
| `ApplicantNumber` | 특허고객번호 |  |
| `ApplicantName` | 출원인명 |  |
| `CorporationNumber` | 법인번호 |  |
| `BusinessRegistrationNumber` | 사업자등록번호 |  |

---

## 출원인 법인 및 사업자 번호(사업자번호)
`corpBsApplicantInfoV3`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `BusinessRegistrationNumber` | 사업자등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `corpBsApplicantInfo` |  |  |
| `ApplicantNumber` | 특허고객번호 |  |
| `ApplicantName` | 출원인명 |  |
| `CorporationNumber` | 법인번호 |  |
| `BusinessRegistrationNumber` | 사업자등록번호 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1 : 출원인 법인 및 사업자 번호(특허고객번호), oper2 : 출원인 법인 및 사업자 번호(법인번호), oper3 : 출원인 법인 및 사업자 번호(사업자번호)) ※ oper1, oper2, oper3 중 원하는 변동정보 검색코드 입력 |
| `year` | 연도 | ※입력방식(ex : YYYY) |
| `quarter` | 분기 | ※입력방식(1 : 1분기, 2: 2분기, 3 : 3분기, 4 : 4분기) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 변동리스트 |  |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | 기본-국내출원번호, DOCP-DOCDB공보번호, DOCA-DOCDB출원번호 |
| `ApplicantNumber` | 특허고객번호 | oper1인 경우만 해당 |
| `CorporationNumber` | 법인번호 | oper2인 경우만 해당 |
| `BusinessRegistrationNumber` | 사업자번호 | oper3인 경우만 해당 |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

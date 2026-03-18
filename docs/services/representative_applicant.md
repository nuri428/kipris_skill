# 대표 출원인

- **API 유형**: REST
- **오퍼레이션 수**: 4개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `RpstApplicantService` (포털 확인)
- **게이트웨이**: OpenAPI (`/openapi/rest/`)
- **인증 키**: `accessKey`

---

## 대표출원인
`rpstApplicantInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rpstApplicantNumber` | 특허고객번호 | (대표출원인번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rpstApplicantInfo` |  |  |
| `applicantNumber` | 특허고객번호 |  |
| `applicantName` | 출원인대표명 | 한글 |
| `applicantNameEng` | 출원인대표명 | 영문 |

---

## 대표출원인V2
`rpstApplicantInfoV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantionNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rpstApplicantV2Info` |  |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `titleOfInvention` | 발명의명칭 |  |
| `titleOfInventionEng` | 발명의명칭 | 영문 |
| `applicantNumber` | 특허고객번호 |  |
| `applicantName` | 출원인대표명 | 한글 |
| `applicantNameEng` | 출원인대표명 | 영문 |
| `rpstApplicantNumber` | 특허고객번호 |  |
| `rpstApplicantName` | 출원인대표명 | 한글 |
| `rpstApplicantNameEng` | 출원인대표명 | 영문 |

---

## 변동정보
`rpstApplicantTransferInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rpstApplicantTransferInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 변동리스트 | ※리스트 형식(특허고객번호,대표출원인번호&#124;) |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rpstApplicantNumber` | 특허고객번호 | (대표출원인번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

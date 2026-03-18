# 국유특허

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 국유특허 기본조회
`governmentownershipPatentInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `GovernmentownershipPatentInfo` |  |  |
| `RegistrationNumber` | 등록번호 |  |
| `InventionInstitution` | 발명기관 |  |
| `Titleofinvention` | 발명의명칭 |  |
| `RegistrationDate` | 등록일자 |  |
| `Continuanceduration` | 존속기간 |  |
| `NochargeType` | 무상구분 |  |
| `EvaluationGrade` | 평가등급 |  |
| `ApplicationNumber` | 출원번호 |  |
| `IntellectualpropertyType` | 지식재산유형 |  |

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
| `transferList` | 등록번호리스트 | (ex : 등록번호1&#124;등록번호2) |

---

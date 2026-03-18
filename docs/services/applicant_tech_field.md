# 출원인 기술분야

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 출원인 권리별 기술분야 정보
`applicantTechInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `patentCustomerNumber` | 특허고객번호 |  |
| `rightType` | 권리구분코드 | (공백:ALL, 1:특허, 2:실용신안, 3:디자인, 4:상표) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantTechInfo` |  |  |
| `patentCustomerNumber` | 특허고객번호 |  |
| `rightType` | 권리구분 |  |
| `rightTypeName` | 권리구분명 |  |
| `serialNumber` | 일련번호 |  |
| `classificationSerialNumber` | 분류일련번호 |  |
| `classificationType` | 분류구분 |  |
| `classificationCode` | 분류코드 |  |
| `version` | 버전 |  |
| `niceCode` | NICE코드 |  |
| `applicationCaseCount` | 출원건수 |  |
| `registrationCaseCount` | 등록건수 |  |
| `terminationCaseCount` | 소멸건수 |  |

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
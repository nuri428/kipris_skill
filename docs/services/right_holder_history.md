# 권리자 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 권리자변동정보
`rightHolderInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightHolderInfo` |  |  |
| `pertinentPartition` | 해당란 |  |
| `rankNumber` | 순위번호 |  |
| `registrationDate` | 등록일자 |  |
| `rankCorrelatorSerialNumber` | 순위관련자일련번호 |  |
| `rankCorrelatorNumber` | 순관련자번호(특허고객번호) |  |
| `rankCorrelatorType` | 순위관련자종류 |  |
| `rankCorrelatorName` | 순위관련자이름 |  |
| `rankCorrelatorAddress` | 순위관련자주소 |  |

---

## 변동정보
`rightHolderTransferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightHolderTransferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 변동일자 |  |
| `transferList` | 등록번호리스트 | (ex : 등록번호1&#124;등록번호2) |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

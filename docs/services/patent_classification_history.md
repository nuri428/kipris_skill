# 특허·실용 분류코드 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 이력정보(IPC)
`ipcClassificationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `ipcClassificationInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `groupSerialNumber` | 그룹일련번호 |  |
| `breakdownSerialNumber` | 내역일련번호 |  |
| `ipcCode` | IPC코드 |  |
| `version` | 분류코드버전 |  |
| `versionDate` | 분류코드버전일자 | (※ 일부 과거건의 경우 일자 대신 버전 정보 출력) |

---

## 이력정보(CPC)
`cpcClassificationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `cpcClassificationInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `groupSerialNumber` | 그룹일련번호 |  |
| `breakdownSerialNumber` | 내역일련번호 |  |
| `cpcCode` | CPC코드 |  |
| `version` | 분류코드버전 |  |
| `versionDate` | 분류코드버전일자 | (※ 일부 과거건의 경우 일자 대신 버전 정보 출력) |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | IPC, CPC |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

# 디자인 분류코드 변동 이력

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 국내분류코드이력정보
`designClassificationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designClassificationInfoResponse` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `DesignSerialNumber` | 디자인일련번호 |  |
| `GroupSerialNumber` | 그룹일련번호 |  |
| `BreakdownSerialNumber` | 내역일련번호 |  |
| `MainClassificationYesorno` | 주분류여부 |  |
| `DomesticClassificationCode` | 국내분류코드 |  |

---

## 로카르노분류코드이력정보
`locarnoClassificationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designClassificationInfoResponse` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `DesignSerialNumber` | 디자인일련번호 |  |
| `GroupSerialNumber` | 그룹일련번호 |  |
| `BreakdownSerialNumber` | 내역일련번호 |  |
| `MainClassificationYesorno` | 주분류여부 |  |
| `LocarnoClassificationCode` | 로카르노분류코드 |  |
| `LocarnoClassificationCodeVER` | 로카르노분류코드버전 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | 기본-국내분류코드, LOC-로카르노 |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---
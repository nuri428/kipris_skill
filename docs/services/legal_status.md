# 법적 상태 이력

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)

---

## 이력정보조회
`getLegStatusHistoryInfoSearch`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Item` |  |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `seq` | 일련번호 |  |
| `legalStatusCode` | 법정상태코드 |  |
| `legalStatusName` | 법적상태명 |  |
| `legalStatusDate` | 법적상태일자 |  |
| `legalStatusComment` | 법적상태설명 |  |

---

## 이벤트정보조회
`getLegStatusEventInfoSearch`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Item` |  |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `seq` | 일련번호 |  |
| `eventseq` | 이벤트일련번호 |  |
| `eventCode` | 이벤트코드 |  |
| `eventName` | 이벤트명 |  |
| `eventDate` | 이벤트일자 |  |

---

## 변동정보
`getTransferListInfoSearch`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1 : 이력정보조회, oper2 : 이벤트정보조회) ※ oper1, oper2 중 원하는 변동정보 검색코드 입력 |
| `searchRight` | 권리 | (all : 전체, p : 특허, u : 실용신안, d : 디자인, t : 상표) ※입력방식(ex : p) |
| `transferDate` | 변동일자 | ※ 입력방식(ex : 20160713) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 현재정보조회
`legalStatusBasicInfo`

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
| `legalStatusBasicInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `legalStatusCode` | 법적상태코드 |  |
| `legalStatusName` | 법적상태명 | 한글 |
| `legalStatusEngName` | 법적상태명 | 영문 |
| `legalStatusDate` | 법적상태일자 |  |
| `legalStatusComment` | 법적상태설명 | 한글 |
| `legalStatusEngComment` | 법적상태설명 | 영문 |

---

## 코드정보조회
`legalStatusCodeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `legalStatusCode` | 법적상태코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusCodeInfo` |  |  |
| `legalStatusCode` | 법적상태코드 |  |
| `legalStatusName` | 법적상태명 |  |
| `legalStatusComment` | 법적상태설명 | 한글 |
| `legalStatusEngName` | 법적상태명 | (영문) |
| `legalStatusEngComment` | 법적상태설명 | (영문) |

---

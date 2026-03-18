# 청구항 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 보정이력순서
`amendmentHistoryInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | ?출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `amendmentHistoryInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptSendSerialNumber` | 접수발송일련번호 |  |
| `receiptSendNumber` | 접수발송번호 |  |
| `receiptSendDate` | 접수발송일자 |  |
| `receiptSendDocumentCode` | 접수발송서류코드 |  |
| `receiptSendDocumentName` | 접수발송서류명 |  |

---

## 보정이력상세내역
`amendmentHistoryDetailInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | ?출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `amendmentHistoryDetailInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptSendSerialNumber` | 접수발송일련번호 |  |
| `receiptSendNumber` | 접수발송번호 |  |
| `petitionclauseNumber` | 청구항번호 |  |
| `changeTypeCode` | 변경구분코드 |  |
| `changeTypeName` | 변경구분명 |  |
| `petitionclause` | 청구항 |  |
| `transferReceiptDocNumber` | 변동대상접수문서번호 |  |
| `transferPetitionclause` | 변동청구항 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-보정이력순서, oper2-보정이력상세내역) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

# 특허·실용 권리자 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)

---

## 국내권리이전이력
`getRightTransferInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightTransferInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `rightTransferSequenceNumber` | 권리이전일련번호 |  |
| `rankNumber` | 순위번호 |  |
| `registrationDate` | 등록일자 |  |
| `receiptNumber` | 접수번호 |  |
| `documentCode` | 서류코드 |  |
| `documentName` | 서류명 |  |
| `registrationCauseName` | 등록원인명 |  |
| `inputDate` | 입력일자 |  |

---

## 국내권리이전관련자
`getRightTransferRelatedPerson`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightTransferInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `rightTransferSequenceNumber` | 권리이전일련번호 |  |
| `registrationRelatedPartyCode` | 등록관련자구분코드 |  |
| `registrationRelatedPartySequenceNumber` | 등록관련자일련번호 |  |
| `rightHolderChangeFlag` | 권리자변경유무 |  |
| `rightHolderCode` | 권리자코드 |  |
| `rightHolderName` | 권리자성명 |  |
| `rightHolderAddress` | 권리자주소 |  |
| `inputDate` | 입력일자 |  |

---

## 국내권리자정보변경이력
`getChangeHistoryOfRightHolderInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightTransferInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `registrationTransferSequenceNumber` | 권리이전일련번호 |  |
| `changeSequenceNumber` | 변경일련번호 |  |
| `registrationDate` | 등록일자 |  |
| `receiptNumber` | 접수번호 |  |
| `documentCode` | 서류코드 |  |
| `documentNumber` | 서류명 |  |
| `informationChangeCause` | 정보변경사유 |  |
| `changeBefore_content` | 변경전내용 |  |
| `changeAfter_content` | 변경후내용 |  |
| `inputDate` | 입력일자 |  |

---

## 국내권리이전이력별권리자
`getRightHoldersByRightTransferInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightTransferInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `registrationTransferSequenceNumber` | 권리이전일련번호 |  |
| `rightHolderSequenceNumber` | 권리자일련번호 |  |
| `rightHolderCode` | 권리자코드 |  |
| `rightHolderName` | 권리자성명 |  |
| `rightHolderAddress` | 권리자주소 |  |
| `inputDate` | 입력일자 |  |

---

## 변동정보
`getRightTransferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 조회종류 | 국내권리이전이력 or 국내권리이전관련자 or 국내권리이전이력별권리자(RT), 국내권리자정보변경이력(RH) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rightTransferInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 등록번호리스트 | (ex : 등록번호1&#124;등록번호2) |

---

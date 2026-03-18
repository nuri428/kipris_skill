# 특허·실용 법적 상태 이력(ST.27)

- **API 유형**: REST
- **오퍼레이션 수**: 9개 (구현: 0, 폐기예정: 0)

---

## 이력 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27Info` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `rightTypeCode` | 권리구분 |  |
| `applicationDate` | 출원일자 |  |
| `openNumber` | 공개번호 |  |
| `openingDate` | 공개일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `trialNumber` | 심판번호 |  |
| `demurrerNumber` | 이의신청번호 |  |
| `keyEventCode` | 주요이벤트코드 |  |
| `detailedEventCode` | 상세법이벤트코드 |  |
| `stateCode` | 법이벤트상태코드 |  |
| `previousStageCode` | 법이벤트전단계코드 |  |
| `currentStageCode` | 법이벤트후단계코드 |  |
| `eventIndicatorCode` | 법이벤트표시코드 |  |
| `nationalEventCode` | 법진행상태코드 |  |
| `eventDate` | 법이벤트일자 |  |

---

## 출원(A) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27AppInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `internationalApplicationNumber` | 국제출원번호 |  |
| `internationalApplicationDate` | 국제출원일자 |  |

---

## 등록전·후심리(E·L·W) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27RegInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `demurrerNumber` | 이의신청번호 |  |
| `oppositionDate` | 이의신청일자 |  |
| `oppositionObject` | 이의신청취지 |  |
| `oppositionMatters` | 이의신청사항 |  |
| `registrationNumber` | 등록번호 |  |
| `oppositionCancellationClauseContent` | 이의신청취소항내용 |  |

---

## IP권리존속기간이후의보호(G) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27AfterRightInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `extensionTargetdemandItemCount` | 연장대상청구항수 |  |
| `extensionTargetPetitionClauseScopeContent` | 연장대상청구항범위내용 |  |
| `extensiontermDate` | 연장기간일 |  |
| `extensiontermMonth` | 연장기간월 |  |
| `extensiontermYear` | 연장기간년 |  |
| `permissionRegistrationContent` | 허가등록내용 |  |

---

## IP권리중단(H) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27StopRightInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `terminationRegistrationCauseDate` | 소멸등록원인일자 |  |
| `terminationRegistrationCauseName` | 소멸등록원인명 |  |

---

## 문서수정(P) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27DocInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `extensionTerminationDate` | 공고제목 |  |
| `internetOpeningPublicDate` | 공개공고일자 |  |
| `openingPublicationNumber` | 인터넷공개공고일자 |  |
| `openingPublicDate` | 공개공고번호 |  |

---

## 납부(U) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27PayInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `startAnnual` | 시작연차 |  |
| `terminationRegistrationCauseDate` | 소멸등록원인일자 |  |
| `terminationRegistrationCauseName` | 소멸등록원인명 |  |

---

## 심판(V) 이벤트 정보 조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 일련번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `legalStatusST27TrialInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `supplySerialNumber` | 보급일련번호 |  |
| `trialTypeCode` | 심판구분 |  |
| `trialNumber` | 심판번호 |  |
| `trialGradeTypeCode` | 심급구분 |  |
| `requestForPatentTrialDate` | 심판청구일자 |  |
| `trialDecisionDate` | 심결일자 |  |
| `trialDecisionPrincipleClauseContent` | 심결주문내용 |  |
| `eventIndicationContent` | 사건표시내용 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | D-이력, A-출원 E-등록전·후심리, G-IP권리존속기간이후, H-IP권리중단, P-문서수정, U-납부, V-심판 |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

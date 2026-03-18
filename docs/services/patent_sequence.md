# 특허 염기서열

- **API 유형**: REST
- **오퍼레이션 수**: 7개 (구현: 0, 폐기예정: 0)

---

## 생명공학출원접수
`biotechApplicationReceiptInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechApplicationReceiptInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingItemCount` | 아미노산염기서열항목수 |  |
| `aminoSeqlistingDrawupProgramName` | 아미노산염기서열작성프로그램 |  |

---

## 생명공학염기서열
`biotechSeqlistingInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechSeqlistingInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingNumber` | 아미노산염기서열번호 |  |
| `aminoSeqlistingLength` | 아미노산염기서열길이 |  |
| `aminoSeqlistingTypeCode` | 아미노산염기서열유형코드 |  |
| `aminoSeqlistingOrganismSeedName` | 아미노산염기서열생물종명 |  |

---

## 생명공학염기서열특징
`biotechSeqlistingFeatureInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechSeqlistingFeatureInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingNumber` | 아미노산염기서열번호 |  |
| `aminoSeqlistingFeatureSerialNumber` | 아미노산염기서열특징일련번호 |  |
| `aminoSeqlistingFeatureName` | 아미노산염기서열특징명칭 |  |
| `aminoSeqlistingFeatureLocationContent` | 아미노산염기서열특징위치내용 |  |
| `aminoSeqlistingFeatureEtceteraContent` | 아미노산염기서열특징기타내용 |  |

---

## 생명공학염기서열원문
`biotechSeqlistingOriginaltextInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechSeqlistingOriginaltextInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingNumber` | 아미노산염기서열번호 |  |
| `aminoSeqlistingContentSerialNumber` | 아미노산염기서열일련번호 |  |
| `aminoSeqlistingContent` | 아미노산염기서열내용 |  |

---

## 생명공학간행물
`biotechJournalInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechJournalInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingNumber` | 아미노산염기서열번호 |  |
| `journalSerialNumber` | 간행물일련번호 |  |
| `journalTitle` | 간행물제목 |  |
| `journalName` | 간행물명 |  |
| `journalAuthorName` | 간행물저자성명 |  |
| `journalVolumeCount` | 간행물권수 |  |
| `journalIssueNumber` | 간행물발간번호 |  |
| `journalIssueDate` | 간행물발간일자 |  |
| `journalPageScopeContent` | 간행물페이지범위내용 |  |
| `databaseRegistrationNumber` | DB등록번호 |  |
| `databaseRegistrationDate` | DB등록일자 |  |
| `citationNumber` | 인용문헌번호 |  |
| `citationApplicationDate` | 인용문헌출원일자 |  |
| `citationOpeningDate` | 인용문헌공개일자 |  |
| `aminoSeqlistingFeatureLocationContent` | 아미노산염기서열특징위치내용 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-생명공학출원접수, oper2-생명공학염기서열, oper3-생명공학염기서열특징, oper4-생명공학염기서열원문, oper5-생명공학간행물, oper6-생명공학염기서열원문가공)) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 생명공학염기서열원문가공
`biotechSeqlistingOriginaltextManufactureInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `biotechSeqlistingOriginaltextManufactureInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `aminoSeqlistingNumber` | 아미노산염기서열일련번호 |  |
| `aminoSeqlistingContentSerialNumber` | 아미노산염기서열내용일련번호 |  |
| `aminoSeqlistingContentRelationSerialNumber` | 아미노산염기서열내용관련일련번호 |  |
| `aminoSeqlistingContent` | 아미노산염기서열내용 |  |

---

# 등록결정서

- **API 유형**: REST
- **오퍼레이션 수**: 9개 (구현: 0, 폐기예정: 1)

---

## 서지정보
`bibliographicInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `bibliographicInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `documentSendNumber` | 문서발송번호 |  |
| `sendDate` | 발송일자 |  |
| `documentSentence` | 문서문구 |  |
| `documentType` | 문서타입 |  |
| `documentPublicationInstitution` | 문서발행기관 |  |
| `documentName` | 문서명 |  |
| `documentDrawupDate` | 문서작성일자 |  |
| `documentApplicationNumber` | 문서출원번호 |  |
| `inventionName` | 발명의명칭 |  |
| `demandItemcount` | 청구항수 |  |
| `originalRegistrationNumber` | 원등록번호 |  |
| `designSerialNumber` | 디자인일련번호 |  |

---

## 인명정보
`personInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `personInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `personType` | 인명구분 |  |
| `contentType` | 내용구분 |  |
| `patentCustomerNumber` | 특허고객번호 |  |
| `content` | 내용 |  |
| `applicationRelationpersonName` | 출원관련인명 |  |
| `designationPatentattorneyName` | 지정변리사명 |  |
| `examinationdepartmentName` | 심사국명 |  |
| `examinationsectionName` | 심사과명 |  |
| `contentInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `personType` | 인명구분 |  |
| `contentType` | 내용구분 |  |
| `content` | 내용 |  |
| `patentCustomerNumber` | 특허고객번호 |  |
| `applicationRelationpersonName` | 출원관련인명 |  |
| `designationPatentattorneyName` | 지정변리사명 |  |
| `examinationdepartmentName` | 심사국명 |  |
| `examinationsectionName` | 심사과명 |  |

---

## 등록결정 및 안내정보
`contentInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `contentInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `contentType` | 내용구분 |  |
| `amendmentTitle` | 직권보정타이틀 |  |
| `content` | 내용 |  |
| `amendmentItem` | 보정항목 |  |
| `amendmentLocation` | 보정위치 |  |
| `amendmentBeforeContent` | 보정전내용 |  |
| `amendmentAfterContent` | 보정후내용 |  |
| `amendmentCause` | 보정사유 |  |
| `amendmentInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `amendmentTitle` | 직권보정타이틀 |  |
| `contentType` | 내용구분 |  |
| `content` | 내용 |  |
| `amendmentItem` | 보정항목 |  |
| `amendmentLocation` | 보정위치 |  |
| `amendmentBeforeContent` | 보정전내용 |  |
| `amendmentAfterContent` | 보정후내용 |  |
| `amendmentCause` | 보정사유 |  |

---

## 직권보정정보
`amendmentInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `amendmentInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `amendmentTitle` | 직권보정타이틀 |  |
| `imageFileName` | 이미지파일명 |  |
| `imageWidth` | 이미지너비 |  |
| `amendmentItem` | 보정항목 |  |
| `imageHeight` | 이미지높이 |  |
| `amendmentLocation` | 보정위치 |  |
| `amendmentBeforeContent` | 보정전내용 |  |
| `imagePath` | 이미지경로 |  |
| `amendmentAfterContent` | 보정후내용 |  |
| `amendmentCause` | 보정사유 |  |
| `imageInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `amendmentTitle` | 직권보정타이틀 |  |
| `imageFileName` | 이미지파일명 |  |
| `imageWidth` | 이미지너비 |  |
| `amendmentItem` | 보정항목 |  |
| `amendmentLocation` | 보정위치 |  |
| `imageHeight` | 이미지높이 |  |
| `imagePath` | 이미지경로 |  |
| `amendmentBeforeContent` | 보정전내용 |  |
| `amendmentAfterContent` | 보정후내용 |  |
| `amendmentCause` | 보정사유 |  |

---

## 이미지수록정보
`imageInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `imageInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `imageFileName` | 이미지파일명 |  |
| `imageWidth` | 이미지너비 |  |
| `imageHeight` | 이미지높이 |  |
| `imagePath` | 이미지경로 |  |

---

## 상세정보
`detailInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `detailInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `serialNumber` | 일련번호 |  |
| `detailInfoTitle` | 상세정보타이틀 |  |
| `detailInfoCountryCode` | 상세정보국가코드 |  |
| `detailInfoNumber` | 상세정보번호 |  |
| `detailInfoCode` | 상세정보코드 |  |
| `detailInfoDesignSerialNumber` | 상세정보디자인일련번호 |  |
| `detailInfoAttachmentContent` | 상세정보첨부내용 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-서지정보, oper2-인명정보, oper3-등록결정 및 안내정보, oper4-직권보정정보, oper5-이미지수록정보, oper6-상세정보, oper7-PDF) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 검색건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## PDF(폐기예정)
`pdfInfo`

- **분류**: 오퍼레이션
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `pdfInfo` |  |  |
| `fileName` | 파일명 |  |
| `filePath` | 파일경로 |  |

---

## PDF_V2
`pdfInfoV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `pdfInfoV2` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `fileName` | 파일명 |  |
| `filePath` | 파일경로 |  |

---

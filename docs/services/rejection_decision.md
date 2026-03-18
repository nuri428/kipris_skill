# 거절결정서

- **API 유형**: REST
- **오퍼레이션 수**: 12개 (구현: 0, 폐기예정: 1)
- **서비스 경로**: `IntermediateDocumentREService` ⚠️ 미검증 (RE=Rejection 추정, 등록결정서일 수도 있음)
- **게이트웨이**: OpenAPI (`/openapi/rest/`) (추정)

---

## 전체검색
`advancedSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `word` | 자유검색 |  |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 |  |
| `inventionTitle` | 제목 | (특허,실용) 발명의명칭, (디자인) 품명 (※ 상표명은 지원하지 않습니다.) |
| `rejectionContent` | 거절사유 |  |
| `sendDate` | 발송일자 |  |
| `sendNumber` | 발송번호 |  |
| `relationpersonName` | 관련자검색 | (출원인, 대리인) |
| `patent` | 특허포함여부 | (true - 포함, false - 미포함)(※ 미입력시 자동 true 검색) |
| `utility` | 실용신안포함여부 | (true - 포함, false - 미포함)(※ 미입력시 자동 true 검색) |
| `design` | 디자인포함여부 | (true - 포함, false - 미포함)(※ 미입력시 자동 true 검색) |
| `tradeMark` | 상표포함여부 | (true - 포함, false - 미포함)(※ 미입력시 자동 true 검색) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |
| `sortSpec` | 정렬기준 | (입력값 : AN(출원번호), AD(출원일자), MN(발송번호), SD(발송일자) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `advancedSearchInfo` |  |  |
| `indexNo` | 검색인덱스번호 |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `sendDate` | 발송일자 |  |
| `title` | 제목 | 발명의명칭(특허,실용), 품명(디자인) (※ 상표명은 제공하지 않습니다.) |
| `filePath` | 서류철PDF경로 |  |

---

## 심사관정보
`examinerInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `examinerInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `sequence` | 순번 |  |
| `documentDrawupDate` | 작성일자 |  |
| `publicationInstitutionName` | 작성처 |  |
| `examinationDepartmentName` | 심사국 |  |
| `examinationType` | 직책 |  |
| `examinerName` | 심사관명 |  |

---

## 심사결과
`examineResultInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 | (※특허,실용신안만 해당) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `examineResultInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `examinationTitle` | 심사대상청구항제목 |  |
| `examinationContent` | 심사대상청구항내용 |  |
| `refusalLawTitle` | 거절이유관련법조항제목 |  |
| `refusalLawTabularstatement` | 거절이유관련법조항표 |  |
| `patentAbleTitle` | 특허가능청구항제목 |  |
| `patentAbleContent` | 특허가능청구항내용 |  |
| `descriptionSummary` | 청구항설명요약 |  |
| `refusalLawarticleSequence` | 거절이유법조항순번 |  |
| `refusalPetitionclause` | 거절이유청구항 |  |
| `refusalLawarticleContent` | 거절이유법조항내용 |  |
| `supplementaryTitle` | 보정서제목 |  |
| `supplementaryContentOne` | 보정서내용1 |  |
| `supplementaryContentTwo` | 보정서내용2 |  |
| `supplementaryContentThree` | 보정서내용3 |  |
| `supplementaryContentFour` | 보정서내용4 |  |

---

## 거절결정내용
`rejectDecisionInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `rejectDecisionInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `lawContent` | 거절내용 |  |
| `lawContentDetail` | 거절결정내용2 |  |
| `lawContentNumber` | 거절결정내용3 |  |
| `rejectionContentTitle` | 거절제목 |  |
| `rejectionContentDetail` | 거절결정내용1 |  |
| `attachmentfileTitle` | 첨부파일제목 |  |
| `attachmentfileContent` | 첨부파일내용 |  |
| `guidanceTitle` | 안내제목 |  |
| `guidanceContent` | 안내내용 |  |

---

## 추가거절내용
`additionRejectInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `additionRejectInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `sendNumber` | 발송번호 |  |
| `sequence` | 순번 |  |
| `additionRejectionContent` | 추가거절내용 |  |

---

## 서지정보
`bibliographicInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber?` | 출원번호 | (선택) |
| `sendDate` | 발송일자 | (선택) |
| `submitDuedate` | 제출일자 | (선택) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `bibliographicInfo` |  |  |
| `applicationNumber` | 출원일자 |  |
| `sendNumber` | 발송번호 |  |
| `documentSendNumber` | 문서발송번호 |  |
| `sendDate` | 발송일자 |  |
| `submitDuedate` | 제출기한일자 |  |
| `publicationInstitution` | 문서발행기관 |  |
| `documentName` | 문서명 |  |
| `documentCode` | 문서코드 |  |
| `documentKind` | 문서종류 |  |
| `rightNumber` | 권리번호 |  |
| `documentApplicationNumber` | 문서출원번호 |  |
| `inventionTitle` | 발명제목 |  |
| `documentSentence` | 문서문구 |  |
| `registrationNumber` | 등록번호 |  |
| `technologyNumber` | 기술평가번호 |  |
| `technologyDate` | 기술평가일자 |  |
| `oppositionNumber` | 이의신청번호 |  |
| `oppositionDate` | 이의신청일자 |  |
| `technologyDescription` | 기술평가설명 |  |
| `relationApplicationNumber` | 권련출원번호 |  |
| `designSerialNumber` | 디자인일련번호 |  |
| `applicationDate` | 출원일자 |  |

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
| `sequence` | 순번 |  |
| `relationpersonType` | 관련인종류 |  |
| `relationpersonName` | 출원인명/ |  |
| `relationpersonNumber` | 관련인번호 |  |
| `patentattorneyName` | 변리사명 |  |

---

## 이미지
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
| `seq` | 순서 |  |
| `imageName` | 이미지명 |  |
| `imagePath` | 이미지경로 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-심사관정보, oper2-거절결정내용, oper3-심사결과, oper4-추가결정내용, oper5-서지정보, oper6-인명정보, oper7-이미지, oper8-삭제정보, oper9-PDF) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
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

## 최종변동일자

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
| `lastTransferDateInfo` | 최종변동일자 |  |

---

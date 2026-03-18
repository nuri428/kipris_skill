# 디자인 공보

- **API 유형**: REST
- **오퍼레이션 수**: 51개 (구현: 0, 폐기예정: 4)

---

## 단어(폐기예정)
`getWordSearch`

- **분류**: 일반검색
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `articleName` | 디자인물품명칭 | (물품명칭, 출원인, 창작자 및 창작자 주소) |
| `searchYearRange` | 검색년도범위 | (0:전체, 최근 1~10년) |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `number` | 번호 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `applicationStatus` | 등록상태 |  |
| `applicantName` | 출원인명 |  |
| `agentName` | 대리인명 |  |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `dsShpClssCd` | 형태분류 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |
| `designNumber` | 디자인일련번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `count` |  |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 번호(폐기예정)
`getNumberSearch`

- **분류**: 일반검색
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `number` | 숫자키워드 |  |
| `searchYear` | 검색년도범위 | (0:전체 년도입력 ex:1999) |
| `pageNo` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `numOfRows` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `item` |  |  |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationStatus` | 상태 |  |
| `articleName` | 디자인물품명칭 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `designNumber` | 디자인일련번호 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `fullText` | 전문존재유무 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `inventorName` | 창작자명 |  |
| `number` | 일련번호 |  |
| `openDate` | 공개일자 |  |
| `openNumber` | 공개번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `publicationDate` | 공고일자 |  |
| `publicationNumber` | 공고번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `count` |  |  |
| `numOfRows` |  |  |
| `pageNo` | 페이지번호 | (검색 페이지 번호) |
| `totalCount` | 전체건수 |  |

---

## 전체검색
`getAdvancedSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `free` | 자유검색 |  |
| `articleName` | 디자인물품명칭 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 형태분류 |  |
| `applicationNumber` | 출원번호 | (AN) |
| `registrationNumber` | 등록번호 | (RN) |
| `publicationNumber` | 공고번호 | (PN) |
| `openNumber` | 공개번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `applicationDate` | 출원일자 | (AD) |
| `registrationDate` | 등록일자 | (RD) |
| `publicationDate` | 공고일자 | (PD) |
| `openDate` | 공개일자 |  |
| `priorityDate` | 우선권주장일자 | (PRD) |
| `inventorName` | 창작자명 |  |
| `applicantName` | 출원인명/특허고객번호 |  |
| `agentName` | 대리인번호 | (AG) |
| `regPrivilegeName` | 등록권자 | (RG) |
| `open` | 공개 |  |
| `rejection` | 거절 |  |
| `destroy` | 소멸 |  |
| `cancle` | 취하 |  |
| `notice` | 공고 |  |
| `registration` | 등록 |  |
| `invalid` | 무효 |  |
| `abandonment` | 포기 |  |
| `simi` | 유사디자인 |  |
| `part` | 부분디자인 |  |
| `etc` | 기타디자인 |  |
| `pageNo` | 페이지번호 |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `number` | 번호 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `applicationStatus` | 출원상태 |  |
| `applicantName` | 출원인명 |  |
| `agentName` | 대리인명 |  |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `dsShpClssCd` | 형태분류 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |
| `designNumber` | 디자인일련번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `count` |  |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 형태분류 검색
`designFormClassInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `dsShpClssCd` | 형태분류코드 |  |
| `open` | 공개 | (포함 : true, 미포함 : false) |
| `rejection` | 거절 | (포함 : true, 미포함 : false) |
| `destroy` | 소멸 | (포함 : true, 미포함 : false) |
| `cancle` | 취하 | (포함 : true, 미포함 : false) |
| `notice` | 공고 | (포함 : true, 미포함 : false) |
| `registration` | 등록 | (포함 : true, 미포함 : false) |
| `invalid` | 무효 | (포함 : true, 미포함 : false) |
| `abandonment` | 포기 | (포함 : true, 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true, 미포함 : false) |
| `part` | 부분디자인 | (포함 : true, 미포함 : false) |
| `etc` | 기타디자인 | (포함 : true, 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `sortSpec` | 정렬기준 | (AD-출원일자, OD-공개일자, RD-등록일자, PD-공고일자, PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 번호 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원잠조번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `regReferenceNumber` | 등록참조일자 |  |
| `registrationDate` | 등록일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `applicationStatus` | 출원상태 |  |
| `applicantName` | 출원인명 |  |
| `agentName` | 대리인명 |  |
| `fullText` | 전문유무 | (Y/N) |
| `inventorName` | 발명자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `dsShpClssCd` | 디자인형태분류 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 자유검색
`freeSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `free` | 자유검색 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 물품명칭
`articleNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `articleName` | 물품명칭 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 디자인분류
`designMainClassificationSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designMainClassification` | 디자인분류코드 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 출원번호
`applicationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 등록번호
`registrationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 공고번호
`publicationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `publicationNumber` | 공고번호 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 공개번호
`openNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `openNumber` | 공개번호 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 우선권주장번호
`priorityNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityNumber` | 우선권주장번호 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 출원일자
`applicationDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationDate` | 출원일자 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 등록일자
`registrationDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationDate` | 등록일자 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 공고일자
`publicationDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `publicationDate` | 공고일자 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 공개일자
`openDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `openDate` | 공개일자 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 우선권주장일자
`priorityDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityDate` | 우선권주장일자 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 창작자
`inventorNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `inventorName` | 창작자명 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 출원인
`applicantNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 대리인
`agentNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 등록권자
`regPrivilegeNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `regPrivilegeName` | 등록권자명 |  |
| `etc` | 기타디자인 | (포함 : true 미포함 : false) |
| `part` | 부분디자인 | (포함 : true 미포함 : false) |
| `simi` | 유사디자인 | (포함 : true 미포함 : false) |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `cancle` | 취하 | (포함 : true 미포함 : false) |
| `destroy` | 소멸 | (포함 : true 미포함 : false) |
| `invalid` | 무효 | (포함 : true 미포함 : false) |
| `notice` | 공고 | (포함 : true 미포함 : false) |
| `open` | 공개 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `rejection` | 거절 | (포함 : true 미포함 : false) |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 OD-공개일자 RD-등록일자 PD-공고일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalCount` | 전체건수 |  |
| `DesignInfo` |  |  |
| `number` | 일련번호 |  |
| `applicationNumber` | 출원번호 | (국제등록번호) |
| `applicationDate` | 출원일자 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `applicationStatus` | 상태 |  |
| `applicantName` | 출원인명/특허고개번호 | 출원인명 특허고객번호 |
| `agentName` | 대리인명/대리인번호 | 대리인명 대리인번호 |
| `fullText` | 전문존재유무 |  |
| `inventorName` | 창작자명 |  |
| `articleName` | 디자인물품명칭 |  |
| `openNumber` | 공개번호 |  |
| `openDate` | 공개일자 |  |
| `designMainClassification` | 디자인분류코드 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imagePath` | 이미지경로 |  |
| `imagePathLarge` | 큰이미지경로 |  |

---

## 서지상세정보(공공데이터 포털 연계)
`getBibliographyDetailInfoSearch`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `agentInfoArray` |  |  |
| `agentInfo` |  |  |
| `agentAddress` | 대리인주소 |  |
| `agentCode` | 대리인번호 |  |
| `agentCountry` | 대리인국가 |  |
| `agentName` | 대리인명 |  |
| `applicantInfoArray` |  |  |
| `applicantInfo` |  |  |
| `applicantAddress` | 출원인주소 |  |
| `applicantCode` | 출원인번호 |  |
| `applicantCountry` | 출원인국가 |  |
| `applicantName` | 출원인명 |  |
| `biblioSummaryInfoArray` |  |  |
| `biblioInfoArray` |  |  |
| `biblioSummaryInfo` |  |  |
| `admstStat` | 행정처분상태 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 |  |
| `articleName` | 디자인물품명칭 |  |
| `designBasicSimilarYn` | 기본유사유무 |  |
| `designCount` | 의장의수 |  |
| `designCountNumber` | 의장의수(실제숫자) |  |
| `designNumber` | 디자인일련번호 |  |
| `designPriorityApplicationCountry` | 우선권주장국가 |  |
| `designPriorityApplicationDate` | 우선권주장일자 |  |
| `designPriorityApplicationNumber` | 우선권주장번호 |  |
| `dsScgrtDmndYn` | 비밀의장여부 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imgFg` | 견본이미지유무 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `lastDispositionCode` | 최종처분코드 |  |
| `lastDispositionDate` | 최종처분일자 |  |
| `lastDispositionDescription` | 최종처분설명 |  |
| `lastRetroDate` | 최종소급일자 |  |
| `lastRetroDescription` | 최종소급구분설명 |  |
| `lastRetroTpcd` | 최종소급구분코드 |  |
| `openDate` | 공개일자 |  |
| `openNumber` | 공개번호 |  |
| `originalApplicationDate` | 원출원일자 |  |
| `originalApplicationNumber` | 원출원번호 |  |
| `partDesignFg` | 부분의장여부 |  |
| `pubFg` | 공고공보유무 |  |
| `publicationDate` | 공고일자 |  |
| `publicationNumber` | 공고번호 |  |
| `regFg` | 등록유무 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `relationApplicationNumber` | 관련출원번호 |  |
| `repubFg` | 정정공보유무 |  |
| `rgstTpcd` | 등록상태 |  |
| `rgstTpcdDscr` | 등록상태설명 |  |
| `classificationCodeInfoArray` |  |  |
| `classificationCodeInfo` |  |  |
| `classificationCode` | 디자인분류코드 |  |
| `designImageInfoArray` |  |  |
| `designImageInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `imagePath` |  |  |
| `imageName` | 이미지명 |  |
| `largePath` | 큰이미지경로 |  |
| `number` | 순번 |  |
| `smallPath` | 이미지경로 |  |
| `fullTextInfoArray` |  |  |
| `fullTextInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `fullTextFileKindCode` | 전문파일종류코드 |  |
| `fullTextFilePath` | 전문파일경로 |  |
| `pageCount` | 페이지수 |  |
| `creativeDescriptionInfoArray` |  |  |
| `creativeDescriptionInfo` |  |  |
| `designDescription` | 창작의내용 |  |
| `designNumber` | 디지안일련번호 |  |
| `creativeSummaryInfoArray` |  |  |
| `creativeSummaryInfo` |  |  |
| `designNumber` | 디지안일련번호 |  |
| `designSummary` | 창작의요점 |  |
| `inventorInfoArray` |  |  |
| `inventorInfo` |  |  |
| `designNumber` | 디지안일련번호 |  |
| `inventorAddress` | 창작자주소 |  |
| `inventorCode` | 특허고객번호(창작자번호) |  |
| `inventorCountry` | 창작자국가 |  |
| `inventorName` | 창작자명 |  |
| `legalStatusInfoArray` |  |  |
| `legalStatusInfo` |  |  |
| `procSTCD` | 처리상태코드 |  |
| `rsDate` | 접수발송일자 |  |
| `rsDocumentName` | 접수발송서류명 | 한글 |
| `rsDocumentNameEng` | 접수발송서류명 | 영문 |
| `rsNo` | 접수발송번호 |  |

---

## 한국분류(2021)
`designClasscodeInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignClasscodeInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `DesignClasscode` | 한국분류코드 |  |
| `DesignClassificationTypeCode` | 한국분류구분코드 | (S14001 : 주분류, S14002 : 부분류) |

---

## 국제분류(2021)
`designLocarnoClasscodeInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignLocarnoClasscodeInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `LocarnoClasscode` | 국제분류코드 | (로카르노) |

---

## 형태분류(2021)
`designShapeClasscodeInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignShapeClasscodeInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `ShapeClasscode` | 형태분류코드 |  |

---

## 우선권정보(2021)
`designClaimofpriorityInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignClaimofpriorityInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `ClaimofpriorityNumber` | 우선권주장번호 |  |
| `ClaimofpriorityDate` | 우선권주장일자 |  |
| `CountryCode` | 국가코드 |  |
| `CountryName` | 국가명칭 |  |

---

## 창작자
`getInventorInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designInventorInfoList` |  |  |
| `designInventorInfo` |  |  |
| `designNumber` | 디자인일련번호 |  |
| `inventorName` | 창작자명 |  |
| `inventorCode` | 특허고객번호(창작자번호) | 특허고객번호(창작자번호) |
| `inventorAddress` | 창작자주소 |  |
| `inventorCountry` | 창작자국가 |  |

---

## 출원인
`getApplicantInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designApplicantInfoList` |  |  |
| `designApplicantInfo` |  |  |
| `applicantName` | 출원인명 |  |
| `applicantCode` | 특허고객번호 |  |
| `applicantAddress` | 출원인주소 |  |
| `applicantCountry` | 출원인국가 |  |

---

## 대리인
`getAgentInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designAgentInfoList` |  |  |
| `designAgentInfo` |  |  |
| `agentName` | 대리인명 |  |
| `agentCode` | 대리인번호 |  |
| `agentAddress` | 대리인주소 |  |
| `agentCountry` | 대리인국가 |  |

---

## 창작의 요점
`getCreativeSummaryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designCreativeSummaryInfoList` |  |  |
| `designCreativeSummaryInfo` |  |  |
| `designNumber` | 디자인일련번호 |  |
| `designSummary` | 창작의요점 |  |

---

## 창작의 내용
`getCreativeDescriptionInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designCreativeDescriptionInfoList` |  |  |
| `designCreativeDescriptionInfo` |  |  |
| `designNumber` | 디자인일련번호 |  |
| `designDescription` | 창작의내용 |  |

---

## 행정처리사항
`getLegalStatusInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designLegalStatusInfoList` |  |  |
| `designLegalStatusInfo` |  |  |
| `rsNo` | 접수발송번호 |  |
| `rsDocumentName` | 접수발송서류명 |  |
| `rsDate` | 접수발송일자 |  |
| `procSTCD` | 처리상태코드 |  |

---

## 서지요약정보
`getDesignBibliographicSummaryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `biblioSummaryInfoArray` |  |  |
| `biblioSummaryInfo` |  |  |
| `admstStat` | 법적상태 |  |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `articleName` | 디자인물품명칭 |  |
| `designBasicSimilarYn` | 기본유사유무 |  |
| `designCount` | 단독디자인다디자인구분 |  |
| `designCountNumber` | 의장의수 |  |
| `designNumber` | 디자인일련번호 |  |
| `designPriorityApplicationCountry` | 우선권주장국가 |  |
| `designPriorityApplicationDate` | 우선권주장일자 |  |
| `designPriorityApplicationNumber` | 우?권주장번호 |  |
| `dsScgrtDmndYn` | 비밀의장여부 |  |
| `dsShpClssCd` | 디자인형태분류코드 |  |
| `imgFg` | 견본이미지유무 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `lastDispositionCode` | 심사진행상태코드 |  |
| `lastDispositionDate` | 심사진행일자 |  |
| `lastDispositionDescription` | 심사진행상태명 |  |
| `lastRetroDate` | 최종소급일자 |  |
| `lastRetroDescription` | 최종소급구분설명 |  |
| `lastRetroTpcd` | 최종소급구분코드 |  |
| `openDate` | 공개일자 |  |
| `openNumber` | 공개번호 |  |
| `originalApplicationDate` | 원출원일자 |  |
| `originalApplicationNumber` | 원출원번호 |  |
| `partDesignFg` | 부분의장여부 |  |
| `pubFg` | 공고공보유무 |  |
| `publicationDate` | 공고일자 |  |
| `publicationNumber` | 공고번호 |  |
| `regFg` | 등록유무 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `relationApplicationNumber` | 관련출원번호 |  |
| `repubFg` | 정정공보유무 |  |
| `rgstTpcd` | 등록상태 |  |
| `rgstTpcdDscr` | 등록상태설명 |  |
| `classificationCodeInfo` |  |  |
| `classificationCode` | 디자인분류코드 |  |
| `designImageInfo` |  |  |
| `imagePath` |  |  |
| `imageName` | 디자인이미지파일이름 |  |
| `largePath` | 큰이미지경로 |  |
| `number` | 순번 |  |
| `smallPath` | 이미지경로 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `fullTextInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `fullTextFileKindCode` | 전문파일종류코드 |  |
| `fullTextFilePath` | 전문파일경로 |  |
| `pageCount` | 페이지수 |  |

---

## 디자인 육면도
`getSixImageInfoSearch`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `designNumber` | 디자인일련번호 |  |
| `imagePath` |  |  |
| `imageName` | 이미지명 |  |
| `largePath` | 큰이미지경로 |  |
| `number` | 번호 |  |
| `smallPath` | 이미지경로 |  |

---

## 공개 전문(폐기예정)
`getPubFullTextInfoSearch`

- **분류**: 도면/전문
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `fileName` | 파일명 |  |
| `path` | 파일경로 |  |

---

## 공고 전문(폐기예정)
`getAnnFullTextInfoSearch`

- **분류**: 도면/전문
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `fileName` | 파일명 |  |
| `path` | 파일경로 |  |

---

## 정정공보
`designUpdateGazetteInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designUpdateGazetteInfo` |  |  |
| `fileName` | 파일명 |  |
| `filePath` | 파일경로 |  |
| `updateDate` | 정정일자 |  |
| `version` | 버전 |  |

---

## 공개전문(2021)
`designOpeningGazetteInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignOpeningGazetteInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `FileName` | 파일명 |  |
| `FilePath` | 파일경로 |  |
| `FileKindCode` | 파일종류 | (S10221:PDF) ※ 참고사항 : 2021.9.13일 기준으로 PDF 보유건에 대해서만 제공합니다. |

---

## 공고전문(2021)
`designRegistrationGazetteInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `designSerialnumber` | 디자인일련번호 | (옵션) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `DesignRegistrationGazetteInfo` |  |  |
| `Applicationnumber` | 출원번호 |  |
| `DesignSerialnumber` | 디자인일련번호 |  |
| `FileName` | 파일명 |  |
| `FilePath` | 파일경로 |  |
| `FileKindCode` | 파일종류 | (S10221:PDF) ※ 참고사항 : 2021.9.13일 기준으로 PDF 보유건에 대해서만 제공합니다. |

---

## 공고책자
`getExamPubBookInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designExamPubBookInfoList` |  |  |
| `designExamPubBookInfo` |  |  |
| `path` | 경로 |  |
| `fileName` | 파일이름 |  |

---

## 모든 전문 및 육면도 유무
`getFullTextCheckInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designFullTextCheckInfo` |  |  |
| `unexPubfullDocPDFCheckResult` | 공개전문유무 | (있음:Y 없음:N) |
| `examPubfullDocPDFCheckResult` | 공고전문유무 | (있음:Y 없음:N) |
| `unexPubBookCheckResult` | 공개책자유무 | (있음:Y 없음:N) |
| `examPubBookCheckResult` | 공고책자유무 | (있음:Y 없음:N) |
| `sixImageCheckResult` | 육면도유무 | (있음:Y 없음:N) |
| `registrationCheckResult` | 등록사항유무 | (있음:Y 없음:N) |
| `revisionPublicationCheckResult` | 정정공보유무 | (있음:Y 없음:N) |

---

## 변동정보
`getChangeInfoSearch`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `date` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `itme` |  |  |
| `count` | 변동건수 |  |
| `transListString` | 출원번호리스트 | 3019880015095&#124;3019900010240&#124;3019910011543&#124;...&#124; |

---

## 변동정보2(2021)
`designTransferInfo2`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 종류 | (한국분류:DCC, 국제분류:DLC, 형태분류:DSC, 공개전문:DOG, 공고전문:DRG, 우선권정보:DCP) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designTransferInfo2` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 디자인 분류
`designCodeSearchInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designNumber` | 디자인분류코드/디자인물품명칭 |  |
| `startNumber` | 페이지번호 | (검색한 결과물의 출력할 번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `getSearchDesignCodeInfoList` |  |  |
| `getSearchDesignCodeInfo` |  |  |
| `designNumber` | 디자인일련번호 |  |
| `designName` | 디자인물품명칭 |  |

---

## 형태분류(초기검색 리스트)
`getShapeFirstInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `-` |  |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `designShapeFirstInfoList` |  |  |
| `designShapeFirstInfo` |  |  |
| `eipcSec` | 디자인섹션 |  |
| `eipcDesc` | 디자인형태분류코드설명 |  |

---

## 형태분류(섹션조회)
`getEipcSecInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `eipcSec` | 섹션 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `designEipcSecInfoList` |  |  |
| `designEipcSecInfo` |  |  |
| `eipcCls` | 디자인클래스 |  |
| `eipcSec` | 디자인섹션 |  |
| `eipcDesc` | 디자인형태분류코드설명 |  |

---

## 형태분류(클래스조회)
`getEipcClassInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `eipcSec` | 섹션 |  |
| `eipcCls` | 클래스 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `designClassInfoList` |  |  |
| `designClassInfo` |  |  |
| `eipcCls` | 디자인클래스 |  |
| `eipcSec` | 디자인섹션 |  |
| `eipcGro` | 디자인그룹 |  |
| `eipcDesc` | 디자인형태분류코드설명 |  |

---

## 형태분류(그룹조회)
`getShapeGroupInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `eipcSec` | 섹션 |  |
| `eipcCls` | 클래스 |  |
| `eipcGro` | 그룹 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `designShapeGroupInfoList` |  |  |
| `designShapeGroupInfo` |  |  |
| `eipcSec` | 디자인섹션 |  |
| `eipcCls` | 디자인클래스 |  |
| `eipcGro` | 디자인그룹 |  |
| `eipcShp` | 디자인형태분류 |  |
| `eipcMain` | 디자인형태분류코드 |  |
| `eipcDesc` | 디자인형태분류코드설명 |  |
| `uciFlag` | UCI코드존재유무 | (Y : 존재 N: 미정) |
| `kadoUrl` | 유통시스템URL |  |

---

## 형태분류(코드조회)
`getShapeCodeInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `eipcMain` | 디자인형태분류코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `totalSearchCount` | 전체건수 |  |
| `designShapeGroupInfoList` |  |  |
| `designShapeGroupInfo` |  |  |
| `eipcMain` | 디자인형태분류코드 |  |
| `eipcDesc` | 디자인형태분류코드설명 |  |
| `kadoUrl` | 유통시스템URL |  |
| `eipcCount` | 건수 |  |

---

## 속보서비스
`getBreakingInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `date` | 속보일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `designBreakingInfoList` |  |  |
| `designBreakingInfo` |  |  |
| `applicationName` | 출원인 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `title` | 디자인물품명칭 |  |

---

## 최종변동일자

- **분류**: 부가기능
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

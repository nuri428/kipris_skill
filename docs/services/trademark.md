# 상표 출원 속보

- **API 유형**: REST
- **오퍼레이션 수**: 54개 (구현: 0, 폐기예정: 2)
- **서비스 경로**: `trademarkInfoSearchService` ⚠️ 미검증
- **게이트웨이**: OpenAPI (`/openapi/rest/`) + KIPO API (`/kipo-api/kipi/`) — 오퍼레이션별 상이 (추정)

---

## 단어(폐기예정)
`getWordSearch`

- **분류**: 일반검색
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `articleName` | 물품명칭 | (물품명칭, 출원인, 창작자 및 창작자 주소) |
| `searchYearRange` | 검색년도범위 | (0:전체, 최근 1~10년) |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `indexNo` | 번호 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 출원공고번호 |  |
| `publicationDate` | 출원공고일자 |  |
| `registrationPublicNumber` | 등록공고번호 |  |
| `registrationPublicDate` | 등록공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `applicationStatus` | 출원상태 |  |
| `classificationCode` | 상품분류코드 |  |
| `viennaCode` | 도형코드 | 비엔나 |
| `applicantName` | 출원인명/특허고객번호 |  |
| `agentName` | 대리인명/대리인번호 |  |
| `regPrivilegeName` | 등록권자명/특허고객번호 |  |
| `title` | 상표명칭 |  |
| `fullText` | 전문존재유무 |  |
| `drawing` | 이미지경로 |  |
| `bigDrawing` | 큰이미지경로 |  |
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
| `searchNumber` | 출원번호/공고번호/등록번호 | 공고번호등록번호 |
| `searchYear` | 검색년도범위 |  |
| `searchRight` | 검색권리 |  |
| `pageNo` | 페이지번호 | (검색 페이지 번호) |
| `numOfRows` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `item` | 전체건수 |  |
| `agentName` | 대리인명 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicantName` | 출원인명 |  |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationStatus` | 법적상태 |  |
| `BigDrawing` | 큰이미지경로 |  |
| `classificationCode` | 상품분류코드 |  |
| `drawing` | 이미지경로 |  |
| `fullText` | 전문존재유무 |  |
| `indexNo` | 번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `publicationDate` | 출원공고일자 |  |
| `publicationNumber` | 출원공고번호 |  |
| `regPrivilegeName` | 등록권자명/특허고객번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationPublicDate` | 등록공고일자 |  |
| `registrationPublicNumber` | 등록공고번호 |  |
| `title` | 상표명칭 |  |
| `viennaCode` | 도형코드 | 비엔나 |
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
| `trademarkName` | 상표명칭 | (TN) |
| `trademarkNameMatch` | 상표명칭완전일치 | (TNM) |
| `classification` | 상품분류코드 | (TC) |
| `asignProduct` | 지정상품 | (GD) |
| `applicationNumber` | 출원번호 | (AN) |
| `registerNumber` | 등록번호 | (RN) |
| `publicationNumber` | 출원공고번호 | (PN) |
| `registrationPublicNumber` | 등록공고번호 | (RPN) |
| `internationalRegisterNumber` | 국제등록번호 | (MN) |
| `priorityNumber` | 우선권주장번호 | (PRN) |
| `applicationDate` | 출원일자 | (AD) |
| `registerDate` | 등록일자 | (RD) |
| `publicationDate` | 출원공고일자 | (PD) |
| `registrationPublicDate` | 등록공고일자 | (RPD) |
| `internationalRegisterDate` | 국제등록일자 | (MD) |
| `priorityDate` | 우선권주장일자 | (PRD) |
| `applicantName` | 출원인명/특허고객번호 | 출원인(AP)/코드 |
| `agentName` | 대리인명/대리인번호 | 대리인(AG)/코드 |
| `regPrivilegeName` | 등록권자 | (RG) |
| `viennaCode` | 도형코드 | DR 비엔나 |
| `freeSearch` | 자유검색 | (자유검색) |
| `similarityCode` | 유사군코드 |  |
| `application` | 출원 | 필수값(포함 : true, 미포함 : false) |
| `registration` | 등록 | 필수값(포함 : true, 미포함 : false) |
| `refused` | 거절 | 필수값(포함 : true, 미포함 : false) |
| `expiration` | 소멸 | 필수값(포함 : true, 미포함 : false) |
| `withdrawal` | 취하 | 필수값(포함 : true, 미포함 : false) |
| `publication` | 공고 | 필수값(포함 : true, 미포함 : false) |
| `cancel` | 무효 | 필수값(포함 : true, 미포함 : false) |
| `abandonment` | 포기 | 필수값(포함 : true, 미포함 : false) |
| `trademark` | 상표 | -40 |
| `serviceMark` | 서비스표 | -41 |
| `trademarkServiceMark` | 상표/서비스표 | -45 |
| `businessEmblem` | 업무표장 | -42 |
| `collectiveMark` | 단체표장 | -43 |
| `geoOrgMark` | 지리적표시단체표장 | -44 |
| `internationalMark` | 국제등록상표 | (마드리드) |
| `certMark` | 증명표장 | -47 |
| `geoCertMark` | 지리적증명표장 | -48 |
| `character` | 문자상표 | 필수값(포함 : true, 미포함 : false) |
| `figure` | 도형상표 | 필수값(포함 : true, 미포함 : false) |
| `compositionCharacter` | 복합문자 | 필수값(포함 : true, 미포함 : false) |
| `figureComposition` | 도형복합 | 필수값(포함 : true, 미포함 : false) |
| `sound` | 소리상표 | 필수값(포함 : true, 미포함 : false) |
| `fragrance` | 냄새상표 | 필수값(포함 : true, 미포함 : false) |
| `color` | 색채상표 | 필수값(포함 : true, 미포함 : false) |
| `dimension` | 입체상표 | 필수값(포함 : true, 미포함 : false) |
| `colorMixed` | 색채복합 | 필수값(포함 : true, 미포함 : false) |
| `hologram` | 홀로그램 | 필수값(포함 : true, 미포함 : false) |
| `motion` | 동작상표 | 필수값(포함 : true, 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | 필수값(포함 : true, 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | 필수값(포함 : true, 미포함 : false) |
| `pageNo` | 페이지번호 |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortSpec` | 정렬기준 |  |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `indexNo` | 번호 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 출원공고번호 |  |
| `publicationDate` | 출원공고일자 |  |
| `registrationPublicNumber` | 등록공고번호 |  |
| `registrationPublicDate` | 등록공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `priorityNumber` | 우선권주장번호 |  |
| `priorityDate` | 우선권주장일자 |  |
| `applicationStatus` | 출원상태 |  |
| `classificationCode` | 상품분류코드 |  |
| `viennaCode` | 도형코드 | 비엔나 |
| `applicantName` | 출원인명/특허고개번호 |  |
| `agentName` | 대리인명/대리인번호 |  |
| `regPrivilegeName` | 등록권자명/특허고객번호 |  |
| `title` | 상표명칭 |  |
| `fullText` | 전문존재유무 |  |
| `drawing` | 이미지경로 |  |
| `bigDrawing` | 큰이미지경로 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `count` |  |  |
| `numOfRows` | 페이지당건수 | (기본 : 30, 최대 500) |
| `pageNo` | 페이지번호 |  |
| `totalCount` | 전체건수 |  |

---

## 자유검색
`freeSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `word` | 자유검색 |  |
| `application` | 출원 | 필수값(포함 : true, 미포함 : false) |
| `registration` | 등록 | 필수값(포함 : true, 미포함 : false) |
| `refused` | 거절 | 필수값(포함 : true, 미포함 : false) |
| `expiration` | 소멸 | 필수값(포함 : true, 미포함 : false) |
| `withdrawal` | 취하 | 필수값(포함 : true, 미포함 : false) |
| `publication` | 공고 | 필수값(포함 : true, 미포함 : false) |
| `cancel` | 무효 | 필수값(포함 : true, 미포함 : false) |
| `abandonment` | 포기 | 필수값(포함 : true, 미포함 : false) |
| `trademark` | 상표 | -40 |
| `serviceMark` | 서비스표 | -41 |
| `trademarkServiceMark` | 상표/서비스표 | -45 |
| `businessEmblem` | 업무표장 | -42 |
| `collectiveMark` | 단체표장 | -43 |
| `geoOrgMark` | 지리적표시단체표장 | -44 |
| `internationalMark` | 국제등록상표 | (마드리드) |
| `certMark` | 증명표장 | -47 |
| `geoCertMark` | 지리적증명표장 | -48 |
| `character` | 문자상표 | 필수값(포함 : true, 미포함 : false) |
| `figure` | 도형상표 | 필수값(포함 : true, 미포함 : false) |
| `compositionCharacter` | 복합문자 | 필수값(포함 : true, 미포함 : false) |
| `figureComposition` | 도형복합 | 필수값(포함 : true, 미포함 : false) |
| `sound` | 소리상표 | 필수값(포함 : true, 미포함 : false) |
| `fragrance` | 냄새상표 | 필수값(포함 : true, 미포함 : false) |
| `color` | 색채상표 | 필수값(포함 : true, 미포함 : false) |
| `dimension` | 입체상표 | 필수값(포함 : true, 미포함 : false) |
| `colorMixed` | 색채복합 | 필수값(포함 : true, 미포함 : false) |
| `hologram` | 홀로그램 | 필수값(포함 : true, 미포함 : false) |
| `motion` | 동작상표 | 필수값(포함 : true, 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | 필수값(포함 : true, 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | 필수값(포함 : true, 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |
| `sortSpec` | 정렬기준 | (PD-공고일자, AD-출원일자, GD-등록일자, OPD-공개일자, FD-국제출원일자, FOD-국제공개일자, RD-우선권주장일자) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 | 비엔나 |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 출원번호 검색
`applicationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |
| `application` | 출원 | 필수값(포함 : true, 미포함 : false) |
| `registration` | 등록 | 필수값(포함 : true, 미포함 : false) |
| `refused` | 거절 | 필수값(포함 : true, 미포함 : false) |
| `expiration` | 소멸 | 필수값(포함 : true, 미포함 : false) |
| `withdrawal` | 취하 | 필수값(포함 : true, 미포함 : false) |
| `publication` | 공고 | 필수값(포함 : true, 미포함 : false) |
| `cancel` | 무효 | 필수값(포함 : true, 미포함 : false) |
| `abandonment` | 포기 | 필수값(포함 : true, 미포함 : false) |
| `trademark` | 상표 | -40 |
| `serviceMark` | 서비스표 | -41 |
| `trademarkServiceMark` | 상표/서비스표 | -45 |
| `businessEmblem` | 업무표장 | -42 |
| `collectiveMark` | 단체표장 | -43 |
| `geoOrgMark` | 지리적표시단체표장 | -44 |
| `internationalMark` | 국제등록상표 | (마드리드) |
| `certMark` | 증명표장 | -47 |
| `geoCertMark` | 지리적증명표장 | -48 |
| `character` | 문자상표 | 필수값(포함 : true, 미포함 : false) |
| `figure` | 도형상표 | 필수값(포함 : true, 미포함 : false) |
| `compositionCharacter` | 복합문자 | 필수값(포함 : true, 미포함 : false) |
| `figureComposition` | 도형복합 | 필수값(포함 : true, 미포함 : false) |
| `sound` | 소리상표 | 필수값(포함 : true, 미포함 : false) |
| `fragrance` | 냄새상표 | 필수값(포함 : true, 미포함 : false) |
| `color` | 색채상표 | 필수값(포함 : true, 미포함 : false) |
| `dimension` | 입체상표 | 필수값(포함 : true, 미포함 : false) |
| `colorMixed` | 색채복합 | 필수값(포함 : true, 미포함 : false) |
| `hologram` | 홀로그램 | 필수값(포함 : true, 미포함 : false) |
| `motion` | 동작상표 | 필수값(포함 : true, 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | 필수값(포함 : true, 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | 필수값(포함 : true, 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |
| `sortSpec` | 정렬기준 | (PD-공고일자, AD-출원일자, GD-등록일자, OPD-공개일자, FD-국제출원일자, FOD-국제공개일자, RD-우선권주장일자) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 | 비엔나 |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 상표명완전일치 검색
`trademarkNameMatchSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkNameMatch` | 상표명 |  |
| `application` | 출원 | 필수값(포함 : true, 미포함 : false) |
| `registration` | 등록 | 필수값(포함 : true, 미포함 : false) |
| `refused` | 거절 | 필수값(포함 : true, 미포함 : false) |
| `expiration` | 소멸 | 필수값(포함 : true, 미포함 : false) |
| `withdrawal` | 취하 | 필수값(포함 : true, 미포함 : false) |
| `publication` | 공고 | 필수값(포함 : true, 미포함 : false) |
| `cancel` | 무효 | 필수값(포함 : true, 미포함 : false) |
| `abandonment` | 포기 | 필수값(포함 : true, 미포함 : false) |
| `trademark` | 상표 | -40 |
| `serviceMark` | 서비스표 | -41 |
| `trademarkServiceMark` | 상표/서비스표 | -45 |
| `businessEmblem` | 업무표장 | -42 |
| `collectiveMark` | 단체표장 | -43 |
| `geoOrgMark` | 지리적표시단체표장 | -44 |
| `internationalMark` | 국제등록상표 | (마드리드) |
| `certMark` | 증명표장 | -47 |
| `geoCertMark` | 지리적증명표장 | -48 |
| `character` | 문자상표 | 필수값(포함 : true, 미포함 : false) |
| `figure` | 도형상표 | 필수값(포함 : true, 미포함 : false) |
| `compositionCharacter` | 복합문자 | 필수값(포함 : true, 미포함 : false) |
| `figureComposition` | 도형복합 | 필수값(포함 : true, 미포함 : false) |
| `sound` | 소리상표 | 필수값(포함 : true, 미포함 : false) |
| `fragrance` | 냄새상표 | 필수값(포함 : true, 미포함 : false) |
| `color` | 색채상표 | 필수값(포함 : true, 미포함 : false) |
| `dimension` | 입체상표 | 필수값(포함 : true, 미포함 : false) |
| `colorMixed` | 색채복합 | 필수값(포함 : true, 미포함 : false) |
| `hologram` | 홀로그램 | 필수값(포함 : true, 미포함 : false) |
| `motion` | 동작상표 | 필수값(포함 : true, 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | 필수값(포함 : true, 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | 필수값(포함 : true, 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `descSort` | 정렬방식 | (asc방식 : false, desc방식 : true) |
| `sortSpec` | 정렬기준 | (PD-공고일자, AD-출원일자, GD-등록일자, OPD-공개일자, FD-국제출원일자, FOD-국제공개일자, RD-우선권주장일자) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 | 비엔나 |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 상표명칭
`trademarkNameSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkName` | 상표명칭 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 상품분류
`classsificationSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `classification` | 상품분류코드 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 지정상품
`designatedGoodsSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `asignProduct` | 지정상품 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 등록번호
`registerNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registerNumber` | 등록번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 출원공고번호
`publicationNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `publicationNumber` | 출원공고번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 국제등록번호
`internationalRegisterNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `internationalRegisterNumber` | 국제등록번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 우선권주장번호
`priorityNumberSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityNumber` | 우선권주장번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 출원일자
`applicationDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationDate` | 출원일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 등록일자
`registerDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registerDate` | 등록일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 출원공고일자
`publicationDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `publicationDate` | 출원공고일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 국제등록일자
`internationalRegisterDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `internationalRegisterDate` | 국제등록일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 우선권주장일자
`priorityDateSearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityDate` | 우선권주장일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 출원인명/특허고객번호
`applicantNamesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantName` | 출원인명/특허고객번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 대리인이름/번호
`agentNamesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `agentName` | 대리인명/대리인번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 등록권자이름
`regPrivilegeNamesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `regPrivilegeName` | 등록권자명 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 도형코드
`viennaCodesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `viennaCode` | 도형코드 | 비엔나 |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 유사군
`similarityCodesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `similarityCode` | 유사군코드 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 등록공고번호
`registrationPublicNumbersearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationPublicNumber` | 등록공고번호 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

---

## 등록공고일자
`registrationPublicDatesearchInfo`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationPublicDate` | 등록공고일자 |  |
| `abandonment` | 포기 | (포함 : true 미포함 : false) |
| `application` | 출원 | (포함 : true 미포함 : false) |
| `cancel` | 무효 | (포함 : true 미포함 : false) |
| `expiration` | 소멸 | (포함 : true 미포함 : false) |
| `publication` | 공고 | (포함 : true 미포함 : false) |
| `refused` | 거절 | (포함 : true 미포함 : false) |
| `registration` | 등록 | (포함 : true 미포함 : false) |
| `withdrawal` | 취하 | (포함 : true 미포함 : false) |
| `businessEmblem` | 업무표장 | (42)(포함 : true 미포함 : false) |
| `certMark` | 증명표장 | (47)(포함 : true 미포함 : false) |
| `collectiveMark` | 단체표장 | (43)(포함 : true 미포함 : false) |
| `geoCertMark` | 지리적증명표장 | (48)(포함 : true 미포함 : false) |
| `geoOrgMark` | 지리적표시단체표장 | (44)(포함 : true 미포함 : false) |
| `internationalMark` | 국제등록상표 | (마드리드)(포함 : true 미포함 : false) |
| `serviceMark` | 서비스표 | (41)(포함 : true 미포함 : false) |
| `trademark` | 상표 | (40)(포함 : true 미포함 : false) |
| `trademarkServiceMark` | 상표/서비스표 | (45)(포함 : true 미포함 : false) |
| `character` | 문자상표 | (포함 : true 미포함 : false) |
| `compositionCharacter` | 복합문자 | (포함 : true 미포함 : false) |
| `figure` | 도형상표 | (포함 : true 미포함 : false) |
| `figureComposition` | 도형복합 | (포함 : true 미포함 : false) |
| `fragrance` | 냄새상표 | (포함 : true 미포함 : false) |
| `sound` | 소리상표 | (포함 : true 미포함 : false) |
| `color` | 색채상표 | (포함 : true 미포함 : false) |
| `colorMixed` | 색채복합 | (포함 : true 미포함 : false) |
| `dimension` | 입체상표 | (포함 : true 미포함 : false) |
| `hologram` | 홀로그램 | (포함 : true 미포함 : false) |
| `invisible` | 기타시각적으로인식불가능 | (포함 : true 미포함 : false) |
| `motion` | 동작상표 | (포함 : true 미포함 : false) |
| `visual` | 기타시각적으로인식가능 | (포함 : true 미포함 : false) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30 최대 500) |
| `sortSpec` | 정렬기준 | (AD-출원일자 RD-등록일자 PD-공고일자 MD-국제등록일자 PRD-우선권주장일자) |
| `descSort` | 정렬방식 | (asc방식 : false desc방식 : true) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `TotalSearchCount` | 전체건수 |  |
| `TradeMarkInfo` |  |  |
| `SerialNumber` | 일련번호 |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 출원공고번호 |  |
| `PublicDate` | 출원공고일자 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `PriorityClaimNumber` | 우선권주장번호 |  |
| `PriorityClaimDate` | 우선권주장일자 |  |
| `ApplicationStatus` | 출원상태 |  |
| `GoodClassificationCode` | 상품분류코드 |  |
| `ViennaCode` | 도형코드 |  |
| `ApplicantName` | 출원인명 |  |
| `AgentName` | 대리인명 |  |
| `RegistrationRightholderName` | 등록권리자명 |  |
| `Title` | 상표명칭 |  |
| `FulltextExistFlag` | 전문존재유무 |  |
| `ImagePath` | 큰이미지경로 |  |
| `ThumbnailPath` | 이미지경로 |  |

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
| `administrativeMeasureInfoArray` |  |  |
| `administrativeMeasureInfo` |  |  |
| `processStateCode` | 처리상태코드 |  |
| `receiptSendDate` | 접수발송일자 |  |
| `receiptSendDocumentEngName` | 접수발송서류영문명 |  |
| `receiptSendDocumentName` | 접수발송서류명 |  |
| `receiptSendNumber` | 접수발송번호 |  |
| `seq` | 처리순서 | (번호) |
| `agentInfoArray` |  |  |
| `agentInfo` |  |  |
| `agentAddress` | 대리인주소 |  |
| `agentCode` | 대리인번호 |  |
| `nameKoreanLong` | 대리인이름 | 한글 |
| `nationalCode` | 대리인국적코드 |  |
| `seq` | 처리순서 |  |
| `applicantInfoArray` |  |  |
| `applicantInfo` |  |  |
| `applicantAddress` | 출원인주소 |  |
| `applicantCode` | 특허고객번호 |  |
| `nameKoreanLong` | 출원인이름 | 한글 |
| `nationalCode` | 출원인국적코드 |  |
| `seq` | 처리순서 |  |
| `applicationNumberInfoArray` |  |  |
| `applicationNumberInfo` |  |  |
| `relatedApplicationDate` | 관련출원일자 |  |
| `relatedApplicationNumber` | 관련출원번호 |  |
| `asignProductArray` |  |  |
| `asignProduct` |  |  |
| `mainCode` | 상품분류코드 |  |
| `productName` | 지정상품명 | 한글 |
| `productNameEng` | 지정상품명 | 영문 |
| `seq` | 지정상품일련번호 |  |
| `subCode` | 유사군코드 |  |
| `biblioSummaryInfoArray` |  |  |
| `biblioSummaryInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationDate` | 출원일자 |  |
| `applicationNumber` | 출원번호 |  |
| `classVersion` | 상품분류버전 |  |
| `designateDate` | 사후지정일자 |  |
| `familyFlag` | 관련출원번호(패밀리)유무 |  |
| `imageFlag` | 견본이미지유무 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `lastDisposalCode` | 최종처분코드 |  |
| `lastDisposalDate` | 최종처분일자 |  |
| `originalApplicationFlag` | 원출원유무 |  |
| `priorityFlag` | 우선권주장유무 |  |
| `productName` | 상품의 명칭 |  |
| `productNameEng` | 상품의 명칭(영문) |  |
| `publicationDate` | 출원공고일자 |  |
| `publicationFlag` | 울원공고유무 |  |
| `publicationNumber` | 출원공고번호 |  |
| `rePublicationFlag` | 정정공보유무 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registerFlag` | 등록유무 |  |
| `registerStatus` | 등록상태 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationPublicDate` | 등록공고일자 |  |
| `registrationPublicGazetteFlag` | 등록공고공보유무 |  |
| `registrationPublicNumber` | 등록공고번호 |  |
| `retroDate` | 최종소급일자 |  |
| `retroDivisionCode` | 소급구분 |  |
| `tmDivisionCode` | 명칭구분코드 |  |
| `tmNameAcquisitionDate` | 상표명칭입수일자 |  |
| `trademarkDivisionCode` | 상표구분코드 |  |
| `trlFlag` | 심판청구유무 |  |
| `CoAgreementInfoArray` |  |  |
| `CoAgreementInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `inputDate` | 입력일자 |  |
| `registrationNumber` | 등록번호 |  |
| `seq` | 일련번호 |  |
| `originalApplicationIndicationArray` |  |  |
| `originalApplicationIndication` |  |  |
| `originalApplicationDate` | 원출원일자 |  |
| `originalApplicationNumber` | 원출원번호 |  |
| `partialRejectInfoArray` |  |  |
| `partialRejectInfo` |  |  |
| `mainCode` | 상품분류코드 |  |
| `productName` | 지정상품명 |  |
| `productNameEng` | 지정상품명 |  |
| `seq` | 지정상품일련번호 |  |
| `subCode` | 유사군코드 |  |
| `priorityClaimInfoArray` |  |  |
| `priorityClaimInfo` |  |  |
| `priorityApplicationCountry` | 우선권주장국가 |  |
| `priorityApplicationDate` | 우선권주장일자 |  |
| `priorityApplicationNumber` | 우선권주장번호 |  |
| `revisionPublicationInfoArray` |  |  |
| `revisionPublicationInfo` |  |  |
| `number` | 순번 |  |
| `openingPublicTypeCodeName` | 공고종류 | 출원정정공고, 등록정정공고 |
| `path` | 파일경로 |  |
| `pdfName` | 파일명 |  |
| `publicationDate` | 발간일자 |  |
| `sampleImageInfoArray` |  |  |
| `sampleImageInfo` |  |  |
| `imageName` | 이미지명 |  |
| `path` | 큰이미지경로 |  |
| `smallPath` | 이미지경로 |  |
| `similarityCodeInfoArray` |  |  |
| `similarityCodeInfo` |  |  |
| `similarCode` | 유사군코드 |  |
| `vfersionInfoArray` |  |  |
| `vfersionInfo` |  |  |
| `cd` | 국제분류정보 | NICE |
| `enNm` | 국제분류명 | NICE분류명(영문) |
| `koNm` | 국제분류명 | NICE분류명(한글) |
| `ver` | 국제분류버전 |  |
| `viennaCodeInfoArray` |  |  |
| `viennaCodeInfo` |  |  |
| `rowNumber` | 번호 |  |
| `viennaCode` | 도형분류코드 | 비엔나코드 |
| `viennaCodeDescription` | 도형분류코드설명 | 비엔나코드 |
| `publicationInfoArray` |  |  |
| `publicationInfo` |  |  |
| `path` | 파일경로 |  |
| `pdfName` | 파일명 |  |

---

## 지정상품정보
`trademarkDesignationGoodstInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkDesignationGoodstInfo` |  |  |
| `DesignationGoodsSerialNumber` | 지정상품일련번호 |  |
| `DesignationGoodsClassificationInformationCode` | 지정상품분류정보코드 |  |
| `SimilargroupCode` | 유사군코드 |  |
| `DesignationGoodsHangeulName` | 지정상품한글명 |  |
| `DesignationGoodsEnglishsentenceName` | 지정상품영문명 |  |
| `partialRejectInfoArray` |  |  |
| `partialRejectInfo` |  |  |
| `DesignationGoodsSerialNumber` | 지정상품일련번호 |  |
| `DesignationGoodsClassificationInformationCode` | 지정상품분류정보코드 |  |
| `SimilargroupCode` | 유사군코드 |  |
| `DesignationGoodsHangeulName` | 지정상품한글명 |  |
| `DesignationGoodsEnglishsentenceName` | 지정상품영문명 |  |

---

## 유사군코드
`trademarkSimilarityCodeInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkSimilarityCodeInfo` |  |  |
| `SimilargroupCode` | 유사군코드 |  |

---

## 서지요약정보
`trademarkBiblioSummaryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkBiblioSummaryInfo` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `AppReferenceNumber` | 출원참조번호 |  |
| `ApplicationDate` | 출원일자 |  |
| `PublicNumber` | 공고번호 |  |
| `PublicDate` | 공고일자 |  |
| `RegistrationNumber` | 등록번호 |  |
| `RegReferenceNumber` | 등록참조번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `TrademarkHangeulName` | 상표한글명 |  |
| `TrademarkEnglishsentenceName` | 상표영문명 |  |
| `LastDispositionCodeName` | 심사진행상태 |  |
| `LastDispositionDate` | 심사진행일자 |  |
| `TrademarkTypeCode` | 상표유형코드 |  |
| `ClassVersion` | 클래스버전 |  |
| `TrademarkNameAcquisitionDate` | 상표명칭취득일자 |  |
| `TrademarkKindCodeName` | 상표종류코드명 |  |
| `ImageFlag` | 이미지유무 |  |
| `PublicGazetteFlag` | 공고공보유무 |  |
| `UpdateGazetteFlag` | 정정공보유무 |  |
| `OriginalApplicationFlag` | 원출원유무 |  |
| `RegistrationFlag` | 등록유무 |  |
| `RelationApplicationNumberFlag` | 관련출원번호유무 |  |
| `PriorityClaimYesorno` | 우선권주장여부 |  |
| `MadridInternationalRegistrationNumber` | 마드리드국제등록번호 |  |
| `MadridInternationalRegistrationDate` | 마드리드국제등록일자 |  |
| `MadridAfterfactDesignationDate` | 마드리드사후지정일자 |  |
| `LastRetroactiveTypeCodeName` | 최종소급구분코드명 |  |
| `LastRetroactiveDate` | 최종소급일자 |  |
| `TrialDemandFlag` | 심판청구유무 |  |
| `RegistrationStatusCodeName` | 법적상태 |  |
| `RegistrationPublicGazetteFlag` | 등록공고공보유무 |  |
| `RegistrationPublicNumber` | 등록공고번호 |  |
| `RegistrationPublicDate` | 등록공고일자 |  |
| `ApplicationGazetteCancellationHistoryFlag` | 출원공보취소이력유무 | (데이터미제공) |

---

## 원출원번호정보
`trademarkOriginalApplicationIndicationInfo`

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
| `trademarkOriginalApplicationIndicationInfo` |  |  |
| `originalApplicationNumber` | 원출원등록번호 |  |
| `originalApplicationDate` | 원출원등록일자 |  |

---

## 비엔나도형분류코드정보
`trademarkViennaCodeInfo`

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
| `trademarkViennaCodeInfo` |  |  |
| `rowNumber` | 번호 |  |
| `viennaCode` | 비엔나코드 |  |
| `viennaCodeDescription` | 비엔나코드설명 |  |

---

## 상품분류 정보
`trademarkVfersionInfo`

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
| `trademarkAdministrativeMeasureInfo` |  |  |
| `ver` | 상품분류버젼 |  |
| `cd` | 상품분류코드 |  |
| `koNm` | 상품분류명 | 한글 |
| `enNm` | 상품분류명 | 영문 |

---

## 관련출원번호(패밀리)정보
`trademarkApplicationNumberInfo`

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
| `trademarkApplicationNumberInfo` |  |  |
| `relatedApplicationDate` | 관련출원일자 |  |
| `relatedApplicationNumber` | 관련출원번호 |  |

---

## 행정처분사항 번호
`trademarkAdministrativeMeasureInfo`

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
| `trademarkAdministrativeMeasureInfo` |  |  |
| `receiptSendNumber` | 접수발송번호 |  |
| `receiptSendDocumentName` | 접수발송서류명 | 한글 |
| `receiptSendDocumentEngName` | 접수발송서류명 | (영문) |
| `receiptSendDate` | 접수발송일자 |  |
| `processStateCode` | 처리상태코드 |  |
| `seq` | 처리순서 | (번호) |

---

## 대리인
`trademarkAgentInfo`

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
| `trademarkAgentInfo` |  |  |
| `nameKoreanLong` | 대리인명 |  |
| `agentAddress` | 대리인주소 |  |
| `nationalCode` | 대리인국가 |  |
| `agentCode` | 대리인번호 |  |
| `seq` | 처리순서 |  |

---

## 출원인
`trademarkApplicantInfo`

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
| `trademarkApplicantInfo` |  |  |
| `nameKoreanLong` | 출원인명 |  |
| `applicantAddress` | 출원인주소 |  |
| `nationalCode` | 출원인국가 |  |
| `applicantCode` | 특허고객번호 |  |
| `seq` | 처리순서 |  |

---

## 변경 상표정보의 출원번호 제공
`trademarkApplicationNumberByModifiedDateInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변경날짜 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trademarkApplicationNumberByModifiedDateInfo` |  |  |
| `modifiedApplicationNumber` | 출원번호 |  |

---

## 변경 정보의 서지요약정보 제공
`trademarkBiblioSummaryByModifedDateInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변경날짜 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trademarkBiblioSummaryByModifedDateInfo` |  |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 출원공고번호 |  |
| `publicationDate` | 출원공고일자 |  |
| `registrationNumber` | 등록번호 |  |
| `registrationDate` | 등록일자 |  |
| `productName` | 상품의명칭 |  |
| `productNameEng` | 상품의명칭 |  |
| `lastDisposalCode` | 심사진행상태 |  |
| `lastDisposalDate` | 심사진행일자 |  |
| `trademarkDivisionCode` | 상표구분코드 |  |
| `classVersion` | 서브코드 |  |
| `imageFlag` | 견본이미지유무 |  |
| `publicationFlag` | 출원공고공보유무 |  |
| `rePublicationFlag` | 정정공보유무 |  |
| `originalApplicationFlag` | 원출원유무 |  |
| `trlFlag` | 심판청구유무 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registerFlag` | 등록여부 |  |
| `familyFlag` | 관련출원번호(패밀리)유무 |  |
| `priorityFlag` | 우선권주장유무 |  |
| `tmNameAcquisitionDate` | 상표명칭입수일자 |  |
| `internationalRegisterNumber` | 국제등록번호 |  |
| `retroDivisionCode` | 소급구분 |  |
| `retroDate` | 최종소급일자 |  |
| `internationalRegisterDate` | 국제등록일자 |  |
| `designateDate` | 사후지정일자 |  |
| `registerStatus` | 법적상태 |  |
| `tmDivisionCode` | 명칭구분코드 |  |
| `registrationPublicGazetteFlag` | 등록공고전문유무 |  |
| `registrationPublicNumber` | 등록공고번호 |  |
| `registrationPublicDate` | 등록공고일자 |  |

---

## 우선권주장번호
`trademarkpriorityNumberSearchInfo`

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
| `trademarkpriorityNumberSearchInfo` |  |  |
| `priorityApplicationCountry` | 우선권주장국가 |  |
| `priorityApplicationDate` | 우선권주장일자 |  |
| `priorityApplicationNumber` | 우선권주장번호 |  |

---

## 공존동의상표정보

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `CoAgreementInfoArray` |  |  |
| `CoAgreementInfo` |  |  |
| `seq` | 일련번호 |  |
| `registrationNumber` | 등록번호 |  |
| `applicationNumber` | 출원번호 |  |
| `inputDate` | 입력일자 |  |

---

## 견본이미지
`getSampleImageInfoSearch`

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
| `imageName` | 이미지명 |  |
| `path` | 큰이미지경로 |  |
| `smallPath` | 이미지경로 |  |

---

## 공고 전문
`getAnnFullTextInfoSearch`

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
| `pdfName` | 파일명 |  |
| `path` | 파일경로 |  |

---

## 정정공보
`trademarkRevisionPublicationInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `revisionPublicationInfo` |  |  |
| `number` | 번호 |  |
| `openingPublicTypeCodeName` | 공개공고구분코드명 |  |
| `path` | 파일경로 |  |
| `pdfName` | 파일명 |  |
| `publicationDate` | 공고일자 |  |

---

## 등록공고공보
`trademarkRegGazetteInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkRegGazetteInfo` |  |  |
| `path` | 파일경로 |  |
| `pdfName` | 파일명 |  |

---

## 모든 전문 및 견본 이미지 유무
`trademarkFullTextCheckInfo`

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
| `trademarkFullTextCheckInfo` |  |  |
| `publicationCheckResult` | 출원공고공보유무 | (있음:Y 없음:N) |
| `revisionPublicationCheckResult` | 정정공보유무 | (있음:Y 없음:N) |
| `registrationCheckResult` | 등록사항유무 | (있음:Y 없음:N) |
| `sampleImageCheckResult` | 견본이미지유무 | (있음:Y 없음:N) |
| `registrationPublicGazetteCheckResult` | 등록공고공보유무 | (있음:Y 없음:N) |

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
| `transListString` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 지정상품조회
`trademarkAsignProductSearchInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchWord` | 검색단어 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkAsignProductSearchInfo` |  |  |
| `version` | 버전 |  |
| `classsification` | 분류 |  |
| `productsNum` | 상품명 |  |
| `main` |  |  |
| `name` | 이름 |  |
| `engName` | 영문이름 |  |
| `productsDesc` |  |  |
| `simm` |  |  |

---

## 유사군코드 조회
`trademarkSimilarCodeSearchInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designatedGoodsName` | 지정상품명 |  |
| `similarCode` | 유사군코드 | (필수값) |
| `startNum` | 검색시작번호 |  |
| `endNum` | 검색카운트 | (최대 60건까지 조회가능) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `totalCount` | 전체건수 |  |
| `trademarkSimilarCodeSearchInfo` |  |  |
| `rowNumber` | 줄번호 |  |
| `niceCode` | 니스코드 |  |
| `niceClassCode` | 니스분류코드 |  |
| `version` | 버전 |  |
| `similarCode` | 유사군코드 |  |
| `asignProductName` | 지정상품명 |  |
| `asignProductNameEnglish` | 지정상품영문명 |  |

---

## 변동정보2
`trademarkTransferInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | (BIB-서지, BIB_NEW-서지_신규입수건, IMG-이미지, ORG-원출원, VIN-비엔나, PRI-우선권, PB-출원공고/등록공고, REPB-정정공고, AP-출원인, AG-대리인, DEL-삭제) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkTransferInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 도형 코드 조회
`trademarkSearchViennaCodeInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchWord` | 검색단어 |  |
| `sectionInfo` | 섹션번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trademarkFullTextCheckInfo` |  |  |
| `rowNumber` | 번호 |  |
| `viennaCode` | 비엔나코드 |  |
| `viennaCodeDescription` | 비엔나코드설명 |  |

---

## 상품분류 지정상품 초기 정보
`trademarkIntroInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `입력 값 없음` |  |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trademarkIntroInfo` |  |  |
| `ver` | 상품분류버젼 |  |
| `cd` | 상품분류코드 |  |
| `koNm` | 상품분류명 |  |
| `enNm` | 상품분류명 |  |

---

## 상품분류 설명(8-9판 분류대조표)
`trademarkGoodClassificationInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `입력 값 없음` |  |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `trademarkGoodClassificationInfo` |  |  |
| `korClssCd` | 한글분류코드 |  |
| `korClssGun` | 한글분류군 |  |
| `korDesc` | 한글분류코드설명 |  |
| `niceClssCd8` | 국제분류코드8 |  |
| `niceClss8Gun` | 국제분류군8 |  |
| `niceSgrCd8` | 국제SGR코드8 |  |
| `niceDesc8` | 국제분류코드설명8 |  |
| `niceClssCd9` | 국제분류코드9 |  |
| `niceSgrCd9` | 국제SGR코드9 |  |
| `niceDesc9` | 국제분류코드설명9 |  |
| `etc` | 기타 |  |

---

## 속보서비스
`trademarkBulletinAllListInfo`

- **분류**: 부가기능
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `firstLoadDate` | 속보일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `bulletinAllListInfo` |  |  |
| `titleKor` | 상표명칭 | 한글 |
| `titleEng` | 상표명칭 | 영문 |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원날짜 |  |
| `applicantName` | 출원인명 |  |

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

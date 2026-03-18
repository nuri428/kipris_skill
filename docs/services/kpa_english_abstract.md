# 한국특허영문초록(KPA)

- **API 유형**: REST
- **오퍼레이션 수**: 26개 (구현: 0, 폐기예정: 0)

---

## 자유
`anySearch`

- **분류**: 일반검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchAny` | 자유검색 | (ex : spring*IP=[G02C5/22]) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 단어
`wordSearch`

- **분류**: 일반검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchWord` | 검색단어 |  |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 이름
`nameSearch`

- **분류**: 일반검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchName` | 출원인명/발명자명 | (출원인, 발명자) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 번호
`numberSearch`

- **분류**: 일반검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchNumber` | 번호 | (번호) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 전체검색
`advancedSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `abstracts` | 초록 | AB |
| `applicant` | 출원인명 | AP |
| `applicationNo` | 출원번호 | EAN |
| `applicationdate` | 출원일자 | AD |
| `inventionName` | 발명의명칭 | TL |
| `inventors` | 발명자명 | IV |
| `ipc` | IPC코드 | EIP |
| `priorityNo` | 우선권주장번호 | PR |
| `registerDate` | 등록일자 | PD |
| `registerNo` | 등록번호 | EPN |
| `collectionValues` | 국가코드 | (KR:KPA) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortState` | 정렬방식 | (true-desc, false-asc) |
| `sortField` | 정렬기준 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## IPC
`ipcSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `ipc` | IPC코드 |  |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 발명의명칭
`inventionNameSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `invention` | 발명의명칭 | (발명의 명칭) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 초록정보
`abstractSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `abstracts` | 초록 | (초록) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 출원번호
`applicationNumberSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 | (출원번호) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 등록번호
`registerNumberSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registerNumber` | 등록번호 | (공개건의 경우는 공개번호) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 우선권번호
`priorityNumberSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityNumber` | 우선권주장번호 | (PR) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 출원일자
`applicationdateSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationdate` | 출원일자 | (출원일자) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |

---

## 등록일자
`registerDateSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registerDate` | 등록일자 | (공개건의 경우는 공개일자) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 출원인
`applicantSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicant` | 출원인명 | (출원인) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 발명자
`inventorsSearch`

- **분류**: 항목별검색
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `inventors` | 발명자명 | (발명자) |
| `currentPage` | 시작번호 | (index) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |
| `sortField` | 정렬기준 |  |
| `sortState` | 정렬방식 | (true-desc, false-asc) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchResult` |  |  |
| `applicant` | 출원인명 | (AP) |
| `applicationDate` | 출원일자 | (AD) |
| `applicationNo` | 출원번호 | (EAN) |
| `inventionName` | 발명의명칭 | (TL) |
| `inventors` | 발명자명 | (IV) |
| `ipc` | IPC코드 | (EIP) |
| `ltrtno` | 문헌번호 |  |
| `priorityDate` | 우선권주장일자 | (PY) |
| `priorityNo` | 우선권주장번호 | (PR) |
| `registerDate` | 등록일자 | (PD) |
| `registerNo` | 등록번호 | (EPN) |
| `colString` | 국가코드 | (KR:KPA) |
| `totalSearchCount` | 전체건수 |  |

---

## 서지상세정보
`bibliographicInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `bibliographicInfo` |  |  |
| `bibliographicSummaryInfo` |  |  |
| `inventionTitle` | 발명의명칭 |  |
| `usKind` | 번호종류 |  |
| `usNo` | 해당번호 |  |
| `patTpcd` | 국외문헌식별코드 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationDate` | 공개일자 |  |
| `publicationNumber` | 공개번호 |  |
| `issueDate` | 공고일자 |  |
| `registerNumber` | 등록번호 |  |
| `registerDate` | 등록일자 |  |
| `imageStandardCode` | 대표도면출처상태코드 | (S10301:존재, S10399:미존재) |
| `pubFg` | 공고공보유무 |  |
| `repubFg` | 정정공보유무 |  |
| `ipcInfo` |  |  |
| `ipcCd` | IPC코드 |  |
| `ipcVersion` | IPC버전 |  |
| `summation` |  |  |
| `astrtCont` | 요약 |  |
| `applicantInfo` |  |  |
| `applicantName` | 출원인명 |  |
| `applicantAddress` | 출원인주소 |  |
| `applicantCountry` | 출원인국가 |  |
| `inventorsInfo` |  |  |
| `inventorName` | 발명자명 |  |
| `inventorAddress` | 발명자주소 |  |
| `inventorCountry` | 발명자국가 |  |
| `legalStatusInfo` |  |  |
| `receiptNumber` | 접수번호 |  |
| `receiptDate` | 접수일자 |  |
| `documentName` | 서류명 |  |
| `commonCodeName` | 공통코드명 |  |

---

## 서지요약정보
`bibliographicSummaryInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `bibliographicSummaryInfo` |  |  |
| `inventionTitle` | 발명의명칭 |  |
| `usKind` | 번호종류 |  |
| `usNo` | 해당번호 |  |
| `patTpcd` | 국외문헌식별코드 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationDate` | 공개일자 |  |
| `publicationNumber` | 공개번호 |  |
| `issueDate` | 공고일자 |  |
| `registerNumber` | 등록번호 |  |
| `registerDate` | 등록일자 |  |
| `imageStandardCode` | 대표도면출처상태코드 | (S10301:존재, S10399:미존재) |
| `pubFg` | 공고공보유무 |  |
| `repubFg` | 정정공보유무 |  |

---

## IPC
`ipcInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `ipcInfo` |  |  |
| `ipcCd` | IPC코드 |  |
| `ipcVersion` | IPC버전 |  |

---

## 초록
`summation`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `summation` |  |  |
| `astrtCont` | 요약 |  |

---

## 출원인
`applicantInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicantInfo` |  |  |
| `applicantName` | 출원인명 |  |
| `applicantAddress` | 출원인주소 |  |
| `applicantCountry` | 출원인국가 |  |

---

## 발명자
`inventorsInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `inventorsInfo` |  |  |
| `inventorName` | 발명자명 |  |
| `inventorAddress` | 발명자주소 |  |
| `inventorCountry` | 발명자국가 |  |

---

## 우선권정보
`priorityNumberDateInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `priorityNumberDateInfo` |  |  |
| `priorityApplicationNumber` | 우선권주장번호 |  |
| `priorityApplicationDate` | 우선권주장일자 |  |
| `priorityApplicationCountry` | 우선권주장국가 |  |

---

## 인용문헌
`patentDocumentsInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `patentDocumentsInfo` |  |  |
| `corgPatno` | 인용문헌번호 |  |
| `patTpcd` | 인용문헌종류코드 |  |
| `exam` | 심사관인용여부 |  |
| `patDt` | 인용문헌공보일자 |  |
| `countryCode` | 인용문헌국가코드 |  |
| `clssCd` | 연계문헌번호 |  |

---

## 행정처리
`legalStatusInfo`

- **분류**: 서지정보
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `legalStatusInfo` |  |  |
| `receiptNumber` | 접수번호 |  |
| `receiptDate` | 접수일자 |  |
| `documentName` | 서류명 |  |
| `commonCodeName` | 공통코드명 |  |

---

## 도면/전문(대표도면)
`representationImageInfo`

- **분류**: 도면/전문
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `representationImageInfo` |  |  |
| `tifPath` | 이미지파일경로 |  |
| `tifFileName` | 이미지파일명 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | BIB-서지, IPC, AB-초록, AP-출원인, IN-발명자, PRI-우선권정보, DOC-인용문헌, ADM-행정처리 |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

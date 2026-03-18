# 분류코드

- **API 유형**: REST
- **오퍼레이션 수**: 8개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `ClassificationService` (포털 확인)
- **게이트웨이**: OpenAPI (`/openapi/rest/`)
- **인증 키**: `accessKey`

---

## IPC코드검색
`searchIPCInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `ipcNumber` | IPC코드/단어 | (IPC 코드 및 단어) |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `totalSearchCount` | 전체건수 |  |
| `getSearchIPCInfo` |  |  |
| `indexNo` | 인덱스번호 |  |
| `ipcNumber` | IPC코드 |  |
| `korDescription` | 한글설명 |  |
| `engDescription` | 영어설명 |  |

---

## 도형코드검색
`searchViennaCodeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchWord` | 검색단어 | (Vienna코드) |
| `sectionInfo` | 섹션번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `getSearchViennaCodeInfo` |  |  |
| `indexNumber` | 번호 |  |
| `viennaCode` | 비엔나코드 |  |
| `viennaCodeDescription` | 비엔나코드설명 |  |

---

## 디자인분류검색
`searchDesignCodeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designNumber` | 디자인분류코드/물품명칭 |  |
| `startNumber` | 시작번호 | (결과 출력 대상의 번호를 입력하여 해당 번홉부터 출력) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `totalSearchCount` | 전체건수 |  |
| `getSearchDesignCodeInfo` |  |  |
| `designNumber` | 디자인코드 |  |
| `designName` | 디자인물품명칭 |  |

---

## EPC코드검색
`searchEPCInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `codeNumber` | EPC코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `GetSearchEPCInfo` |  |  |
| `epcNumber` | EPC코드 |  |
| `korDescription` | 한글설명 |  |
| `engDescription` | 영문설명 |  |

---

## UPC코드검색
`searchUPCInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `codeNumber` | UPC코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `GetSearchUPCInfo` |  |  |
| `upcNumber` | UPC코드 |  |
| `korDescription` | 한글설명 |  |
| `engDescription` | 영문설명 |  |

---

## FI코드검색
`searchFIInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `codeNumber` | FI코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `GetSearchFIInfo` |  |  |
| `fiCode` | FI코드 |  |
| `korDescription` | 한글설명 |  |
| `engDescription` | 영문설명 |  |

---

## FTERM코드검색
`searchFTERMInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `codeNumber` | FTERM코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `GetSearchFTERMInfo` |  |  |
| `ftermCode` | FTERM코드 |  |
| `korDescription` | 한글설명 |  |
| `engDescription` | 영문설명 |  |

---

## CPC코드검색
`searchCPCInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `codeNumber` | CPC코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `getSearchCPCInfo` |  |  |
| `section` | CPC코드 |  |
| `koreanExplanation` | 한글설명 |  |
| `originalTextExplanation` | 영문설명 |  |

---

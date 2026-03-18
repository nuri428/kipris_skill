# 특허 패밀리

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)

---

## 특허패밀리정보조회(국내출원번호)
`getAppNoPatFamInfoSearch`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `Items` |  |  |
| `docdbFamilyID` | DOCDB패밀리ID |  |
| `applicationCountryCode` | DOCDB출원국가코드 |  |
| `applicationDate` | DOCDB출원일자 |  |
| `applicationKindCode` | DOCDB출원종류코드 |  |
| `applicationNumber` | DOCDB출원번호 |  |
| `publicationCountryCode` | DOCDB공보국가코드 |  |
| `publicationDate` | DOCDB공보일자 |  |
| `publicationKindCode` | DOCDB공보종류코드 |  |
| `publicationNumber` | DOCDB공보번호 |  |

---

## 패밀리정보조회(DOCDB공보번호)
`familyInfoSearchDOCPubNumber`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `gazetteNumber` | DOCDB공보번호 |  |
| `gazetteCountryCode` | DOCDB공보국가코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `familyInfoSearchDOCPubNumber` |  |  |
| `familyIdentification` | DOCDB패밀리ID |  |
| `applicationCountryCode` | DOCDB출원국가코드 |  |
| `applicationDate` | DOCDB출원일자 |  |
| `applicationKindCode` | DOCDB출원종류코드 |  |
| `applicationNumber` | DOCDB출원번호 |  |
| `gazetteCountryCode` | DOCDB공보국가코드 |  |
| `gazetteDate` | DOCDB공보일자 |  |
| `gazetteKindCode` | DOCDB공보종류코드 |  |
| `gazetteNumber` | DOCDB공보번호 |  |

---

## 패밀리정보조회(DOCDB출원번호)
`familyInfoSearchDOCAppNumber`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | DOCDB출원번호 |  |
| `applicationCountryCode` | DOCDB출원국가코드 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `familyInfoSearchDOCAppNumber` |  |  |
| `familyIdentification` | DOCDB패밀리ID |  |
| `applicationCountryCode` | DOCDB출원국가코드 |  |
| `applicationDate` | DOCDB출원일자 |  |
| `applicationKindCode` | DOCDB출원종류코드 |  |
| `applicationNumber` | DOCDB출원번호 |  |
| `gazetteCountryCode` | DOCDB공보국가코드 |  |
| `gazetteDate` | DOCDB공보일자 |  |
| `gazetteKindCode` | DOCDB공보종류코드 |  |
| `gazetteNumber` | DOCDB공보번호 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |
| `searchType` | 검색코드 | 기본-국내출원번호, DOCP-DOCDB공보번호, DOCA-DOCDB출원번호 |
| `searchCountry` | 검색국가 | US-미국, JP-일본, CP-중국, EP-유럽, WO-WIPO 등 |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : [기본]출원번호1&#124;출원번호2, [DOCP]DOCDB공보번호1&#124;DOCDB공보번호2, [DOCA]DOCDB출원번호1&#124;DOCDB출원번호2) |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | 기본-국내출원번호, DOCP-DOCDB공보번호, DOCA-DOCDB출원번호 |
| `searchCountry` | 국가코드 |  |
| `applicationNumber` | 출원번호 | 기본, DOCA 인 경우만 해당 |
| `gazetteNumber` | 공보번호 | DOCP인 경우만 해당 |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

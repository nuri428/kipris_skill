# 다인용 선행문헌

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 다인용 선행문헌 조회
`multiCitationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `start_citationDate` | 참증시작일자 | (필수) |
| `end_citationDate` | 참증종료일자 | (필수) |
| `ipcCode` | IPC코드 | (필수, LIKE검색지원) |
| `countryCode` | 국가코드 | AU-오스트레일리아, CA-캐나다, CH-스위스, CN-중국, DE-독일, EP-유럽특허청(EPO), FR-프랑스, GB-영국, JP-일본, KR-대한민국, PJ-일본영문초록, PL-폴란드, RU-러시아, US-미국, WO-WIPO |
| `documentNumber` | 출원번호/문헌번호 | (국내)출원번호, (해외)문헌번호 |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `multiCitationInfo` |  |  |
| `countryCode` | 국가코드 |  |
| `documentNumber` | 출원번호/문헌번호 | (국내)출원번호, (해외)문헌번호 |
| `citationDate` | 참증일자 |  |
| `ipcCode` | IPC코드 |  |
| `applicationDate` | 출원일자 |  |
| `inventionTitle` | 발명의명칭 |  |
| `citationCount` | 참증횟수 |  |
| `openDate` | 공개일자 |  |
| `openNumber` | 공개번호 |  |
| `registrationDate` | 등록일자 |  |
| `registrationNumber` | 등록번호 |  |
| `publicationDate` | 공고일자 |  |
| `publicationNumber` | 공고번호 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 변동리스트 | (국가코드,번호,참증일자,IPC) ※번호-(국내)출원번호, (해외)문헌번호 |

---
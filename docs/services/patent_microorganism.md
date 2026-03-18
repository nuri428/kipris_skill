# 특허 기탁 미생물

- **API 유형**: REST
- **오퍼레이션 수**: 4개 (구현: 0, 폐기예정: 1)

---

## 특허기탁미생물 기본조회(폐기예정)
`patentDepositionMicroorganismInfo`

- **분류**: 오퍼레이션
- **상태**: ⚠️ 폐기예정

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `PatentDepositionMicroorganism` |  |  |
| `ApplicationNumber` | 출원번호 |  |
| `MicroorganismDepositionSerialnumber` | 미생물수탁일련번호 |  |
| `MicroorganismDepositionNumber` | 미생물수탁번호 |  |
| `MicroorganismDepositionDate` | 미생물수탁일자 |  |
| `MicroorganismDepositionInstitution` | 미생물수탁기관 |  |

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
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 특허기탁미생물 기본조회 ver.2
`patentDepositionMicroorganismInfoV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `patentDepositionMicroorganismV2` |  |  |
| `applicationNumber` | 출원번호 |  |
| `microorganismDepositionNumber` | 수탁번호 |  |
| `microorganismDepositionDate` | 기탁일자 |  |
| `microorganismNm` | 미생물명 |  |
| `microorganismKindNm` | 미생물종류 |  |
| `depositoryInstitutionNm` | 기탁기관명 |  |
| `depositor` | 기탁자 |  |
| `microorganismDepositionMemo` | 기타사항 |  |
| `microorganismDepositionInKoreaYn` | 국내외기탁 | Y : 국내기탁, N : 국제기탁 |

---

## 특허기탁미생물 검색
`patentDepositionMicroorganismSearch`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `microorganismDpathNm` | 기탁기관 |  |
| `microorganismDepositionDate` | 기탁일자 | (입력 예시 : YYYYMMDD~YYYYMMDD) |
| `depositor` | 기탁자 |  |
| `microorganismNm` | 미생물명 |  |
| `microorganismSpno` | 수탁번호 |  |
| `microorganismKindNm` | 미생물종류 |  |
| `inventionTitle` | 발명의명칭 |  |
| `microorganismDepositionInKoreaYn` | 국내외기탁 | Y : 국내기탁, N : 국제기탁 |
| `mcdtbNm` | 분양자 |  |
| `mcdtbHistoryYN` | 분양이력여부 | Y : 분양(O), N : 분양(X) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `item` |  |  |
| `totalCount` | 전체건수 |  |
| `patentDepositionMicroorganismSearch` |  |  |
| `applicationNumber` | 출원번호 |  |
| `microorganismDepositionNumber` | 수탁번호 |  |
| `inventionTitle` | 발명의명칭 |  |
| `microorganismNm` | 미생물명 |  |
| `microorganismKindNm` | 미생물종류 |  |
| `microorganismDepositionDate` | 기탁일자 |  |
| `microorganismDpathNm` | 기탁기관 |  |
| `mcdtbHistoryYN` | 분양이력 |  |

---

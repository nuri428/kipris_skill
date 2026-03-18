# 일본 특허 합금조성비

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 5개 (구현: 0, 폐기예정: 0)

---

## 서지조회
`bibliographyInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `inputnumber` | 입력번호 |  |
| `inputnumberType` | 입력번호종류 | 문헌번호(LN), 표준출원번호(SAN), 표준공보번호(SGN),국제출원번호(IAN), 국외출원번호(OAN), 국외등록번호(ORN), 국외공개번호(OON), 국외공보번호(OGN) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `JapanAlloycompositionratioBibliographyInfoList` |  |  |
| `Literaturenumber` | 문헌번호 |  |
| `Serialnumber` | 일련번호 |  |
| `StandardApplicationnumber` | 표준출원번호 |  |
| `OutsidenationApplicationnumber` | 국외출원번호 |  |
| `OutsidenationApplicationDate` | 국외출원일자 |  |
| `OutsidenationRegistrationnumber` | 국외등록번호 |  |
| `OutsidenationRegistrationDate` | 국외등록일자 |  |
| `InternationalApplicationnumber` | 국제출원번호 |  |
| `InternationalApplicationDate` | 국제출원일자 |  |
| `OutsidenationLaid-Opennumber` | 국외공개번호 |  |
| `OutsidenationOpeningDate` | 국외공개일자 |  |
| `StandardGazettenumber` | 표준공보번호 |  |
| `OutsidenationGazettenumber` | 국외공보번호 |  |
| `OutsidenationGazetteDate` | 국외공보일자 |  |
| `OutsidenationTitleofinvention` | 국외발명의명칭 |  |

---

## 조성비조회
`basicInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `literaturenumber` | 문헌번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `JapanAlloycompositionratioBasicInfoList` |  |  |
| `Literaturenumber` | 문헌번호 |  |
| `Serialnumber` | 일련번호 |  |
| `PetitionclauseSerialnumber` | 청구항일련번호 |  |
| `CompositoinratioSerialnumber` | 조성비일련번호 |  |
| `ElementSymbolName` | 원소부호명 |  |
| `ElementHangeulName` | 원소한글명 |  |
| `ElementEnglishName` | 원소영문명 |  |
| `ElementMiniumPercentage` | 원소최소비율 |  |
| `ElementMaximumPercentage` | 원소최대비율 |  |
| `ElementUnitName` | 원소단위명 |  |
| `MainIngredientYn` | 주성분여부 |  |

---

## 청구항조회
`petitionclauseInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `literaturenumber` | 문헌번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `JapanAlloycompositionratioPetitionclauseInfoList` |  |  |
| `Literaturenumber` | 문헌번호 |  |
| `Serialnumber` | 일련번호 |  |
| `PetitionclauseSerialnumber` | 청구항일련번호 |  |
| `PetitionclauseDetailContent` | 청구항상세내용 |  |
| `CompositoinratioYn` | 조성비여부 |  |
| `DependentclaimNumberList` | 종속항번호목록 |  |

---

## IPC조회
`ipcInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `literaturenumber` | 문헌번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `JapanAlloycompositionratioIpcInfoList` |  |  |
| `Literaturenumber` | 문헌번호 |  |
| `Serialnumber` | 일련번호 |  |
| `ClassificationSerialnumber` | 분류일련번호 |  |
| `InternationalpatentclassificationCode` | IPC코드 |  |
| `ClassificationDate` | 분류일자 |  |
| `MainClassificationYn` | 주분류여부 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |
| `searchType` | 검색종류 | 서지(BIB), 조성비(BASIC), 청구항(PTCLS), IPC(IPC) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 문헌번호리스트 | (ex : 문헌번호?1&#124;문헌번호?2) |

---
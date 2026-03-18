# 특허권 존속기간 연장등록 공보

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 4개 (구현: 0, 폐기예정: 0)

---

## 기본정보
`extensionPatentGazetteInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `extensionPatentGazetteInfo` |  |  |
| `applicationnumber` | 출원번호 |  |
| `issueDate` | 발간일자 |  |
| `gazetteKind` | 공보종류 |  |
| `extensionApplicationNumber` | 연장출원번호 |  |
| `receiptNumber` | 접수번호 |  |
| `sendNumber` | 발송번호 |  |

---

## 부가정보
`extensionPatentGazetteAdditionalInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `extensionPatentGazetteAdditionalInfo` |  |  |
| `applicationnumber` | 출원번호 |  |
| `PermissionSerialnumber` | 허가일련번호 |  |
| `permissionDate` | 허가일자 |  |
| `permissionContent` | 허가내용 |  |
| `compoundName` | 화합물명칭 |  |
| `articleName` | 물품명칭 | 한글 |
| `articleEnglishName` | 물품명칭 | 영문 |
| `merchandiseName` | 상품명칭 | 한글 |
| `merchandiseEnglishName` | 상품명칭 | 영문 |
| `usageContent` | 용도내용 | 한글 |
| `usageEnglishContent` | 용도내용 | 영문 |

---

## 공보전문PDF
`extensionPatentGazettePdfInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `pdfInfo` |  |  |
| `gazetteKind` | 공보종류 |  |
| `sendNumber` | 발송번호 |  |
| `fileName` | 파일명 |  |
| `filePath` | 파일경로 |  |

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
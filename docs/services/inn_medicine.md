# 의약품 국제일반명칭

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## INN 기본조회
`basicINNInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `referenceevidenceNumber` | 참증번호 | (내부관리번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `INNInfo` |  |  |
| `ReferenceevidenceNumber` | 참증번호 |  |
| `ReferenceevidenceArticleEnglishName` | 참증물품영문명 |  |
| `FigureImageExistFlag` | 도형이미지존재유무 |  |
| `InternationalMedicineRequestNumber` | 국제의약품요청번호 |  |
| `InternationalMedicineLatinName` | 국제의약품라틴어명 |  |
| `InternationalMedicineEnglishName` | 국제의약품영어명 |  |
| `InternationalMedicineFranceName` | 국제의약품프랑스어명 |  |
| `ReferenceevidenceImageSerialnumber` | 참증이미지일련번호 |  |

---

## INN 명칭조회
`nameINNInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `nameType` | 명칭타입 | (LATIN:라틴어, ENGLISH:영어, FRENCH:프랑스어) |
| `internationalMedicineName` | 국제의약품명칭 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `INNInfo` |  |  |
| `ReferenceevidenceNumber` | 참증번호 |  |
| `ReferenceevidenceArticleEnglishName` | 참증물품영문명 |  |
| `FigureImageExistFlag` | 도형이미지존재유무 |  |
| `InternationalMedicineRequestNumber` | 국제의약품요청번호 |  |
| `InternationalMedicineLatinName` | 국제의약품라틴어명 |  |
| `InternationalMedicineEnglishName` | 국제의약품영어명 |  |
| `InternationalMedicineFranceName` | 국제의약품프랑스어명 |  |
| `ReferenceevidenceImageSerialnumber` | 참증이미지일련번호 |  |

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
| `transferList` | 참증번호리스트 | (ex : 참증번호1&#124;참증번호2) |

---

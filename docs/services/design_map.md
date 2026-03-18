# 디자인맵 형태분류

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 디자인맵
`designMapInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationCountry` | 출원국가 |  |
| `applicationNumber` | 출원번호 |  |
| `applicationDate` | 출원일자 |  |
| `gazetteDate` | 공보일자 |  |
| `registrationDate` | 등록일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `designMapInfo` |  |  |
| `articleCode` | 물품코드 |  |
| `applicationNumber` | 출원번호 |  |
| `designSerialNumber` | 디자인일련번호 |  |
| `applicationCountry` | 출원국가 |  |
| `designClassificationCode` | 디자인분류코드 |  |
| `articleName` | 물품명칭 |  |
| `applicationDate` | 출원일자 |  |
| `gazetteDate` | 공고일자 |  |
| `registrationDate` | 등록일자 |  |
| `formsymbol` | 폼심볼 |  |
| `originalcopyArticleName` | 원본물품명 |  |
| `similarDesignFlag` | 유사디자인유무 |  |
| `conflictDesignFlag` | 분쟁디자인유무 |  |
| `propertyCode01` | 특성코드01 |  |
| `propertyCode02` | 특성코드02 |  |
| `propertyCode03` | 특성코드03 |  |
| `propertyCode04` | 특성코드04 |  |
| `propertyCode05` | 특성코드05 |  |
| `propertyCode06` | 특성코드06 |  |
| `propertyCode07` | 특성코드07 |  |
| `propertyCode08` | 특성코드08 |  |
| `propertyCode09` | 특성코드09 |  |
| `propertyCode10` | 특성코드10 |  |
| `propertyCode11` | 특성코드11 |  |
| `propertyCode12` | 특성코드12 |  |
| `propertyCode13` | 특성코드13 |  |
| `propertyCode14` | 특성코드14 |  |
| `propertyCode15` | 특성코드15 |  |
| `propertyCode16` | 특성코드16 |  |
| `propertyCode17` | 특성코드17 |  |
| `propertyCode18` | 특성코드18 |  |
| `propertyCode19` | 특성코드19 |  |
| `propertyCode20` | 특성코드20 |  |
| `propertyCode21` | 특성코드21 |  |
| `propertyCode22` | 특성코드22 |  |
| `propertyCode23` | 특성코드23 |  |
| `propertyCode24` | 특성코드24 |  |
| `propertyCode25` | 특성코드25 |  |

---

## 특성분류
`propertyCodeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `articleCode` | 물품코드 | (필수) |
| `propertyCode` | 특성코드 | (필수) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `propertyCodeInfo` |  |  |
| `depth` | 레벨 |  |
| `classificationSystemName` | 분류체계명 |  |
| `propertyCode` | 특성코드 |  |
| `articleCode` | 물품코드 |  |
| `articleName` | 물품명칭 |  |

---

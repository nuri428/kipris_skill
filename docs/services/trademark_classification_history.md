# 상표 분류코드 변동 이력

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 이력정보
`tradeMarkClassificationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `identificationNumber` | 출원번호/등록번호 |  |
| `docsStart` | 페이지번호 | (검색 페이지 번호) |
| `docsCount` | 페이지당건수 | (기본 : 30, 최대 500) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `tradeMarkClassificationInfo` |  |  |
| `identificationNumber` | 출원번호/등록번호 |  |
| `status` | 상태 |  |
| `serialNumber` | 일련번호 |  |
| `classOfGoodSerialNumber` | 지정상품일련번호 |  |
| `classificationTypeCodeName` | 분류구분코드명 |  |
| `classificationVersion` | NICE분류판 |  |
| `goodsClassificationCode` | 상품분류코드 |  |
| `classofgoodServiceName` | 지정상품명 |  |
| `additionDeletionCode` | 추가삭제코드 |  |

---

## 변동정보

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호/등록번호1&#124;출원번호/등록번호2) |

---

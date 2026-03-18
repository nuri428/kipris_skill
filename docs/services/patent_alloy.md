# 특허 합금조성비

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 합금조성비
`alloyCompositionInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `alloyCompositionInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `openingPublicTypeCode` | 공개공고구분코드 |  |
| `openingPublicTypeName` | 공개공고구분명 |  |
| `petitionclauseSerialNumber` | 청구항일련번호 |  |
| `petitionclause` | 청구항 |  |
| `compositionYN` | 조성비여부 |  |
| `subordinationClauseYN` | 종속항여부 |  |
| `elementSymbolNumber` | 원소기호번호 |  |
| `serialNumber` | 일련번호 |  |
| `elementNameKR` | 원소한글명 |  |
| `elementNameEN` | 원소영문명 |  |
| `miniumValue` | 최소값 |  |
| `maximumValue` | 최대값 |  |
| `elementUnit` | 원소단위 |  |
| `mainComponentYN` | 주성분여부 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-합금조성비) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 |  |

---
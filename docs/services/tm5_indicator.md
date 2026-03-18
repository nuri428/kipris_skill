# TM5 공통상태 지표

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## TM5 공통상태 지표
`trademarkTM5Info`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `trademarkTM5Info` |  |  |
| `applicationNumber` | 출원번호 |  |
| `tm5CodeName` | TM5코드명 |  |
| `tm5CodeDescription` | TM5코드설명 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1-TM5공통상태지표) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변공건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

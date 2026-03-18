# 상표 행정처리 이력

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 통합이력정보(상표)
`relatedDocsonfileInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `relateddocsonfileInfo` |  |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `documentNumber` | 접수발송번호 |  |
| `documentDate` | 접수발송일자 |  |
| `documentTitle` | 접수발송서류명 |  |
| `documentTitleEng` | 접수발송서류명 | (영문) |
| `status` | 처리상태 |  |
| `statusEng` | 처리상태 | (영문) |
| `step` | 단계 | (출원, 심판, 등록) |
| `trialNumber` | 심판번호 |  |
| `registrationNumber` | 등록번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1 : 통합이력정보(상표)) |
| `transferDate` | 변동일자 | ※ 입력방식(ex : 20160713) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

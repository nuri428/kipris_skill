# 특허·실용 행정처리 이력

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 통합이력정보(특실)
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
| `documentNumber` | 접수발송번호 |  |
| `documentDate` | 접수발송일자 |  |
| `documentTitle` | 접수발송서류명 | 한글 |
| `documentTitleEng` | 접수발송서류명 | 영문 |
| `status` | 처리상태 | 한글 |
| `statusEng` | 처리상태 | 영문 |
| `step` | 단계 | (출원, 심판, 등록) |
| `trialNumber` | 심판번호 |  |
| `registrationNumber` | 등록번호 |  |

---

## 변동정보
`transferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `kind` | 검색코드 | (oper1 : 통합이력정보(특실)) |
| `searchRight` | 권리 | (all : 전체, p : 특허, u : 실용신안) ※ 입력방식(ex : p) |
| `transferDate` | 변동일자 | ※ 입력방식(ex : 20160713) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `transferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 출원번호리스트 | (ex : 출원번호1&#124;출원번호2) |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `applicationNumber` | 출원번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

# 인터넷 기술공지

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 2개 (구현: 0, 폐기예정: 0)

---

## 인터넷기술공지
`internetTechNoticeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `announcementTitle` | 공지제목 |  |
| `drawupDate` | 작성일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `internetTechNoticeInfo` |  |  |
| `developer` | 개발자 |  |
| `drawingPath` | 도면경로 |  |
| `announcementNumber` | 공지번호 |  |
| `announcementTitle` | 공지제목 |  |
| `drawupDate` | 작성일자 |  |
| `drawupPerson` | 작성자 |  |
| `drawupPersonAddress` | 작성자주소 |  |
| `technologyConfiguration` | 기술구성 |  |
| `technologyEffect` | 기술효과 |  |
| `technologyCorrelatorField` | 기술관련분야 |  |
| `technologyPurpose` | 기술목적 |  |

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
| `transferList` | 출원번호리스트 | (ex : 공지제목1&#124;공지제목2) |

---
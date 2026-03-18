# 특허 중한 코퍼스

> ⚠️ **ServicePath 미확인 — 스킬 미지원**
> 이 서비스는 KIPRIS Plus 포털에서 API로 제공되지만, REST API 경로(ServicePath)가 아직 확인되지 않아 `/kipris` 스킬에서 호출할 수 없습니다.

- **API 유형**: REST
- **오퍼레이션 수**: 1개 (구현: 0, 폐기예정: 0)

---

## 기본조회

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `inputnumber` | 입력번호 |  |
| `inputnumberType` | 입력번호종류 | 문헌번호(LN), 출원번호(AN) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `PatentChineseKoreanCorpusInfo` |  |  |
| `CountryCode` | 국가코드 |  |
| `CountryCodeName` | 국가코드명 |  |
| `Literaturenumber` | 문헌번호 |  |
| `Applicationnumber` | 출원번호 |  |
| `LanguageCode` | 언어코드 |  |
| `LanguageCodeName` | 언어코드명 |  |
| `Internationalpatentclassification` | IPC코드 |  |
| `LiteratureKindCode` | 문헌종류코드 |  |
| `LiteratureKindName` | 문헌종류명 |  |
| `Type` | 구분 |  |
| `OriginalcopyLiterature` | 원본문헌 |  |
| `TranslationLiterature` | 번역문헌 |  |
| `LetterCount` | 글자수 |  |

---
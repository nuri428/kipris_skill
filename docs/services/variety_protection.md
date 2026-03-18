# 품종보호권 등록 식물 명칭

- **API 유형**: REST
- **오퍼레이션 수**: 3개 (구현: 0, 폐기예정: 0)

---

## 품종 기본조회
`basicVarietyInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `referenceevidenceNumber` | 참증번호 | (내부관리번호) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `VarietyInfoList` |  |  |
| `ReferenceevidenceNumber` | 참증번호 |  |
| `ReferenceevidenceArticleHangeulName` | 참증물품한글명 |  |
| `ReferenceevidenceArticleEnglishsentenceName` | 참증물품영문명 |  |
| `RelationCountryCode` | 관련국가코드 |  |
| `RegistrationNumberOrder` | 등록번호순서 |  |
| `RegistrationNumber` | 등록번호?※특허제도와무관한등록번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `TrademarkReferenceevidenceDataOfferplaceName` | 상표참증자료제공처명 |  |
| `InternationalorganizationClassificationCode` | 국제기구분류코드 |  |
| `InternationalorganizationName` | 국제기구명 |  |
| `LoadBasisName` | 탑재근거명 |  |
| `LanguageTypeCode` | 언어구분코드 |  |
| `CityNationalityName` | 시도국적명 |  |
| `LoadBasisContent` | 탑재근거내용 |  |
| `CropsTypeCode` | 작물구분코드 |  |
| `PlantName` | 식물명 |  |
| `SeedDescription` | 종자설명 |  |
| `RacePetitionerName` | 품종신청인명 |  |
| `SeedNameApplicationNumber` | 종자명출원번호 |  |
| `SeedNameApplicationDate` | 종자명출원일자 |  |
| `SeedNamePublicNumber` | 종자명공고번호 |  |
| `SeedNamePublicDate` | 종자명공고일자 |  |
| `RaceRegistrationNumber` | 품종등록번호 |  |
| `RaceContinuanceStartDate` | 품종존속시작일자 |  |
| `RaceContinuanceEndDate` | 품종존속종료일자 |  |
| `SeedNameMotionNumber` | 종자명신청번호 |  |
| `SeedNameMotionDate` | 종자명신청일자 |  |
| `SeedNameRecordNumber` | 종자명등재번호 |  |
| `SeedNameRecordDate` | 종자명등재일자 |  |
| `RecordValidationTermStartDate` | 등재유효기간시작일자 |  |
| `RecordValidationTermEndDate` | 등재유효기간종료일자 |  |
| `SeedNameStatementReceiptNumber` | 종자명신고접수번호 |  |
| `SeedNameStatementReceiptDate` | 종자명신고접수일자 |  |
| `SeedNameStatementCertificateNumber` | 종자명신고증서번호 |  |
| `SeedNameStatementCertificateDate` | 종자명신고증서일자 |  |
| `SeedNameStatementApplicationNumber` | 종자명신고출원번호 |  |
| `SeedNameStatementApplicationDate` | 종자명신고출원일자 |  |
| `SeedNameStatementPublicNumber` | 종자명신고공고번호 |  |

---

## 품종 명칭조회
`nameVarietyInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `referenceevidenceArticleName` | 참증물품명 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `VarietyInfoList` |  |  |
| `ReferenceevidenceNumber` | 참증번호 |  |
| `ReferenceevidenceArticleHangeulName` | 참증물품한글명 |  |
| `ReferenceevidenceArticleEnglishsentenceName` | 참증물품영문명 |  |
| `RelationCountryCode` | 관련국가코드 |  |
| `RegistrationNumberOrder` | 등록번호순서 |  |
| `RegistrationNumber` | 등록번호?※특허제도와무관한등록번호 |  |
| `RegistrationDate` | 등록일자 |  |
| `TrademarkReferenceevidenceDataOfferplaceName` | 상표참증자료제공처명 |  |
| `InternationalorganizationClassificationCode` | 국제기구분류코드 |  |
| `InternationalorganizationName` | 국제기구명 |  |
| `LoadBasisName` | 탑재근거명 |  |
| `LanguageTypeCode` | 언어구분코드 |  |
| `CityNationalityName` | 시도국적명 |  |
| `LoadBasisContent` | 탑재근거내용 |  |
| `CropsTypeCode` | 작물구분코드 |  |
| `PlantName` | 식물명 |  |
| `SeedDescription` | 종자설명 |  |
| `RacePetitionerName` | 품종신청인명 |  |
| `SeedNameApplicationNumber` | 종자명출원번호 |  |
| `SeedNameApplicationDate` | 종자명출원일자 |  |
| `SeedNamePublicNumber` | 종자명공고번호 |  |
| `SeedNamePublicDate` | 종자명공고일자 |  |
| `RaceRegistrationNumber` | 품종등록번호 |  |
| `RaceContinuanceStartDate` | 품종존속시작일자 |  |
| `RaceContinuanceEndDate` | 품종존속종료일자 |  |
| `SeedNameMotionNumber` | 종자명신청번호 |  |
| `SeedNameMotionDate` | 종자명신청일자 |  |
| `SeedNameRecordNumber` | 종자명등재번호 |  |
| `SeedNameRecordDate` | 종자명등재일자 |  |
| `RecordValidationTermStartDate` | 등재유효기간시작일자 |  |
| `RecordValidationTermEndDate` | 등재유효기간종료일자 |  |
| `SeedNameStatementReceiptNumber` | 종자명신고접수번호 |  |
| `SeedNameStatementReceiptDate` | 종자명신고접수일자 |  |
| `SeedNameStatementCertificateNumber` | 종자명신고증서번호 |  |
| `SeedNameStatementCertificateDate` | 종자명신고증서일자 |  |
| `SeedNameStatementApplicationNumber` | 종자명신고출원번호 |  |
| `SeedNameStatementApplicationDate` | 종자명신고출원일자 |  |
| `SeedNameStatementPublicNumber` | 종자명신고공고번호 |  |

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

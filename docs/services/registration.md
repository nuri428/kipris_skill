# 등록사항

- **API 유형**: REST
- **오퍼레이션 수**: 12개 (구현: 0, 폐기예정: 0)
- **서비스 경로**: `RegistrationService` (포털 확인)
- **게이트웨이**: OpenAPI (`/openapi/rest/`)
- **인증 키**: `accessKey`

---

## 등록사항
`registrationInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationInfo` |  |  |
| `registrationRightHolderInfo` |  |  |
| `registrationRightHolderInfoA` |  |  |
| `rankNumber` | 순위번호 |  |
| `rankCorrelatorSerialNumber` | 순위관련자일련번호 |  |
| `rankCorrelatorType` | 순위관련자종류 | 권리자, 의무자 등 |
| `rankCorrelatorName` | 순위관련자명 | 권리자명, 의무자명 등 |
| `rankCorrelatorAddress` | 순위관련자주소 |  |
| `registrationRightHolderInfoB` | 권리자정보B |  |
| `rankNumber` | 순위번호 |  |
| `documentName` | 서류명 |  |
| `receiptDate` | 접수일자 |  |
| `registrationCauseName` | 등록원인명 |  |
| `indicationOfEvent` | 사건의표시 |  |
| `registrationRightRankInfo` |  |  |
| `rankNumber` | 순위번호 |  |
| `pertinentPartition` | 해당란 |  |
| `contactId` | 담당자ID |  |
| `documentName` | 서류명 |  |
| `documentCode` | 서류코드 |  |
| `originalRegistrationNumber` | 원등록번호 |  |
| `registrationPurpose` | 등록목적 |  |
| `registrationDate` | 등록일자 |  |
| `registrationCsCode` | 등록원인코드 |  |
| `registrationCauseName` | 등록원인명 |  |
| `registrationCauseDate` | 등록원인일자 |  |
| `registrationTpCode` | 등록구분코드 |  |
| `receiptNumber` | 접수번호 |  |
| `receiptDate` | 접수일자 |  |
| `disappearanceFlag` | 주말유무 | (Y/N) |
| `disappearanceCauseName` | 주말원인내용 |  |
| `disappCscd` | 주말원인코드 |  |
| `disappearanceDate` | 주말일자 |  |
| `internationalRegRecordDateMD` | 국제등록기록일자 | (마드리드) |
| `expirationDateMD` | 존속기간만료일자 | (마드리드) |
| `latestRenewalDateMD` | 최근갱신일자 | (마드리드) |
| `subDesignationDateMD` | 사후지정일자 | (마드리드) |
| `registrationFeeInfo` |  |  |
| `registrationDate` | 등록일자 |  |
| `startAnnual` | 시작연차 |  |
| `lastAnnual` | 마지막연차 |  |
| `paymentDegree` | 납부차수 |  |
| `paymentFee` | 납부금액 |  |
| `paymentDate` | 납부일자 |  |
| `registrationLastRightHolderInfo` |  |  |
| `lastRightHolderNumber` | 최종권리자번호(특허고객번호) |  |
| `lastRightHolderName` | 최종권리자명 |  |
| `lastRightHolderAddress` | 최종권리자주소 |  |
| `lastRightHolderCountry` | 최종권리자국가 |  |
| `registrationRightInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationDate` | 등록일자 |  |
| `assessmentDate` | 사정일자 |  |
| `expirationDate` | 존속기간만료일자 |  |
| `terminationCauseName` | 소멸원인명 |  |
| `terminationDate` | 소멸일자 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `internationRegistrationNumber` | 국제등록번호 |  |
| `internationRegistrationDate` | 국제등록일자 |  |
| `originalApplicationNumber` | 원출원번호 |  |
| `originalApplicationDate` | 원출원일자 |  |
| `trademarkRegistrationPublicDate` | 상표등록공고일자 |  |
| `trademarkRegistrationPublicNumber` | 상표등록공고번호 |  |
| `classCode` | 분류코드 |  |
| `titleOfInvention` | 발명의명칭/물품명칭/상표명칭 | 한글 |
| `titleOfInventionEng` | 발명의명칭/물품명칭/상표명칭 | 영문 |
| `claimCount` | 청구항수 |  |
| `priorityCountry` | 우선권주장국가 |  |
| `priorityDate` | 우선권주장일자 |  |
| `priorityCount` | 우선권주장수 |  |
| `dsNonExaminationTarget` | 디자인무심사대상여부 | 심사, 일부심사, 무심사 * 20140701(무심사, 일부심사 분기) |

---

## 권리정보
`registrationRightInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationRightInfo` |  |  |
| `registrationNumber` | 등록번호 |  |
| `regReferenceNumber` | 등록참조번호 |  |
| `registrationDate` | 등록일자 |  |
| `assessmentDate` | 사정일자 |  |
| `expirationDate` | 존속기간만료일자 |  |
| `terminationCauseName` | 소멸원인명 |  |
| `terminationDate` | 소멸일자 |  |
| `applicationNumber` | 출원번호 |  |
| `appReferenceNumber` | 출원참조번호 |  |
| `applicationDate` | 출원일자 |  |
| `publicationNumber` | 공고번호 |  |
| `publicationDate` | 공고일자 |  |
| `internationRegistrationNumber` | 국제등록번호 |  |
| `internationRegistrationDate` | 국제등록일자 |  |
| `originalApplicationNumber` | 원출원번호 |  |
| `originalApplicationDate` | 원출원일자 |  |
| `classCode` | 분류코드 |  |
| `titleOfInvention` | 발명의명칭/물품명칭/상표명칭 | 한글 |
| `titleOfInventionEng` | 발명의명칭/물품명칭/상표명칭 | 영문 |
| `claimCount` | 청구항수 |  |
| `priorityCountry` | 우선권주장국가 |  |
| `priorityDate` | 우선권주장일자 |  |
| `priorityCount` | 우선권주장수 |  |

---

## 권리자정보
`registrationRightHolderInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationRightHolderInfo` |  |  |
| `registrationRightHolderInfoA` |  |  |
| `rankNumber` | 순위번호 |  |
| `rankCorrelatorSerialNumber` | 순위관련자일련번호 |  |
| `rankCorrelatorType` | 순위관련자종류 | 권리자, 의무자 등 |
| `rankCorrelatorName` | 순위관련자명 | 권리자명, 의무자명 등 |
| `rankCorrelatorAddress` | 순위관련자주소 |  |
| `registrationRightHolderInfoB` | 권리자정보B |  |
| `rankNumber` | 순위번호 |  |
| `documentName` | 서류명 |  |
| `receiptDate` | 접수일자 |  |
| `registrationCauseName` | 등록원인명 |  |
| `indicationOfEvent` | 사건의표시 |  |

---

## 권리순위정보
`registrationRightRankInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationRightRankInfo` |  |  |
| `rankNumber` | 순위번호 |  |
| `pertinentPartition` | 해당란 |  |
| `documentName` | 서류명 |  |
| `originalRegistrationNumber` | 원등록번호 |  |
| `registrationPurpose` | 등록목적 |  |
| `registrationDate` | 등록일자 |  |
| `registrationCauseName` | 등록원인명 |  |
| `registrationCauseDate` | 등록원인일자 |  |
| `receiptNumber` | 접수번호 |  |
| `receiptDate` | 접수일자 |  |
| `disappearanceFlag` | 주말유무 | (Y/N) |
| `disappearanceCauseName` | 주말원인명 |  |
| `disappearanceDate` | 주말일자 |  |
| `internationalRegRecordDateMD` | 국제등록기록일자 | (마드리드) |
| `expirationDateMD` | 존속기간만료일자 | (마드리드) |
| `latestRenewalDateMD` | 최근갱신일자 | (마드리드) |
| `subDesignationDateMD` | 사후지정일자 | (마드리드) |

---

## 등록료정보
`registrationFeeInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationFeeInfo` |  |  |
| `registrationDate` | 등록일자 |  |
| `startAnnual` | 시작연차 |  |
| `lastAnnual` | 마지막연차 |  |
| `paymentDegree` | 납부차수 |  |
| `paymentFee` | 납부금액 |  |

---

## 최종권리자정보
`registrationLastRightHolderInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationLastRightHolderInfo` |  |  |
| `lastRightHolderNumber` | 최종권리자번호(특허고객번호) |  |
| `lastRightHolderName` | 최종권리자명 |  |
| `lastRightHolderAddress` | 최종권리자주소 |  |
| `lastRightHolderCountry` | 최종권리자국가 |  |

---

## 변동정보
`registrationTransferListInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `searchType` | 검색코드 | (BIB:서지, FEE:등록료, ORD:권리순위, HLD:권리자) |
| `transferDate` | 변동일자 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationTransferListInfo` |  |  |
| `transferCount` | 변동건수 |  |
| `transferList` | 등록번호리스트 | (ex : 등록번호1&#124;등록번호2) |

---

## 권리자정보V2
`registrationRightHolderV2Info`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationRightHolderV2Info` |  |  |
| `registrationRightHolderV2InfoA` |  |  |
| `rankNumber` | 순위번호 |  |
| `rankCorrelatorSerialNumber` | 순위관련자일련번호 |  |
| `rankCorrelatorType` | 순위관련자종류 | 권리자, 의무자 등 |
| `rankCorrelatorCode` | 순위관련자명 | 권리자명, 의무자명 등 |
| `rankCorrelatorName` | 순위관련자코드 |  |
| `rankCorrelatorAddress` | 순위관련자주소 |  |
| `registrationRightHolderV2InfoB` | 권리자정보B |  |
| `rankNumber` | 순위번호 |  |
| `documentName` | 서류명 |  |
| `receiptDate` | 접수일자 |  |
| `registrationCauseName` | 등록원인명 |  |
| `indicationOfEvent` | 사건의표시 |  |

---

## 존속기간만료예정일자
`registrationContinuanceTermInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationContinuanceTermInfo` |  |  |
| `continuanceDate` | 만료일자 |  |

---

## 등록사항 조회(권리란, 권리자란, 전용·통상사용권자란)
`registrationInformationV2`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |
| `searchCode` | 검색코드 | (권리란 : 20901, 권리자란 : 20902, 전용권자란 : 20903, 통상권자란 : 20904) |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationInformationV2` |  |  |
| `registrationRightRankV2` |  |  |
| `rgstno` | 등록번호 |  |
| `ptprtCd` | 해당란코드 |  |
| `ptprtCdNm` | 해당란 |  |
| `rkno` | 순위번호 |  |
| `rgstTpcd` | 등록구분코드 |  |
| `rgstTpcdNm` | 등록구분코드명 |  |
| `docCd` | 서류코드 |  |
| `docNm` | 서류명 |  |
| `rcptDt` | 접수일자 |  |
| `idsappFg` | 주말유무 |  |
| `disappCscd` | 주말원인코드 |  |
| `disappCsCont` | 주말원인내용 |  |
| `disappDt` | 주말일자 |  |
| `rgstCscd` | 등록원인코드 |  |
| `rgstCsNm` | 등록원인명 |  |
| `rgstCsDt` | 등록원인일자 |  |
| `rgstPupos` | 등록목적 |  |
| `divRgstno` | 분할등록번호 |  |
| `lcnsUsprdStrtDt` | 실시권사용기간시작일자 |  |
| `lcnsUsprdEndDt` | 실시권사용기간종료일자 |  |
| `wrkgContCd` | 실시내용코드 |  |
| `wrkgCont` | 실시내용 |  |
| `wrkgRgsNm` | 실시지역명 |  |
| `etcLcnsMtr` | 기타실시권사항 |  |
| `rmvWavItcnt` | 말소포기항수 |  |
| `cntryRsmptAdmnrNm` | 국가승계관리자성명 |  |
| `cntryRsmptIntndNm` | 국가승계관리청명 |  |
| `rsmptOffcNm` | 승계청명 |  |
| `pldgCdamtCont` | 질권채권액내용 |  |
| `pldgExptnDt` | 질권채권변제일자 |  |
| `pldgSpcntMtr` | 질권특약사항 |  |
| `cmmssMtrLwatcNo` | 위임사항법조항번호 |  |
| `trpreTrlno` | 심판예고심판번호 |  |
| `trpreDmndDt` | 심판예고청구일자 |  |
| `trpreEvtIndicCont` | 심판예고사건표시내용 |  |
| `trpreDmndObjt` | 심판예고청구취지 |  |
| `dotdcTrlno` | 심결확정심판번호 |  |
| `dotdcDt` | 심결확정일자 |  |
| `dotdcInvldDmndItcnt` | 심결확정무효청구항수 |  |
| `dotdcAbs` | 심결확정요지 |  |
| `wthdwTrlno` | 취하심판번호 |  |
| `wthdwDt` | 취하일자 |  |
| `seizrEvtIndicCont` | 촉탁사건표시내용 |  |
| `cntnTmextApplno` | 존속기간연장출원번호 |  |
| `cndrtExaplDt` | 존속기간연장출원일자 |  |
| `cntnTmextDcsnDt` | 존속기간연장결정일자 |  |
| `cntnTmextDays` | 존속기간연장일수 |  |
| `cntnTmextYear` | 존속기간연장년 |  |
| `cntnTmextMm` | 존속기간연장월 |  |
| `cntnTmextDd` | 존속기간연장일 |  |
| `extnTrnsfCndrtDt` | 연장이전존속기간일자 |  |
| `cntnTmextDmndItcnt` | 존속기간연장청구항수 |  |
| `cntnTmextPmsnCont` | 존속기간연장허가내용 |  |
| `cntnTmextTgtDmndScope` | 존속기간연장대상청구범위 |  |
| `opstnPbancDemrno` | 이의신청예고이의신청번호 |  |
| `opstnPbancOpstnDt` | 이의신청예고이의신청일자 |  |
| `opstnPbancOpstnCs` | 이의신청예고이의신청이유 |  |
| `dmdcsDemrno` | 이의결정이의신청번호 |  |
| `dmdcsDt` | 이의결정일자 |  |
| `dmdcsAbs` | 이의결정요지 |  |
| `cndrtTnwlApplDt` | 존속기간갱신출원일자 |  |
| `cndrtRnwlApplno` | 존속기간갱신출원번호 |  |
| `cndrtRnwlDcsnDt` | 존속기간갱신결정일자 |  |
| `dvtrRgstno` | 분할이전등록번호 |  |
| `cofgdAddApplDt` | 지정상품추가출원일자 |  |
| `cofgdAddApplno` | 지정상품추가출원번호 |  |
| `orgnlRgstno` | 원등록번호 |  |
| `hgrnkTcevlDmndno` | 상위기술평가청구번호 |  |
| `tcevlDmndDt` | 기술평가청구일자 |  |
| `tcevlDmndObjt` | 기술평가청구취지 |  |
| `tcevlCfmtnDt` | 기술평가확정일자 |  |
| `tcevlCfmtnAbs` | 기술평가확정요지 |  |
| `lcnsPriceAmtCont` | 실시권대가금액내용 |  |
| `lcnsPricePayMthd` | 실시권대가지급방법 |  |
| `lcnsPricePmeraCont` | 실시권대가지급시기내용 |  |
| `partRmvWavClausCont` | 일부말소포기항내용 |  |
| `pldgIrAgmntCont` | 질권이자약정내용 |  |
| `pldgPntyAgmntCont` | 질권위약금약정내용 |  |
| `dcsnCoargInvldPtclsCont` | 결정등록취소무효청구항내용 |  |
| `remnClausCont` | 유지항내용 |  |
| `dcsnDelItcnt` | 결정삭제항수 |  |
| `dcsnRgstDlclsCont` | 결정등록삭제항내용 |  |
| `mdItrgtRecDt` | 마드리드국제등록기록일자 |  |
| `mdCndrtExptnDt` | 마드리드존속기간만료일자 |  |
| `mdLtstRnwlDt` | 마드리드최근갱신일자 |  |
| `mdItrgtEfocrDt` | 마드리드국제등록효력발생일자 |  |
| `anxtnTgtIntnlRgstno` | 병합대상국제등록번호 |  |
| `dcsnCoargInvldDmndItcnt` | 결정등록취소무효청구항수 | 권리란(20901) |
| `registrationRightHolderInfoV3` |  |  |
| `rkCrltrSeq` | 순위관련자일련번호 |  |
| `rkCrltrTpcd` | 순위관련자코드 |  |
| `rkCrltrTpcdNm` | 순위관련자코드명 | 권리자,의무자 등(입력값 관련 권리란, 권리권자란, 전용권자란, 통상권자란에 해당하는 인명정보) |
| `rkCrltrNm` | 순위관련자명 | 권리자명, 의무자명 등 |
| `rkCrltrAddr` | 순위관련자주소 |  |

---

## (신규)권리자 정보를 제공
`newRightfulPersonInfo`

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `newRightInfo` |  |  |
| `rkno` | 순위번호 |  |
| `doc_nm` | 서류명 |  |
| `rcpt_dt` | 접수일자 |  |
| `rgst_cs_nm` | 등록원인 |  |
| `evt_indic_seizr` | 사건의표시 |  |
| `newRightPersonInfo` |  |  |
| `rkno` | 순위번호 |  |
| `rk_psn_nm` | 순위관련자명 | 권리자명,의무자명 등 |
| `rk_rel_psn_seq` | 순위관련자일련번호 |  |
| `rk_rel_psn_tpcd` | 순위관련자종류 | 권리자,의무자 등 |
| `rk_rel_psn_addr` | 순위관련자주소 |  |

---

## 최종변동일자

- **분류**: 오퍼레이션
- **상태**: ❌ 미구현

### 요청 파라미터 (IN)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `registrationNumber` | 등록번호 |  |

### 응답 파라미터 (OUT)

| 항목명 | 설명 | 비고 |
|--------|------|------|
| `items` |  |  |
| `lastTransferDateInfo` | 최종변동일자 |  |

---

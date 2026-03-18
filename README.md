# KIPRIS 한국 지식재산 검색 — Claude Code Skill

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![KIPRIS API](https://img.shields.io/badge/KIPRIS-Open%20API-003DA5.svg)](https://plus.kipris.or.kr)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-orange.svg)](https://claude.ai/code)

> **Korean Intellectual Property Search for Claude Code**
> Search Korean patents, utility models, designs, trademarks, and foreign patents directly from Claude Code using KIPRIS Plus Open API.

한국특허청(KIPRIS) Open API를 활용하여 특허, 실용신안, 디자인, 상표, 해외특허 정보를 Claude Code에서 직접 검색할 수 있는 Skill입니다.

## Demo

```
You: /kipris 인공지능 관련 특허를 검색해줘

Claude: KIPRIS API로 "인공지능" 키워드 검색을 수행합니다...

총 106,285건 검색됨 (상위 5건 표시)

| # | 발명의명칭 | 출원번호 | 출원인 | 등록상태 |
|---|-----------|---------|--------|---------|
| 1 | 의미론적 정보와 공간적 정보를 보강하여 휴먼 파싱을 수행하는 인공지능 네트워크 | 1020240124164 | 아주대학교산학협력단 | 공개 |
| 2 | 인공지능 기반 실시간 이상 행동 분류 및 감지 장치 및 방법 | 1020240004987 | 동국대학교 산학협력단 | 공개 |
| 3 | 질의-응답 과업 성능을 향상시키기 위해 인공지능 모델을 학습시키는 방법 및 장치 | 1020240191256 | 성균관대학교산학협력단 | 등록 |
| ... | ... | ... | ... | ... |
```

```
You: /kipris artificial intelligence 미국 특허 검색

Claude: KIPRIS 해외특허 API로 미국(US) 특허를 검색합니다...

| # | Title | Application No. | Applicant |
|---|-------|----------------|-----------|
| 1 | Code Enhancement System and Method Using Artificial Intelligence | 19299938 | Turing Intelligence Technology Limited |
| 2 | Systems and methods for slot machine game development utilizing graphic-based AI | 18354589 | Sierra Artificial Neural Networks |
| ... | ... | ... | ... |
```

## 지원 검색

| 분류 | 검색 유형 | 오퍼레이션 수 |
|------|----------|-------------|
| 국내 특허·실용 | 키워드, 출원번호, 출원인, 등록권자, 서지정보 | 7개 |
| 해외 특허 | 키워드, 출원번호, 국제공개번호, 출원인, 국제출원번호 | 5개 |
| 기타 47개 서비스 | ServicePath 확인 후 동적 호출 가능 | 528개 |

**총 49개 서비스, 540개 오퍼레이션** 커버 (12개 Tier 1 즉시 사용, 528개 Tier 2 문서 참조 호출)

## 바로 사용 가능한 API (Tier 1 — 12개)

ServicePath가 검증된 오퍼레이션으로, `/kipris` 스킬에서 즉시 호출할 수 있습니다.

### 국내 특허·실용신안 (7개)

| # | 오퍼레이션 | ID | 설명 |
|---|-----------|-----|------|
| 1 | 전체검색 | `getAdvancedSearch` | 다항목 복합 조건 검색 (발명명칭, 출원인, IPC 등) |
| 2 | 자유검색 | `freeSearchInfo` | 키워드 기반 자유 검색 |
| 3 | 출원번호검색 | `applicationNumberSearchInfo` | 출원번호로 특정 특허 조회 |
| 4 | 출원인검색 | `applicantNameSearchInfo` | 출원인명으로 특허 검색 |
| 5 | 등록권자검색 | `rightHolerSearchInfo` | 등록권자명으로 특허 검색 |
| 6 | 서지상세정보 | `getBibliographyDetailInfoSearch` | 청구항, 발명자, IPC 등 상세정보 |
| 7 | 서지요약정보 | `getBibliographySumryInfoSearch` | 특허 요약 서지정보 |

### 해외 특허 (5개)

| # | 오퍼레이션 | ID | 지원 국가 |
|---|-----------|-----|----------|
| 1 | 자유검색 | `freeSearch` | US, EP, WO, JP, CN 등 13개국 |
| 2 | 출원번호검색 | `applicationNumberSearch` | 〃 |
| 3 | 국제공개번호검색 | `internationalOpenNumberSearch` | 〃 |
| 4 | 출원인검색 | `applicantSearch` | 〃 |
| 5 | 국제출원번호검색 | `internationalApplicationNumberSearch` | 〃 |

> 이 외 528개 오퍼레이션은 `docs/services/` 문서 참조 후 동적 호출 가능 (20개 서비스는 ServicePath 확인됨, 29개는 미확인)

## Quick Start

```bash
# 1. Clone
git clone https://github.com/nuri428/kipris_skill.git ~/dev/kipris_skill

# 2. API 키 설정 (KIPRIS Plus에서 발급)
echo 'export KIPRIS_API_KEY="your-api-key"' >> ~/.zshrc
source ~/.zshrc

# 3. Skill 등록
mkdir -p ~/.claude/skills
ln -s ~/dev/kipris_skill/SKILL.md ~/.claude/skills/kipris.md

# 4. 사용!
# Claude Code에서: /kipris 인공지능 특허 검색해줘
```

## 설치 상세

### 1. API 키 발급

두 가지 발급처가 있으며, 오퍼레이션에 따라 사용하는 게이트웨이가 다릅니다:

| 게이트웨이 | 키 파라미터 | 발급처 |
|-----------|-----------|--------|
| OpenAPI | `accessKey` | [KIPRIS Plus](https://plus.kipris.or.kr) 회원가입 후 발급 |
| KIPO API | `ServiceKey` | [공공데이터 포털](https://www.data.go.kr) 활용 신청 후 발급 |

### 2. 환경변수 설정

```bash
export KIPRIS_API_KEY="발급받은_API_키"
```

셸 프로필(`~/.zshrc`, `~/.bashrc` 등)에 추가하면 영구 적용됩니다.

### 3. Skill 등록

**전역 설치** (모든 프로젝트에서 사용):

```bash
mkdir -p ~/.claude/skills
ln -s ~/dev/kipris_skill/SKILL.md ~/.claude/skills/kipris.md
```

**프로젝트별 설치**:

```bash
mkdir -p /path/to/project/.claude/skills
ln -s ~/dev/kipris_skill/SKILL.md /path/to/project/.claude/skills/kipris.md
```

## API 사용 제한

| 항목 | 제한 |
|------|------|
| 초당 호출 횟수 | **⚠️ 50회 미만** (초과 시 IP 차단) |
| 월간 무료 호출 | **1,000회/월** (무료 가입자 기준) |
| 호출 횟수 초기화 | 매월 1일 |
| 미신청 API 호출 | **헤더에 에러 메시지 반환** (신청하지 않은 API 호출 시) |

> **Note**: 무료 가입자는 월 1,000회까지 API 호출이 가능합니다. 초과 사용이 필요한 경우 [KIPRIS Plus](https://plus.kipris.or.kr)에서 유료 플랜을 확인하세요.
>
> **주의**: 유료 플랜 사용 시에도 별도로 신청한 API만 호출할 수 있습니다. 신청하지 않은 API를 호출하면 응답 헤더에 에러 메시지가 반환되므로, 사용할 서비스를 KIPRIS Plus 포털에서 미리 신청해야 합니다.

## 사용법

Claude Code에서 `/kipris` 명령으로 호출하거나 자연어로 요청합니다:

```
/kipris 인공지능 관련 특허를 검색해줘
/kipris 삼성전자가 출원한 특허를 찾아줘
/kipris 출원번호 1020200123456의 상세정보
/kipris artificial intelligence 미국 특허 검색
/kipris LG에너지솔루션 등록특허 조회
```

### 지원 오퍼레이션

#### 국내 특허·실용신안

| 검색 유형 | 주요 파라미터 | 예시 |
|----------|-------------|------|
| 키워드 검색 | `word` | "배터리 관련 특허" |
| 출원번호 검색 | `applicationNumber` | "출원번호 1020200123456" |
| 출원인 검색 | `applicant` | "삼성전자 출원 특허" |
| 등록권자 검색 | `rightHoler` | "현대자동차 등록특허" |
| 전체검색 (다항목) | 복합 파라미터 | "발명명칭에 AI, 출원인 카이스트" |
| 서지상세정보 | `applicationNumber` | "출원번호 xxx의 청구항, 발명자 정보" |
| 서지요약정보 | `applicationNumber` | "출원번호 xxx의 요약정보" |

#### 해외 특허

| 검색 유형 | 주요 파라미터 | 예시 |
|----------|-------------|------|
| 키워드 검색 | `free`, `collectionValues` | "AI 미국 특허" |
| 출원번호 검색 | `applicationNumber` | "US 출원번호 17/xxx" |
| 국제공개번호 검색 | `internationalOpenNumber` | "WO2024/xxx" |
| 출원인 검색 | `applicant` | "Google 유럽 특허" |
| 국제출원번호 검색 | `internationalApplicationNumber` | "PCT/US2024/xxx" |

**해외 지원 국가**: 미국(US), 유럽(EP), PCT(WO), 일본(JP), 중국(CP/CN), 대만(TW), 러시아(RU), 콜롬비아(CO), 스웨덴(SE), 스페인(ES), 이스라엘(IL)

## 아키텍처

```
사용자 요청 → Claude Code → SKILL.md (오퍼레이션 매핑)
                                ↓
                        curl (KIPRIS API 호출)
                                ↓
                        XML 응답 수신
                                ↓
                        python3 (XML → JSON 파싱)
                                ↓
                        Claude가 결과 정리 → 사용자에게 테이블로 제공
```

## 문서 구조

```
├── SKILL.md                    # 스킬 본체 (Single Source of Truth)
├── CLAUDE.md                   # 프로젝트 컨텍스트
├── README.md                   # 이 파일
└── docs/
    ├── README.md               # API 명세 인덱스 (49개 서비스)
    └── services/               # 서비스별 상세 명세
        ├── patent_utility.md   # 특허·실용 (61 ops) ✅
        ├── foreign_patent.md   # 해외특허 (81 ops) ✅
        ├── design.md           # 디자인 (51 ops) ✅
        ├── trademark.md        # 상표 (54 ops) ✅
        └── ...                 # 총 49개 파일
```

## Contributing

1. Fork this repository
2. 새로운 서비스의 `ServicePath`를 확인하여 문서에 반영
3. Pull Request 제출

특히 다음 기여를 환영합니다:
- 미확인 29개 서비스의 `ServicePath` 매핑
- 디자인, 상표 서비스 Tier 1 추가
- 에러 핸들링 개선

## License

이 프로젝트는 MIT 라이선스를 따릅니다. API 데이터는 [KIPRIS Plus 이용약관](https://plus.kipris.or.kr)을 따릅니다.

---

<p align="center">
  <b>한국 지식재산 데이터를 Claude Code에서 바로 검색하세요!</b><br>
  Search Korean IP data directly from Claude Code!<br><br>
  <a href="https://github.com/nuri428/kipris_skill">Star this repo</a> if you find it useful ⭐
</p>

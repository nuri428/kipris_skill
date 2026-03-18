# KIPRIS 한국 지식재산 검색 — Claude Code Skill

한국특허청(KIPRIS) Open API를 활용하여 특허, 실용신안, 디자인, 상표, 해외특허 정보를 Claude Code에서 직접 검색할 수 있는 Skill입니다.

## 지원 검색

| 분류 | 검색 유형 | 오퍼레이션 수 |
|------|----------|-------------|
| 국내 특허·실용 | 키워드, 출원번호, 출원인, 등록권자, 서지정보 | 7개 |
| 해외 특허 | 키워드, 출원번호, 국제공개번호, 출원인, 국제출원번호 | 5개 |
| 기타 50개 서비스 | docs 참조하여 동적 호출 가능 | 552개 |

## 설치

### 1. API 키 발급

- [KIPRIS Plus](https://plus.kipris.or.kr) 회원가입 후 API 키 발급
- 또는 [공공데이터 포털](https://www.data.go.kr)에서 활용 신청

### 2. 환경변수 설정

```bash
export KIPRIS_API_KEY="발급받은_API_키"
```

셸 프로필(`~/.zshrc` 등)에 추가하면 영구 적용됩니다.

### 3. Skill 등록

이 저장소를 clone 한 후, `SKILL.md` 파일을 Claude Code skills 디렉토리에 심볼릭 링크합니다:

```bash
# 저장소 clone
git clone <이_저장소_URL> ~/dev/kipris_skill

# skills 디렉토리 생성 (없는 경우)
mkdir -p ~/.claude/skills

# 심볼릭 링크 생성
ln -s ~/dev/kipris_skill/SKILL.md ~/.claude/skills/kipris.md
```

또는 프로젝트별로 사용하려면:

```bash
mkdir -p /path/to/project/.claude/skills
ln -s ~/dev/kipris_skill/SKILL.md /path/to/project/.claude/skills/kipris.md
```

## 사용법

Claude Code에서 `/kipris` 명령으로 스킬을 호출합니다:

```
/kipris 인공지능 관련 특허를 검색해줘
/kipris 삼성전자가 출원한 특허를 찾아줘
/kipris 출원번호 1020200123456의 상세정보
/kipris artificial intelligence 미국 특허 검색
```

또는 자연어로 요청하면 자동으로 적절한 오퍼레이션이 선택됩니다.

## 문서 구조

```
├── SKILL.md                    # 스킬 본체 (Single Source of Truth)
├── CLAUDE.md                   # 프로젝트 컨텍스트
├── README.md                   # 이 파일
└── docs/
    ├── README.md               # API 명세 인덱스 (52개 서비스)
    └── services/               # 서비스별 상세 명세
        ├── patent_utility.md   # 특허·실용 (61 ops)
        ├── foreign_patent.md   # 해외특허 (81 ops)
        ├── design.md           # 디자인 (51 ops)
        ├── trademark.md        # 상표 (54 ops)
        └── ...                 # 총 52개 파일
```

## 라이선스

API 데이터는 [KIPRIS Plus 이용약관](https://plus.kipris.or.kr)을 따릅니다.

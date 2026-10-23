# code-flow

프로젝트의 구조와 기능 흐름을 한국어로 설명해 주는 Claude 스킬.

## 기능
1. **전체 지도** — "이 프로젝트 뭐 있어?" → 기능 목록(로그인, 회원가입, 게시판 등)과 핵심 파일
2. **기능 흐름** — "로그인 설명해줘" → 요청이 지나가는 순서와 파일·함수별 역할
3. **주석** — 요청할 때만, 블록 단위 흐름 주석(① ② ③, ← →)을 파일에 반영

기본은 파일을 수정하지 않는 설명이며, 코드에서 직접 확인한 연결 관계만 말한다.

## 설치
Claude Code 플러그인으로 설치 (한 줄):
```text
/plugin install code-flow --marketplace chltkdwns/code-flow
```

또는 마켓플레이스를 먼저 등록한 뒤 설치:
```text
/plugin marketplace add chltkdwns/code-flow
/plugin install code-flow@chltkdwns-skills
```

스킬만 설치:
```bash
npx skills add chltkdwns/code-flow
```

## 사용 예
- "이 프로젝트에 어떤 기능 있어?"
- "로그인 흐름 설명해줘"
- "이 파일 어디서 쓰여?"
- "이 함수에 주석 달아줘"

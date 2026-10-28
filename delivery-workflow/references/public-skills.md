# 공개 후보와 가져오기

이 문서는 후보 연결표이며 다운로드한 스킬 본문이 아니다. 설치 여부를 확인하거나 실제로 읽기 전에는 하위 스킬을 사용했다고 표현하지 않는다. 2026-10-28에 공개 원문을 확인한 후보들이다. 원격 main 브랜치는 변경될 수 있다.

| 역할 | 공개 폴더 | 함께 확인할 것 |
| --- | --- | --- |
| 설계 | https://github.com/obra/superpowers/tree/main/skills/writing-plans | 현재 과제에 필요한 계획 깊이, 관련 스킬 참조 |
| 제작 | https://github.com/obra/superpowers/tree/main/skills/executing-plans | 같은 세션의 구현 절차, 참조 파일과 후속 검토 지침 |
| 테스트 | https://github.com/obra/superpowers/tree/main/skills/test-driven-development | 실제 실패를 확인하는 테스트, 프로젝트의 기존 테스트 도구 |
| 검증 | https://github.com/obra/superpowers/tree/main/skills/verification-before-completion | 실행 증거와 요구사항 대조 |
| 보안 | https://github.com/openai/skills/tree/main/skills/.curated/security-best-practices | Python·JavaScript/TypeScript·Go와 해당 프레임워크 references |
| 오류 원인 추적 | https://github.com/obra/superpowers/tree/main/skills/systematic-debugging | 같은 폴더의 참고 자료와 TDD·검증 스킬 참조 |

## 필요한 경우에만 가져오는 절차

1. 같은 이름의 스킬이 이미 등록되어 있는지 확인하고, 있으면 설치 위치의 원문을 읽는다. 같은 이름이라는 이유만으로 출처와 버전이 같다고 가정하지 않는다.
2. 없는 후보는 위 공개 원본의 존재, 내용, 라이선스, 참고 파일·스크립트·다른 스킬 의존성을 확인한다. OpenAI skills 저장소에는 deprecated 안내가 있으므로 이동·폐기 여부를 함께 확인한다. 대체 출처를 추정해서 설치하지 않는다.
3. 네트워크·설치가 허용되면 현재 환경에서 지원하는 skill-installer 또는 공식 스킬 설치 방법으로 해당 폴더와 필요한 지원 파일을 가져온다. SKILL.md 하나만 복사해 scripts/references가 빠지지 않게 한다. 다운로드한 보조 스크립트는 필요한 경우 내용을 읽고 실행한다.
4. 후보 하나를 위해 전체 플러그인·시작 훅·외부 커넥터를 자동 활성화하지 않는다. 필요한 추가 의존성이 과제에 비해 크거나 규정과 충돌하면 통합 스킬의 기본 절차로 수행한다.
5. 가능하면 사용한 저장소 커밋과 폴더 경로를 기록한다. 현재 CLI가 실제로 발견하는지 확인하고 필요할 때 세션을 다시 시작한다. 단순 원문 읽기, 로컬 설치, 실제 스킬 실행을 구분한다.

공식 사용법: https://learn.chatgpt.com/docs/build-skills

공식 하위 에이전트 안내: https://learn.chatgpt.com/docs/agent-configuration/subagents

이 통합 스킬은 독립적으로 작성한 조율 지침이다. 위 프로젝트의 원문·코드·자산을 이 폴더에 재배포하지 않는다. 향후 함께 배포한다면 각 프로젝트의 라이선스·저작권 표시를 별도로 준수해야 한다. 설치와 실행은 현재 프로젝트 및 실행 환경의 도구·자료 이용 정책을 따른다.

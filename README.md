# codex-kit

Codex로 시간 제한이 있는 개발 과제를 수행할 때 쓰는 작업 지침과 스킬 모음이다. 과제 내용이나 정답 코드는 들어 있지 않고, 진행 방법만 담는다.

## 구성

- `AGENTS.md`: 작업 공간 전체에 적용할 기준(우선순위, 시간, 금지 사항, 검증, 기록)
- `skills/task-kickoff`: 과제를 읽고 PLAN.md를 만든다
- `skills/verify-before-done`: 완료라고 말하기 전에 실행 결과로 확인한다
- `skills/submission-docs`: 제출 문서를 쓰고 제출 직전 점검을 한다
- `skills/explain-my-work`: 작업 구조와 판단을 직접 설명할 수 있게 정리한다

## 사용 방법

작업 공간 터미널에서 실행한다.

```
git clone https://github.com/tember8003/codex-kit /tmp/codex-kit
mkdir -p ~/.codex && cp /tmp/codex-kit/AGENTS.md ~/.codex/AGENTS.md
```

`~/.codex/AGENTS.md`는 모든 작업 폴더에 적용되는 전역 지침이라 제출물 폴더에 섞이지 않는다. Codex 안에서 이 지침을 따르는지 한 번 물어 확인한다. 과제 폴더에 원래 있는 `AGENTS.md`는 그대로 두며, 그 파일이 더 구체적인 지침으로 우선한다.

스킬은 Codex 안에서 설치한 뒤 Codex를 다시 시작한다.

```
$skill-installer install https://github.com/tember8003/codex-kit/tree/main/skills/task-kickoff
$skill-installer install https://github.com/tember8003/codex-kit/tree/main/skills/verify-before-done
$skill-installer install https://github.com/tember8003/codex-kit/tree/main/skills/submission-docs
$skill-installer install https://github.com/tember8003/codex-kit/tree/main/skills/explain-my-work
```

`$skill-installer`를 쓸 수 없으면 `cp -r /tmp/codex-kit/skills/* ~/.codex/skills/`로 복사한다.

## 라이선스

MIT

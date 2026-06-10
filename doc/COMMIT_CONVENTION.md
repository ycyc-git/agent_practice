# Commit Convention

## 커밋 메시지 구조

```
<type> subject

body

footer
```

---

## Type

| 타입 | 설명 |
|------|------|
| `feat` | 새로운 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 수정 |
| `style` | 코드 포맷팅, 세미콜론 누락 등 (로직 변경 없음) |
| `refactor` | 코드 리팩토링 (기능 변경 없음) |
| `test` | 테스트 코드 추가 또는 수정 |
| `chore` | 빌드 설정, 패키지 매니저 등 기타 변경 |
| `ci` | CI/CD 설정 변경 |
| `perf` | 성능 개선 |
| `revert` | 이전 커밋 되돌리기 |

---

## Scope (선택)

변경 범위를 괄호 안에 작성합니다.

예: `feat(auth)`, `fix(api)`, `docs(readme)`

---

## Subject

- 50자 이내로 작성
- 마침표 없이 끝내기
- 명령문 형태로 작성 (과거형 사용 금지)
- **한글 사용 필수**
- 헤더(type)는 반드시 `< >` 문자로 감싸서 작성
  - 형식: `<type> 한글 메시지`
  - 예시: `<fix> 긴급Fix`

---

## Body (선택)

- 무엇을, 왜 변경했는지 설명
- 72자 단위로 줄바꿈
- subject와 한 줄 공백으로 구분

---

## Footer (선택)

- 이슈 번호 참조: `Closes #123`, `Refs #456`
- 브레이킹 체인지: `BREAKING CHANGE: <설명>`

---

## 예시

```
<feat> 소셜 로그인 기능 추가

Google, Kakao OAuth2 로그인을 지원하도록 구현.
기존 이메일 로그인과 병행 사용 가능.

Closes #42
```

```
<fix> 긴급Fix
```

```
<fix> 사용자 조회 시 null 반환 오류 수정
```

```
<docs> 커밋 컨벤션 초안 작성
```

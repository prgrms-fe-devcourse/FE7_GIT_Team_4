# 이제원
* 변수명 카멜케이스, 약자 및 단축어 사용
* 하드 탭

# 정진환
- 자간 2칸, 탭 4칸
- 브랜치 전략
  - 브랜치 네이밍 규칙
  ```feat/login, fix/payment-bug, hotfix/server-error```
- 커밋 메시지 규칙
  - 형식 (예: `<emoji>` `<type>`: `<message>`)
  - type 목록 정의
    - ✨ feat: 새로운 기능
	- 🐛 fix: 버그 수정
	- 🎨 style: 스타일 변경 (코드 로직 영향 없음)
	- 🧼 refactor: 리팩토링
	- 📝 docs: 문서 수정
	- ✅ test: 테스트 코드 추가/수정
	- 🧰 chore: 기타 작업
    
# 안수민
* 변수명: 카멜케이스
* 파일명: 소문자, 언더바로 연결 (뒤에 붙는 숫자는 그냥 붙임. 예: project1_sos.js)
* 커밋메시지: [20250901] - 커밋 내용
* pr 단위: 최대 하루 묶음
* pr 제목: [브랜치 하단 파일명] 대상 (예: [feat] 사이드바 컴포넌트)

## 브랜치 전략
- 기능별로 브랜치 생성: `feature/기능명`, `bugfix/버그명`
- 메인 브랜치(`main`)는 항상 배포 가능한 상태 유지
- 작업 브랜치는 짧게, 자주 `main`과 동기화

## 충돌 방지
- 메인 브랜치 변경 사항을 자주 pull & rebase
- 공통 파일(README, 설정 등) 수정 최소화
- 코드 스타일 통일
- 필요 시 임시/백업 브랜치 사용

## Pull Request(PR)
- PR 생성 전 기능 브랜치 최신화 (`git fetch` + `git rebase origin/main`)
- 리뷰 후 승인된 PR만 병합
- 충돌 발생 시 PR 내에서 해결

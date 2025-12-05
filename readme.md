# 1. 깃 커밋 템플릿 사용 하기
## 1.1. 깃 템플릿 등록 방법 
- 커밋 할 떄 `-m` 옵션을 사용 하지 않고 `git commit`만 입력 할 경우 
.gitmessage.txt 파일이 템플릿 으로 설정 됨
- 명령어 `git config commit.template .git/.gitmessage.txt`
- .git/.gitmessage.txt 파일 내용
```
# <타입>: <제목> (50자 이내)


# [타입 리스트] (각 행은 72자 이내)
# feat    : 기능 추가
# fix     : 버그 수정
# refactor: 리팩토링 (기능변경 X)
# style   : 스타일 (포맷팅, 세미콜론 등)
# docs    : 문서 수정
# test    : 테스트 코드
# chore   : 기타 빌드, 설정 등
# ci      : CI/CD(지속적 통합/배포) 설정 파일이나 스크립트 수정
#
# [본문] (선택사항: 무엇을, 왜 변경했는지) 


# [꼬리말] (선택사항: 이슈 번호 등. 예: #123)


# ---------------------------------------------------------
```

# 2. git commit 에디터 변경
- `git config core.editor "code --wait"` 터미널이 아닌 vs code로 커밋 메시지 입력 

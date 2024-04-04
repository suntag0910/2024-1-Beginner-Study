## git log   
- commit 기록을 최신 순으로 확인   
- **--oneline** 옵션을 사용하면 각 커밋을 한 줄 요약   

## Commit Id   
- commit의 식별을 위해 사용하는 40자 길이의 16진수   
- 중복 확률은 2의 80제곱 분의 1   
- SHA-1 해시 함수를 사용(SHA-1 해시 함수:입력을 받고 메시지 다이제스트라는 160비트(20바이트) 해시값을 만드는 암호화 해시 함수)   

## HEAD   
- HEAD는 현재 작업 중인 위치를 가리킴   
- 현재 작업 중인 브랜치의 가장 최근 commit   
- 다음 commit의 base가 되는 다음 commit   
- 새로운 commit이 생기면 HEAD도 변경   

## git status   
- 세 가지 상태에 따라 파일 분류하여 확인(Untracked, Changes not staged for commit, Changes to be commited)   

## commit --amend   
- 마지막 commit의 내용에 변경이 있을 때 사용   
- 완전히 새로운 commit으로 대체   
    - commit id가 바뀜
- vim으로 진입하여 commit 메시지를 수정하게 됨 (vim:vi 에디터를 향상시켜 만든 텍스트 편집기)   

## reset   
- commit을 제거하는데 사용   
- 3가지 옵션 존재(soft, mixed, hard)   
# soft   
- 커밋만 취소   
- 변경 사항이 Staging Area로 돌아감   
# mixed   
- 커밋을 취소   
- 변경 사항이 Working Directory로 돌아감   
# hard   
- 커밋을 취소   
- 변경 사항을 모두 제거하고 이전 커밋으로 돌아감   

## revert   
- commit을 제거하지 않고 되돌림   
- 되돌리기 위한 새로운 commit이 생성됨   
- --edit 옵션이 default
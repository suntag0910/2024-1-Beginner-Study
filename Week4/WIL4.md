### 브랜치 전략   
## Git Flow   
- 2010년에 Vincent Driessen이 고안한 방법   
- 브랜치를 관리하기 위한 전략   
# 브랜치 종류   
- main(master):프로젝트 생성 시 기본으로 생성되는 브랜치로 영원히 존재하는 첫 브랜치   
- develop:영원히 존재하는 두번째 브랜치, feature 브랜치의 기반이 되어 이 브랜치를 기준으로 Merge   
- feature:develop 브랜치에서 분기하여 작업, 기능 개발 완료 후 다시 develop으로 병합, 대부분의 이름 사용 가능   
- release:배포 준비를 위한 브랜치, 자잘한 버그 수정 및 QA(품질검사)를 함   
- hotfix:긴급히 수정이 필요할 때 사용, main(master) 브랜치에서 분기, main(master)과 develop 브랜치에 모두 병합해주어야 함   
## GitHub Flow   
- Git Flow가 배포가 수시로 이루어지는 현 시대의 웹앱과는 부적합하다고 판단되어 사용되는 전략   
# 브랜치 종류   
- main(master):항상 배포 가능 상태로 유지, 병합 전에 충분한 test 필요   
- feature:main(master) 브랜치에서 분기하여 main(master) 브랜치로 병합, 브랜치의 목적을 이름에 잘 담아야하고 코드 리뷰가 중요함   
# 그 외 전략   
- GitLab 전략:복잡한 GitFlow와 너무 간단한 GitHub Flow의 절충안   
## 가져야할 태도,자세   
- convention 활용   
- 구글링 꼼꼼히   
- 코드에 대한 주인 의식   
- 질문 활용    
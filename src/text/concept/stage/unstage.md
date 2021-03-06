---
layout: home
title: "스테이지"
keyword: "스테이지"
breadcrumb:
- "text"
- "concept"
- "stage"
---

# 파일의 stage 상태와 unstage 상태
---
워킹 디렉터리에 있는 tracked 상태의 파일들은 스테이지 영역과 긴밀한 상관관계를 맺습니다.  
스테이지 영역으로 등록된 모든 파일은 untracked 상태에서 tracked 상태로 변경됩니다.  
스테이지는 워킹 디렉터리 안에 있는 파일들의 추적 상태를 관리하는 역할을 수행합니다.  

<br>

## 상태구분
---
스테이지 영역은 파일을 stage 상태와 unstage 상태로 구분합니다. 
깃이 변화 이력을 기록하려면 파일들의 최종 상태가 stage 상태여야 합니다.  
unstage 상태라면 파일에 변화가 있다는 것을 의미합니다.   

즉, 스테이지 영역에 있는 파일과 워킹 디렉터리 안에 있는 파일 내용에 차이가 있을 때는 unstage 상태가 됩니다.  

또 넓게 보면 아직 스테이지 영역으로 등록하지 않은 워킹 디렉터리 안의 파일도 unstage 상태라고 생각할 수 있습니다.  
이때는 unstage 상태이자 동시에 untracked 상태입니다.  

unstage 상태라고 해서 실제 파일이 없어지는 것은 아닙니다. 단지 파일이 수정되어 임시적으로 스테이지 목록에서 제외된 것입니다. 
`git add` 명령어를 사용하면 스테이지에 다시 추가할 수 있습니다.  

<br>
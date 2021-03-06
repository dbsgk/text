---
layout: home
title: "gitignore"
keyword: "gitignore"
breadcrumb:
- "text"
- "concept"
- "file"
---

# .gitignore 파일
---
`.gitignore`는 git과 ignore(무시하다)의 합성어입니다.  

<br>

## 생성위치
---
`워킹 디렉터리` 루트에 `.gitignore` 파일을 생성합니다.  
이 파일은 앞에 점(.)이 있어 숨겨진 파일로 관리됩니다.  

<br>

## 제외목록
---
`.gitignore` 파일은 깃에서 관리하지 않는 파일들의 `목록`을 가지고 있습니다.  
깃은 이 파일에 작성된 목록들을 `추적하지 않습니다`.  
또 로컬 저장소를 서버로 전송하거나 다른 사람과 공유할 때도 이를 `분리`하여 처리합니다.  

<br>

## 작성방법
---
`.gitignore` 파일은 `텍스트 에디터`를 이용하여 간단하게 작성할 수 있습니다.  
특별한 도구 없이 파일 이름만 .gitignore로 만들면 됩니다.  

깃에서 제외할 파일 목록을 직접 적어 주거나 `규칙`을 사용하여 나열할 수 있습니다.  
.gitignore 파일을 작성할 때는 저장소 폴더의 최상위 디렉터리에 두어야 합니다.  

<br>
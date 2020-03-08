---
layout: home
---
# 깃의 내부
깃의 동작원리를 이해하기 위해서는 HEAD파일, index파일, objects 디렉터리, refs 디렉터리에 대한 상세한 구조와 파일에 대해서 학습이 필요합니다.

## Content addressable
깃은 컨덴츠를 기반으로 주소를 생성하고 파일 관리를 합니다. 깃은 모든 컨덴츠를 디렉토리와 파일 형태로 관리하기 때문에 마치 파일 시스템과도 유사합니다. 초창기 깃 1.5 이전의 버전의 경우 이러한 파일처리 특성 때문에 사용하기가 쉽지 않았습니다.

대부분의 명령들은 저수준으로 처리되었습니다. 최근들어 고수준의 명령들을 제공하고 쉽게 접근이 가능해졌습니다.

하지만 컨덴츠를 기반으로 디렉토리와 파일명을 생성하고, 이를 관리하는 것은 매우 매력적인 방법입니다. 필자 또한 이분분에 대한 깊은 감명을 받았습니다.

## 저장소 구조
깃 저장소에는 깃의 내부관리를 위해서 여러 파일들이 존재를 합니다. 각 디렉토리와 파일들은 특별한 의미들을 가지고 있습니다. 

```
infoh@DESKTOP-VAKLOFQ MINGW64 /e/gitstudy19 (master)
$ ls .git -F1
config
description
HEAD
hooks/
info/
objects/
refs/
```

깃 저장소의 내부 입니다. 저장소에는 여러 개의 파일이 있는 것을 확인해 볼 수 있습니다. 이중에서 가장 집중해서 봐야 할 4가지 항목이 있습니다.

### Objects
Objects 디렉터리는 깃의 컨덴츠 객체들을 담고 있습니다.

### Refs
Refs는 커밋들의 포인터를 담고 있습니다.

### HEAD
HEAD는 현재 체크아웃된 브랜치의 커밋 포인터를 담고 있습니다.

### Index
Index 파일은 스테이지 영역의 정보를 담고 있습니다.

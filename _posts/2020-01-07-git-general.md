---
title: 'git general command'
layout: post
tags:
  - development
category: development
---

```git
이력을 그래프로 보여주는 명령어
git log --decorate --all --oneline --graph  

원격 설정
git remote add origin https://github.com/parduck/redux-ex.git

원격 origin 에 local master branch push
git push -u origin master
```

```git
git pull origin "branch name" --allow-unrelated-histories
```

refusing to merge unrelated histories

이 명령 옵션은 이미 존재하는 두 프로젝트의 기록(history)을 저장하는 드문 상황에 사용된다고 한다. 
즉, git에서는 서로 관련 기록이 없는 이질적인 두 프로젝트를 병합할 때 기본적으로 거부하는데, 이것을 허용해 주는 것이다.

<pre>
<code>
설정된 버전 확인
git remote -v

버전으로 reset.. 상세한건 fetch_reset에...
git reset --hard "버전"
</code>
</pre>
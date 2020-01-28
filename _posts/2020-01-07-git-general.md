---
title: 'git general command'
layout: post
tags:
  - development
category: development
---

```git
git log --decorate --all --oneline --graph

git remote add origin https://github.com/parduck/redux-ex.git

git push -u origin master
```

>git pull origin 브런치명 --allow-unrelated-histories
>refusing to merge unrelated histories
>이 명령 옵션은 이미 존재하는 두 프로젝트의 기록(history)을 저장하는 드문 상황에 사용된다고 한다. 즉, git에서는 서로 관련 기록이 없는 이질적인 두 프로젝트를 병합할 때 기본적으로 거부하는데, 이것을 허용해 주는 것이다.

<pre>
<code>
git remote -v

git reset --hard "버전"
</pre>
</code>
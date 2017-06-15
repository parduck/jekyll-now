---
title: 'git fetch, reset'
layout: post
tags:
  - git
category: dev
---
처음 remote저장소(github)에서 로컬에 소스를 당겨올때.
pull 하면 merge 관련 오류등이 나는 경우.

{% highlight git %}
 git fetch -all
 git reset --hard origin/master
{% endhighlight %}

1. git fetch -all
최신 remote 소스를 merge나 rebase 없이 다운로드함

[fetch](https://git-scm.com/book/ko/v1/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-%EB%A6%AC%EB%AA%A8%ED%8A%B8-%EB%B8%8C%EB%9E%9C%EC%B9%98)

2. git reset --hard origin/master
마스터 브랜치를 fetch해온 정보로 reset 함. 
예전 정보(commit or staged)는 날라감.
stash와 commit을 하거나 branch를 만들어 놓아 기존 소스 날리는 것을 방지.
fetch 전에 git branch new-branch

[reset](https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-Reset-%EB%AA%85%ED%99%95%ED%9E%88-%EC%95%8C%EA%B3%A0-%EA%B0%80%EA%B8%B0)


---
title: github page setting
author: choieunji
date: 2020-08-27 11:07:00 +0800
categories: [Blogging, github_page]
tags: [writing, github]
---

## github page setting

블로그를 보다보면 계정명.github.io 라는 주소로 되어있는 블로그들이 눈에 자주 보이는데
github blog 세팅 후 공부하면서 찾은 내용, 공유하고 싶거나 정리하고 싶은 내용들을 가끔씩 포스팅 하고자 합니다!
우선 이 블로그를 세팅하기 위해 jekyll을 사용한다. jekyll에 들어가면 다양한 테마들이 많은데 내가 fork해온 테마는
(https://github.com/choieunii/jekyll-theme-chirpy)
이 테마이다. 

## setting 방법

세팅방법을 간단히 정리하자면 다음과같다.
1. fork해온뒤 clone
2. 루비가 깔려있지 않다면 루비설치
3. bundle install
4. config.yml 수정
5. jekyll serve -> 로컬에서 서버구동하여 localhost:4000으로 접속하면 확인이 가능하다.
6. 마지막으로 본인의 github repository에 push하면된다.

## Error 해결

내 컴퓨터에는 루비가 설치되어있지 않기에 처음에 루비설치를 먼저 진행하였다.
ruby 설치는 chocolatey를 사용하여
```
choco install ruby
choco install ruby2.devkit
```
순서로 입력후 jekyll을 설치
```
gem install jekyll
```

그러나 에러발생...에러를 해결못하고 헤매다가 구글링후 chocolatey를 사용하지 않고 ruby설치를 진행하였다.

ruby가 잘설치완료!!
그러면 자신이 clone해온 테마의 폴더로 가서
```
bundle install
jekyll serve
```
를 하게되면 자신의 local에서 잘 구동이 되는것을 확인가능하다.

구동이 잘되는것을 확인하였다면
push 한다!!

---
title: terminal 새창 열 때 동작 등록
---

# terminal 새창 열 때 동작 등록
* terminal 새창을 열 때 특정 동작을 등록 할 수 있다. 
* env와 같은 값을 설정 할 수 있다. 
* 이외의 bash script를 실행 할 수 있도록 할 수 있다. 
* user에 따라 커스터 마이징 해서 사용 할 수 있다.

# How to 
## step 1
`.bash_profile`가 존재 하지 않을 경우, 만들어 준다.
```bash
$ vi ~/.bash_profile
```

## step 2
`bash_profile`에 원하는 command를 입력해준다.

## step 3 
terminal 열기 또는 source .bash_profile를 통하여 테스트 해본다.

# Test View
![View](../images/posts/terminal-bashrc/image1.gif)

# Add information
`.bashrc` 이외에 `.bash_profile`, `profile`, `/etc/bashrc` 등이 추가로 있다. 해당 파일의 기본 설정 호출 순서는 다음과 같다.
1. /etc/profile → /etc/profile.d/test.sh
2. ~/.bash_profile → ~/.bashrc → /etc/bashrc
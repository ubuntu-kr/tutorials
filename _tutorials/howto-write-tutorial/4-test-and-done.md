---
layout: tutorial
category: 튜토리얼 작성하기
title: 4. 테스트 하고 마무리 하기
order: 4
---

미리 설치한 `jekyll` 를 이용하여, 튜토리얼이 사이트에서 잘 보이는지 테스트 합니다. 먼저 터미널을 열고, 로컬에 복제한 튜토리얼 저장소 디렉토리에 접근합니다.

그리고 아래와 같은 명령을 실행하여 Jekyll 테스트 서버를 시작합니다.

```bash
bundle exec jekyll serve
```

그리고, 웹 브라우저를 열고 http://127.0.0.1:4000/tutorials/ 에 접속하여, 작성한 튜토리얼이 잘 나오는지 확인합니다.

확인 후, 커밋과 푸시로 마무리 합니다. Fork 된 저장소에 푸시 한 경우, [원래 저장소 페이지](https://github.com/skhu-sw/tutorials) 에서 Pull Request 를 엽니다.

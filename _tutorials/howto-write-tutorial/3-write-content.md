---
layout: tutorial
category: 튜토리얼 작성하기
title: 3. 내용 작성
order: 3
---
개요 페이지를 작성한 후, 본격적으로 튜토리얼의 단계 별로 페이지를 만들어 작성합니다.
단계별 페이지 파일 이름은 `<단계>-<단계 제목>.md` 로 구성합니다. (예 : `1-start.md`)   
개요 페이지를 작성할 때 처럼, 가장 앞에 `YAML Front Matter` 를 넣어 줍니다.
다만, `tutorial_desc`, `tutorial_authors` 는 넣지 않습니다.   
`category`는 개요 페이지의 것과 동일한 것으로 해 줘야 하며, `order` 는 순서에 맞는 숫자를 넣어줍니다.

> 예제   

```
---
layout: tutorial
category: 튜토리얼 작성하기
title: 3. 내용 작성
order: 3
---
```

마찬가지로 `YAML Front Matter` 바로 아래에 마크다운 문법에 따라 내용을 작성합니다.

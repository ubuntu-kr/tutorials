---
layout: tutorial
category: 튜토리얼 작성하기
title: 2. 개요 페이지 작성
order: 2
---
모든 튜토리얼의 첫 페이지는 개요 입니다. 개요는 튜토리얼에 대한 요약된 정보를 보여줍니다.

  - 먼저 `_tutorials` 디렉터리 안에 새 디렉터리를 만듭니다.
    - 디렉터리 이름은 영어로 하길 권장합니다. 새로 만들 디렉터리에 튜토리얼 문서 파일이 들어갑니다.
  - 개요 페이지 파일을 생성합니다. 파일 이름은 `0-intro.md` 로 하길 권정합니다.
  - 개요 페이지 파일을 텍스트 편집기로 엽니다.

개요 페이지 파일을 열었으면, 튜토리얼에 대한 정보를 먼저 입력합시다. 아래와 같은 내용으로 `YAML Front Matter` 를
문서의 가장 앞에 넣습니다.

```
---
layout: tutorial
category: <튜토리얼 제목>
tutorial_desc: <튜토리얼 설명>
tutorial_authors:
  - <튜토리얼 작성자>(<작성자 추가정보>)
title: 이 단계의 제목
order: <단계의 순서>
---
```

아래는 지금 보고 있는 튜토리얼의 개요 페이지에 있는 `YAML Front Matter` 입니다.
```
---
layout: tutorial
category: 튜토리얼 작성하기
tutorial_desc: 새로 튜토리얼 문서를 작성하는 방법을 알아봅시다.
tutorial_authors:
  - 한영빈(sukso96100@gmail.com)
title: 0. 개요
order: 0
---
```

  - `layout` : 페이지 레이아웃을 지정합니다. `tutorial` 로 하여 튜토리얼 레이아웃으로 해 줍니다.
  - `category` : 카테고리 입니다만, 이 사이트 에서는 여러 단계로 나눠진 튜토리얼 문서들을 묶는 역할이자 튜토리얼의 제목 역할을 합니다.
  - `tutorial_desc` : 튜토리얼에 대한 간단한 설명입나다. 개요 페이지에만 넣어줍니다.
  - `tutorial_authors` : 튜토리얼 작성자 목록입니다. 개요 페이지에만 넣어줍니다.
  - 여려명을 작성자로 포함하려면, 다음과 같은 형식으로 작성합니다.
  ```
  tutorial_authors:
    - 홍길동(hong@example.com)
    - 2MB(2mb@example.com)
    - Elon Musk(musk@example.com)
  ```
  - `title` : 페이지 제목이자 단계의 제목입니다.
  - `order` : 단계의 순서 번호(Index) 입니다. 개요 페이지의 `order` 는 항상 0 입니다.

  `YAML Front Matter` 작성 후에는 바로 하단에 페이지 내용을 작성합니다. 첫 페이지는 개요 페이지 이므로,
  튜토리얼에 대한 소개, 튜토리얼을 통해 무엇을 배울 수 있는지, 튜토리얼을 따라하려면 무엇이 필요한지 정도를 작성합니다.
  내용은 마크다운 문법에 따라서 작성합니다.

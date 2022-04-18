---
title: localhost MD로 블로그 글쓰기
description: localhost 글쓰기라 login 관리가 필요없다... 하지만 md 문법을 알아야한다.
img: https://images.unsplash.com/reserve/LJIZlzHgQ7WPSh5KVTCB_Typewriter.jpg?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=60
alt: my first blog post
author: 
  name: 김태성
  bio: finiview server Team publisher
  img: https://images.unsplash.com/photo-1533636721434-0e2d61030955?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2550&q=80
tags: 
  - nuxtjs
  - javascript
  - mdx
---

글쓰기는 ide에서 직접 작성할 수도 있으며, dev를 실행시켜 프론트화면에서 직접 작성 할 수도 있다. 하지만 새 글을 작성하기 위해서는 새로운 md파일을 작성하기 때문에 결국 ide를 사용하는 것이 가장 효율적이다.

## This is a heading
This is some more info
<div class="bg-blue-500 text-white p-4 mb-4">
  This is HTML inside markdown that has a class some classes
</div>

<info-box>
  <template #info-box>
    This is a vue component inside markdown using slots
  </template>
</info-box>

```js[nuxt.config.js]
export default {
  nuxt: "is the best"
}
```
```html[my-first-blog-post.md]
<p>code styling is easy</p>
```

### This is a sub heading
This is some more info

### This is another sub heading
This is some more info

## This is another heading
This is some more info

### html을 이용한 이미지 추가
<div>
  <img src="/pikicast1186117392.jpg" alt="">
</div>

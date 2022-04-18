---
title: nuxt content 를 이용한 Blog 관리
description: content 를 이용해 md 문서를 작성하고 localhost liveview 로 편집을 할 수 있다.
img: /images/bg-studio.png
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

Welcome to my first blog post using content module

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

## html tag 를 이용한 image 출력
<div>
	<img src="/images/images.png" alt="테스트 이미지">
</div>

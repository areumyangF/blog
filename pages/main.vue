<template>
  <div class="main-container">
    <NavBar />
    <FirstWrap />
    <SecondWrap />
  </div>
</template>

<script>
import NavBar from '@/components/Landing/Navbar'
import FirstWrap from '@/components/Landing/FirstWrap'
import SecondWrap from '@/components/Landing/SecondWrap'
export default {
  name: 'index',
  components: {
    FirstWrap,
    SecondWrap,
    NavBar
  },
  head() {
    return {
      title: 'nuxt content 를 이용한 Blog 관리',
      meta: [
        {
          hid: 'description', // nuxt 의 hid 라는 유니크한 식별자를 통해 meta 태그를 덮어 씌어준다.
          name: 'description',
          content:
            'content 를 이용해 md 문서를 작성하고 localhost liveview 로 편집을 할 수 있다.'
        },
        {
          hid: 'keywords',
          name: 'keywords',
          content: ['nuxtjs', 'javascript', 'mdx']
        },
        {
          hid: 'og:title',
          property: 'og:title',
          content: 'nuxt content 를 이용한 Blog 관리'
        },
        {
          hid: 'og:description',
          property: 'og:description',
          content:
            'content 를 이용해 md 문서를 작성하고 localhost liveview 로 편집을 할 수 있다.'
        },
        {
          hid: 'og:image',
          property: 'og:image',
          // content: 'http://placeimg.com/640/480/fashion'
          content: '/images/bg-studio.png'
        }
      ],
      link: [
        {
          hid: 'canonical',
          rel: 'canonical',
          href: this.meta.url
        }
      ]
    }
  }
}
</script>

<style>
@import '@/assets/css/font.css';

body {
  font-family: HallymGothic-Regular, Arial, Verdana, Tahoma, sans-serif;
}
video {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
button,
ul,
li {
  outline: 0;
  border: 0;
  cursor: pointer;
}
.main-button {
  position: relative;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  margin: 1px 0 0;
  white-space: nowrap;
  font-size: var(--btn-font-size-l);
}

.main-container {
  width: 100%;
  height: 100vh;
  overflow-y: scroll;
  scroll-snap-type: y mandatory;
}
.main-wrapper {
  position: relative;
  scroll-snap-align: center;
  scroll-snap-stop: always;
}

h1,
h2,
h3,
h4,
h5,
h6,
span,
p {
  word-break: keep-all;
  white-space: pre-wrap;
}
</style>

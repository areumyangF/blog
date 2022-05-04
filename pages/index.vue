<template>
  <div class="main-container">
    <NavBar />
    <FirstWrap />
    <SecondWrap />
  </div>
</template>

<script>
import NavBar from '../components/Landing/Navbar.vue'
import FirstWrap from '../components/Landing/FirstWrap'
import SecondWrap from '../components/Landing/SecondWrap'
export default {
  name: 'index',
  components: {
    FirstWrap,
    SecondWrap,
    NavBar
  }
}
</script>

<style>
@import '../assets/css/font.css';

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

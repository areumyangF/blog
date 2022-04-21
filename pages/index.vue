<template>
  <FirstWrap>
  </FirstWrap>
</template>

<script>
import FirstWrap from "@/components/Landing/FirstWrap";
export default {
  name: "index",
  components:{
    FirstWrap
  }
}
</script>

<style>
@font-face {
  font-family: 'SpoqaHanSansNeo-Regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2108@1.1/SpoqaHanSansNeo-Regular.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
h1 {
  font-family: SpoqaHanSansNeo-Regular, Arial, Verdana, Tahoma, sans-serif;;
}
video {
  object-fit: cover;
  width: 100%;
  height: 100%;
}
button {
  outline: 0;
  border: 0;
}
.link-button {
  background-color: var(--token-tds-color-grey-opacity-800, var(--adaptiveOpacity800, rgba(0, 12, 30, 0.8)));
  color: white;
  padding: 10px 20px 10px 17px;
  position: relative;
  display: inline-flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
</style>

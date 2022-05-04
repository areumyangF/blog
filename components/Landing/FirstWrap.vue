<template>
  <div class="main-wrapper">
    <video muted playsinline autoplay>
      <source src="@/assets/video/toss-im-web-intro.mp4" type="video/mp4" />
    </video>

    <div class="gradient"></div>
    <div class="content-wrapper">
      <div class="content-sub-wrapper">
        <h1>{{ $t('main.title') }}</h1>
        <div class="button-wrapper">
          <button class="link-button main-button">
            <img
              src="https://static.toss.im/png-icons/timeline/applekorea.png"
            />
            App Store
          </button>

          <button class="link-button main-button">
            <img
              src="https://static.toss.im/png-icons/timeline/googleplay.png"
            />
            Google Play
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.main-wrapper {
  height: 100vh;
}
.gradient {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 500px;
  background: linear-gradient(
    180deg,
    white 0%,
    white 59px,
    rgba(255, 255, 255, 0) 100%
  );
}
.content-wrapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  -webkit-box-align: center;
  align-items: center;
  display: flex;
  flex-direction: column;
  -webkit-box-pack: justify;
  justify-content: space-between;
  animation: 0.5s ease-in-out 0s 1 normal forwards running animation-8hxyql;
}
.content-sub-wrapper {
  margin-top: 170px;
  -webkit-box-align: center;
  align-items: center;
  display: flex;
  flex-direction: column;
  -webkit-box-pack: start;
  justify-content: flex-start;
}
.content-sub-wrapper > h1 {
  width: 100%;
  text-align: center;
  margin-bottom: 50px;
  font-size: 64px;
  font-weight: 900;
  line-height: 1.4;
}
.link-button {
  background-color: var(
    --token-tds-color-grey-opacity-800,
    var(--adaptiveOpacity800, rgba(0, 12, 30, 0.8))
  );
  color: white;
  font-weight: 600;
  border-radius: 30px;
  height: 56px;
  padding: 15px 28px;
}
.link-button > img {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}
</style>

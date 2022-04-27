<template>
  <div class="main-wrapper">
    <p class="detail">{{ $t('main.detail') }}</p>
  </div>
</template>

<style scoped>
.main-wrapper {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
.detail {
  text-align: center;
  font-size: 25px;
  font-weight: 600;
  line-height: 1.8;
  color: #191f28;
}
</style>

<template>
    <div class="navbar-wrapper">
        <div class="navbar-container">
            <img src="https://webpds.saramin.co.kr/pds/united_company/logo/68137_logo.png"/>
            <div>
                <ul class="language-menu">
                    <li><nuxt-link :to="switchLocalePath('ko')">KOR</nuxt-link></li>
                    <span>|</span>
                    <li><nuxt-link :to="switchLocalePath('en')">ENG</nuxt-link></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.navbar-wrapper {
    position: fixed;
    width: 100%;
    height: var(--navbar-height);
    z-index: var(--nav-index);
    border-bottom: 1px solid transparent;
    background-color: var(--white);
    left: 0;
    transition: background-color .2s ease;
}
.navbar-container {
    max-width: 1140px;
    width: 100%;
    height: 100%;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.navbar-container > img {
    height: 85%;
}

.language-menu {
    display: flex;
}
.language-menu > span {
    margin: 0 10px;
}
</style>
<script setup>
import { siteText } from "@/constants/index";
</script>

<template>
    <section id="site">
        <div class="site__inner">
            <div class="site__title">
                Site Coding <em>나의 작업물</em>
            </div>
            <div class="site__wrap">
                <div :class="['site__item', 's' + (key + 1)]" v-for="(site, key) in siteText" :key="key">
                    <span class="num">{{ key + 1 }}.</span>
                    <div class="text">
                        <div>{{ site.text[0] }}</div>
                        <div>{{ site.text[1] }}</div>
                        <div>{{ site.text[2] }}</div>
                    </div>
                    <h3 class="title">{{ site.title }}</h3>
                    <div class="btn">
                        <a href="#">{{ site.code }}</a>
                        <a href="#">{{ site.view }}</a>
                    </div>
                    <div class="info">
                        <span>{{ site.info[0] }}</span>
                        <span>{{ site.info[1] }}</span>
                        <span>{{ site.info[2] }}</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- //site -->
</template>

<style lang="scss">
.site__inner {
    padding: 16px;
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    background-color: var(--mainBg-color);
}

.site__title {
    position: sticky;
    top: 70px;
    left: 0;
    width: 48%;
    height: 5vw;
    font-size: 4vw;
    font-weight: 900;
    line-height: 1.6;
    text-transform: uppercase;
    font-family: var(--mainNum--font);
    border-bottom: 0.4vw solid var(--white500);
    color: var(--white500);
    left: 0;
}

.site__title em {
    font-size: var(--mainNum--font);
    font-size: 1.25rem;
    font-weight: 400;
    display: inline-block;
    color: var(--white500);
}

.site__wrap {
    margin-top: 5vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

}

.site__item .num {
    font-family: var(--mainKor-font);
    font-size: 5vw;
    line-height: 1;
    font-weight: 900;
    color: var(--black);
    position: absolute;
    left: 1vw;
    top: 1vw;
}

.site__item .text {
    text-align: center;
    margin-bottom: 1rem;

}

.site__item .text>div {
    font-size: 3vw;
    line-height: 1;
    font-weight: 900;
    text-transform: uppercase;
    text-decoration: underline;
    font-family: var(--mainPop-font);
}

.site__item .title {
    font-family: var(--mainNum--font);
    font-family: var(--mainKor-font);
    margin-bottom: 1rem;
}

.site__item .btn a {
    text-decoration: underline;
    text-transform: uppercase;
    color: var(--black);
    font-size: 1rem;
    transition: all 0.3s;
}

.site__item .btn a:hover {
    color: var(--black);
}

.site__item .info {
    position: absolute;
    left: 0;
    bottom: 3%;
    width: 98%;
    margin-left: 1%;
    border-top: 1px solid var(--black);
    border-bottom: 1px solid var(--black);
    display: flex;
    justify-content: space-between;
}

.site__item .info span {
    font-family: var(--mainNum--font);
    font-size: 12px;
    padding: 3px 0;
    text-transform: uppercase;
}

.site__item {
    height: 70vh;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    position: sticky;
    left: 0;
}

.site__item.s1 {
    padding: 5vw 5vh;
    height: 80vh;
    width: 100%;
    background-color: #9f9a95;
    top: 180px;
}

.site__item.s2 {
    padding: 5vw 5vh;
    height: 80vh;
    width: 100%;
    background-color: #c0bab3;
    top: 200px;
}

.site__item.s3 {
    padding: 5vw 5vh;
    height: 80vh;
    width: 100%;
    background-color: #e4ded7;
    top: 220px;
}

.site__item.s4 {
    padding: 5vw 5vh;
    height: 80vh;
    width: 100%;
    background-color: #e4ded7;
    top: 240px;
}

.site__item .link a {
    border: 1px solid #000;
    width: 100%;
    height: 200px;
    padding: 10px;
}
</style>
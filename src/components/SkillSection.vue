<script setup>
import { skillText } from "@/constants/index";
</script>

<template>
    <section id="skill">
        <div class="skill__inner">
            <h2 class="skill__title">
                challenge <em>나의 도전</em>
            </h2>
            <div class="skill__desc">
                <div v-for="(skill, key) in skillText" :key="key">
                    <span>1.</span>
                    <h3>{{ skill.title }}</h3>
                    <p>{{ skill.desc }}</p>
                </div>
            </div>
        </div>
    </section>
    <!-- //skill -->
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Archivo+Black&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@100;200;300;400;500;600;700;800;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Racing+Sans+One&display=swap');



.skill__inner {
    padding: 16px;
    display: flex;
    justify-content: space-between;
    background-color: var(--mainBg-color);
}

.skill__title {
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
}

.skill__title em {
    font-size: var(--mainNum--font);
    font-size: 1.25rem;
    font-weight: 400;
    display: inline-block;
    color: var(--white500);
}

.skill__desc {
    width: 50%;
}

.skill__desc span {
    font-family: var(--mainKor-font);
    font-size: 5vw;
    line-height: 1;
    font-weight: 900;
    color: var(--white500);
}

.skill__desc h3 {
    font-size: 1.5rem;
    text-decoration: underline;
    text-underline-position: under;
    margin-bottom: 1vw;
    color: var(--white500);
    font-family: var(--mainNum--font);
}

.skill__desc p {
    font-size: 15px;
    color: var(--white500);
    margin-bottom: 30vh;
    font-family: var(--mainNum--font);

}

@media(max-width: 800px) {
    .skill__inner {
        flex-direction: column;
    }

    .skill__title {
        width: 100%;
        margin-bottom: 10vw;
        height: auto;
        background-color: var(--mainBg-color);
    }

    .skill__desc {
        width: 100%;
    }

    .skill__desc h3 {
        font-size: 18px;
    }

    .skill__desc p {
        font-size: 14px;
        font-weight: 400;
    }

    .skill__desc span {
        font-size: 20vw;
    }
}
</style>
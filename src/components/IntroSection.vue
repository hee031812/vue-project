
<template>
    <section id="intro">
        <div class="intro__inner">
            <h1 class="intro__title">
                CREATIVE DEVELOPER
            </h1>
            <div class="intro__lines" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>
            <div class="intro__text">
                <div class="text">
                    <div>The <em>world</em></div>
                    <div>turns</div>
                    <div>to <em>creativity</em></div>
                </div>
                <div class="img"></div>
            </div>
            <div class="intro__lines bottom" aria-hidden="true">
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
                <span class="line"></span>
            </div>
        </div>

    </section>
    <!-- //intro -->
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Archivo+Black&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@100;200;300;400;500;600;700;800;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Racing+Sans+One&display=swap');

#intro {
    height: 100vh;
}

.intro__inner {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: flex-start;
    justify-content: flex-end;
    background-color: var(--mainBg-color);
    flex-direction: column;
    padding: 1vw;
}

.intro__title {
    font-size: 7.6vw;
    text-transform: uppercase;
    font-family: "Archivo Black";
    color: var(--mainBg-fontcolor);
    text-align: center;
    line-height: 1;
    margin: 0 auto;
}

.intro__lines {
    width: 100%;
    display: block;
    /* margin: -1.5vw; */
    margin-bottom: -1.8vw;
    align-items: flex-start;
    justify-content: flex-end;
}

.intro__lines .line {
    display: block;
    height: 1px;
    background-color: var(--mainBg-fontcolor);
    margin: 0.5vw;
}

.intro__lines .line:nth-child(1) {
    height: 1px;
    background-color: var(--subGg200);
}

.intro__lines .line:nth-child(2) {
    height: 2px;
    background-color: var(--subGg200);
}

.intro__lines .line:nth-child(3) {
    height: 3px;
    background-color: var(--subGg200);
}

.intro__lines .line:nth-child(4) {
    height: 4px;
    background-color: var(--subGg300);
}

.intro__lines .line:nth-child(5) {
    height: 5px;
    background-color: var(--subGg300);
}

.intro__lines .line:nth-child(6) {
    height: 6px;
    background-color: var(--subGg400);
}

.intro__lines .line:nth-child(7) {
    height: 7px;
    background-color: var(--subGg500);
}

.intro__lines.bottom {
    display: none;
}

.intro__lines.bottom .line {
    display: block;
    height: 1px;
    background-color: var(--subGg100);
    margin: 0.5vw;
}

.intro__lines.bottom .line:nth-child(6) {
    height: 1px;
    background-color: var(--subGg200);
}

.intro__lines.bottom .line:nth-child(5) {
    height: 2px;
    background-color: var(--subGg200);
}

.intro__lines.bottom .line:nth-child(4) {
    height: 3px;
    background-color: var(--subGg200);
}

.intro__lines.bottom .line:nth-child(4) {
    height: 4px;
    background-color: var(--subGg300);
}

.intro__lines.bottom .line:nth-child(3) {
    height: 5px;
    background-color: var(--subGg300);
}

.intro__lines.bottom .line:nth-child(2) {
    height: 6px;
    background-color: var(--subGg400);
}

.intro__lines.bottom .line:nth-child(1) {
    height: 7px;
    background-color: var(--subGg500);
}

.intro__text {
    background-color: var(--subGg500);
    /* height: 37vh; */
    width: 100%;
    margin-top: 1.2vh;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    padding: 8vw 0;
}

.intro__text .text {
    font-size: 4.5vw;
    font-family: "Archivo Black";
    line-height: 0.9;
    color: var(--mainBg-fontcolor);
    z-index: 2;
    text-align: center;
    transition: all 0.3s;
}

.intro__text .img {
    background-image: url(../assets/img/Frame5.png);
    width: 18vw;
    height: 18vw;
    background-size: cover;
    border-radius: 50%;
    position: absolute;
    z-index: 1;
    filter: grayscale(100%);
    filter: opacity(85%);
}

/* .intro__text .img::after {
    background-image: url(../../img/Frame5.png);
    width: 18vw;
    height: 18vw;
    background-size: cover;
    border-radius: 50%;
    position: absolute;
    z-index: 1;
    filter: grayscale(100%);
    filter: opacity(85%);
    text-align: center;
    position: relative;
    cursor: pointer;
} */
.intro__text:hover {
    opacity: 0.2s;
}

.intro__text:hover .text {
    opacity: 0;
}

.intro__text:hover .text::after {
    opacity: 0;
}

.intro__text:hover {
    opacity: 0.2s;
}

.intro__text:hover .img {
    opacity: 0;
}

.intro__text:hover .img::after {
    opacity: 0;
}

@media(max-width:800px) {
    .intro__inner {
        align-items: center;
        justify-content: center;
    }

    .intro__lines.bottom {
        display: block;
    }

    .intro__text .text {
        font-size: 30px;
    }

    .intro__text .text>div:nth-child(1) {
        color: #351d1d;
    }

    .intro__text .text>div:nth-child(2) {
        color: #3a1717;
    }

    .intro__text .text>div:nth-child(3) {
        color: #240303;
    }

    .intro__text .img {
        width: 300px;
        height: 300px;
    }

    .intro__text .img::after {
        opacity: 0.3;
    }

}
</style>
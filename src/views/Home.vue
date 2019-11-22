<template>
    <div class="home">
        <div ref="box" class="box">
            <div class="container">
                <h1 id="title">Portfolio</h1>
                <p>Haruki Tosa</p>
            </div>
        </div>
        <div class="profile">
            <div class="info">
                <h2>Haruki Tosa</h2>
                <h3>2000/3/28</h3>
                <h3>github:<a href="https://github.com/harukitosa">@harukitosa</a></h3>
                <h3>twitter:<a href="https://twitter.com/tosa_now">@tosa_now</a></h3>
                <h3>Mail:13haruki28@gmail.com</h3>
            </div>
            <div class="language">
                <h3>プログラミング言語</h3>
                <div class="lang-1">
                    <h5>個人制作使用経験あり</h5>
                    <div class="row-container">
                        <p>Golang/Javascript/html/css</p>
                    </div>
                </div>
                <div class="lang-2">
                    <h5>学習経験あり</h5>
                    <div class="row-container">
                        <p>C/Java</p>
                    </div>
                </div>
            </div>
            <div class="language">
                <h3>フレームワーク</h3>
                <div class="lang-1">
                    <h5>個人制作使用経験あり</h5>
                    <div class="row-container">
                        <p>gin/gorilla/Vue.js</p>
                    </div>
                </div>
                <div class="lang-2">
                    <h5>学習経験あり</h5>
                    <div class="row-container">
                        <p>Nuxt.js</p>
                    </div>
                </div>
            </div>
            <div class="language">
                <h3>インフラ</h3>
                <div class="row-container">
                    <p>heroku, netlify, firebase</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { TimelineLite } from "gsap";
export default {
    name: 'home',
    data() {
        return {
            show: true,
        }
    },
    mounted() {
        const { box } = this.$refs
        const timeline = new TimelineLite()
        timeline.to(box, 2.5, {
                height: "100vh",
                backgroundColor: "black",
                color: "white",
            })
            .to(box, 1.5, {
                backgroundColor: "#eeeeee",
                color: "black",
            })
            .to(".container", 1, {
                width: "100vw",
                height: "15vh",
                borderBottom: "1px solid black",
            })
            .to(box, 0, {
                width: "100vw",
                height: "15vh",
                borderBottom: "1px solid black",
            })
            .to(".profile", 0, {
                display: "inline-block",
                backgroundColor: "#eee",
                height: "120vh",
            })
    }
}
</script>

<style lang="scss" scoped>
.profile {
    display: none;
    box-sizing: border-box;
    width: 100vw;
    .info {
        width: 80vw;
        box-sizing: border-box;
        max-width: 600px;
        margin: auto;
        padding: 32px;
        @media screen and (max-width: 640px) {
            width: 95vw;
        }
        a {
            text-decoration: none;
            color: blue;
            font-size: 18px;
        }
    }
    .language {
        width: 80vw;
        max-width: 600px;
        margin: auto;
        padding: 16px 32px;
        @media screen and (max-width: 640px) {
            width: 95vw;
            padding: 16px 32px;
        }
        h3 {
            padding: 16px 0px;
        }
        .lang-1,
        .lang-2 {
            h5 {
                font-size: 16px;
            }
            .row-container {
                display: flex;
                flex-flow: row nowrap;
                p {
                    font-size: 18px;
                    padding: 8px;
                }
            }
        }
    }
}

.box {
    height: 100%;
    width: 100vw;
    background-color: black;
    position: relative;
    .container {
        width: 100vw;
        height: 85%;
        display: flex;
        flex-flow: column nowrap;
        justify-content: center;
        align-items: center;
    }
    .profile {
        background-color: #eee;
        height: 3000px;
    }
}

.title {
    margin: auto;
    font-size: 32px;
}
</style>




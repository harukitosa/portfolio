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
            <div class="language">
                <h2>Works</h2>
                <work title="学生団体warmth様" imgURL="https://warmth.netlify.com/img/logoImage.f98884c8.jpeg" type="web site(coding)" linkURL="https://warmth.netlify.com/"/>
                <work title="eigorilla" imgURL="https://eigorilla-app.com/img/eigorilla.b6d7ee8d.png" type="web application" linkURL="https://eigorilla-app.com/"/>
            </div>
            <div class="language">
                <h2>painting</h2>
                <work title="学生団体warmth様" imgURL="https://lh3.googleusercontent.com/AP3mYvO0419nDGAQMJG6RGcAYS4lJ--TKdbvWzHl6_fHpfDERFzaVIm0gXXOhCSuBKaghiImTWBa24_JliBE1zlvgpHKVCa1-mTxZ6Vb3UIewK63tJeqavBvD2Vl15oyRxjCCugXZyDmLZizJYBHiy1zRrlNG3usW4-PkuT7Zx-yIvFyQ6ktHUbsAgwGq3yl9vNQjrAJ0v60abX3omBf6pO3obI2ptO7A8l-i-KMTvxiZmBr4bFAY2Nk5juOYFolRd0MxyXkW--IO6_W4htL59IWMqNB1VOBYqaU23d9g4-N7NdhN20TxhkBSSYgjV1HbwF-cdOfZQm-KcdUpyL2POA1A8vzCzJQyyyj0IrLOhNJ_F_HTJJOOjkGRXakxfszLQ2-klw02qACEqxdPTwWy1pr0m1kEQbZFFTp_kmyLnJvhULMUnD9YXq8o_ls4tdDeumfcg349KV_6TcINUWQXWgM5yk_crpEL_EH2igp-4tVoxnSSqCqTs2IQdfmqcQB8V7WeyJnLreKhADX7fX9U7pmJkYwcZ7LHfIAOp5eDNogIBmv8tAAn8n2wrqL_AIU8wjO8lH2YpOSwhaeeJw043gFzMNryyzNphOx6jr4sxqrvseBxaoRk0568i2_8DX2sNi-AJJvEzCQ5K2SOINwcvmaFf0iVP-8U2EfJIvjc5ZmAs98ujuxpg=w581-h774-no" type="web site(coding)" linkURL="https://warmth.netlify.com/"/>
                <work title="eigorilla" imgURL="https://eigorilla-app.com/img/eigorilla.b6d7ee8d.png" type="web application" linkURL="https://eigorilla-app.com/"/>
            </div>
        </div>
    </div>
</template>

<script>
import { TimelineLite } from "gsap";
import Work from "@/components/WorkApp.vue"
export default {
    name: 'home',
    data() {
        return {
            show: true,
        }
    },
    components: {
        Work,
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
                height: "320vh",
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
                flex-flow: column nowrap;
                p {
                    font-size: 18px;
                    padding: 8px;
                }
            }
        }
    }
}

.box {
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
    }
}

.title {
    margin: auto;
    font-size: 32px;
}
</style>




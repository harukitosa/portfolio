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
                <work  imgURL="https://lh3.googleusercontent.com/AP3mYvO0419nDGAQMJG6RGcAYS4lJ--TKdbvWzHl6_fHpfDERFzaVIm0gXXOhCSuBKaghiImTWBa24_JliBE1zlvgpHKVCa1-mTxZ6Vb3UIewK63tJeqavBvD2Vl15oyRxjCCugXZyDmLZizJYBHiy1zRrlNG3usW4-PkuT7Zx-yIvFyQ6ktHUbsAgwGq3yl9vNQjrAJ0v60abX3omBf6pO3obI2ptO7A8l-i-KMTvxiZmBr4bFAY2Nk5juOYFolRd0MxyXkW--IO6_W4htL59IWMqNB1VOBYqaU23d9g4-N7NdhN20TxhkBSSYgjV1HbwF-cdOfZQm-KcdUpyL2POA1A8vzCzJQyyyj0IrLOhNJ_F_HTJJOOjkGRXakxfszLQ2-klw02qACEqxdPTwWy1pr0m1kEQbZFFTp_kmyLnJvhULMUnD9YXq8o_ls4tdDeumfcg349KV_6TcINUWQXWgM5yk_crpEL_EH2igp-4tVoxnSSqCqTs2IQdfmqcQB8V7WeyJnLreKhADX7fX9U7pmJkYwcZ7LHfIAOp5eDNogIBmv8tAAn8n2wrqL_AIU8wjO8lH2YpOSwhaeeJw043gFzMNryyzNphOx6jr4sxqrvseBxaoRk0568i2_8DX2sNi-AJJvEzCQ5K2SOINwcvmaFf0iVP-8U2EfJIvjc5ZmAs98ujuxpg=w581-h774-no"/>
                <work imgURL="https://lh3.googleusercontent.com/Z4lMcyV0Ud-YHOp-rRBicejl5cSK4lz1o3bPaNZtPEC72gbILRMglfHsrUKbMwmm-9uoXwSf5eoYzOsyD8ce0gkhJP5_guik3ppioquV1xMfakbMdetj77cTzmF9kq39rPtouAF3XffhLU9AmkDrvX87-EKyo5zPO7AQrTeUayQdRf03B1aVxt9W_37lQ385ykvAJrEHCo14lc1j3vtYd26JExdAZXa7uVn6RG7QtHc5JAjhjIfAmXorP6nAxGBJkhZTPITD1hQGAfv1-I65ozVM7Rgb3Egk2Zi2jbwMasaq_9gVGurR98PuZUKPBOkng6hd0wIcdAj26NQAqb8f1lwriEawf0x93vPYewDfFY704DIiAxkVV2FYm9o6g8uUU1siZbs3CMxHH5TvY6-N4UKufU7f685jkOeuls--iKHDS2tM6sXoeRsW9hAkbMVKjrG0EPBH7ugDiSlYmjL4QvRd-1x4o1ZImDxJBmerMXo2oIzDXySPmtTckk0-CdQ0ZcJ1bO-aD8SvCWxVaW89QB3qe4Uh_FDn3xSpsCFkA8hg2YbL09qL272sZeEJw7TDIGmThMxjRCsKNCQyJdqtgFWxaik0bT9RZ_dvt2gk17oOUY6RshS-cT5LHone2m9RLFD-rJ1EZ7haQjCAkwFyq4S6oMqhOu74370_raUmpQ0ClX0s1fXGpA=w207-h259-no" />
                <work imgURL="https://lh3.googleusercontent.com/Ip7afjPs5lSL4Z8ePZx-f7AtKJEqTbNyTyP3xqytcz6mjF5mXSJAkM2vCHOu2eOzREa4m9y8S_kQKJeFPrwihRtwaZXB-cYKgmY376f8XTBL2crdH6GlVmxU_aQRLf3uba2NLvPkev0cfY7KjjK5lvBt5TLHGRxUioXNQTCTtQr_WS1687waUCwCgn1d-vJ29_gM6cmqa03k1P8a5znQABsEZw-VZFESyu4skiRkltoJpFl8JfRq_NSow7K6690RZc40xgPe6umHI3dUH6qsXH0Ni0EyIKyMof3I_G72NvDetNZiMXHGi0pYh1J8MOQyzWNoJJx05I2OfFgmlQm-kh3GcNBl-zfA3rNsBzzIpvvmTSAZ7P9H9kmQ8my_m_oURYRTd71gnFYw-EQgJS1F24peFTbUJlE9A6hFOHTdbWqIKx_5k0qD7ScIcsYueJTbOE0lST67RASRKT-uKHZDmVI2lgm60N8iDNG5EUo0e-vooI67DvYg8zQYQJgywaj3SZe2DUgGYwTdpi7_WK0zf8LskJjyCeyB0XwgTZGmpgasbDFTeeVUTd01w6lVPs1z--CGBUn3BOkCUIRaxFRl7QdHYqLTeahkGgiBCmCObozo2i793FkCxiasEaBV0oqplDtlQe9T9omZUQjjMzW2G-6KrBVPBoL2UEpYjOY3LBfItU0yvr8buA=w552-h774-no"/>
            </div>
            <div class="language">
                <h2 class="contact">contact</h2>
                <div class="lang-1">
                    <h5>Webサイト制作承っております。</h5>
                    <p>TwitterのDMまたはメールアドレス13haruki28@gmail.comまでご連絡ください。</p>
                </div>
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
                height: "380vh",
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
        .contact {
            margin-bottom: 12px;
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




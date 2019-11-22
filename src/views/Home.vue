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
            <h3>github</h3>
            <h3>twitter</h3>
            <h3>Mail</h3>
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
                // repeat: 1,
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
                display: "block",
                backgroundColor: "#eee",
                height: "120vh",
            })
    }
}
</script>

<style lang="scss" scoped>
.profile {
    display: none;
    width: 100vw;
    .info {
      width: 80vw;
      max-width: 600px;
      margin: auto;
      @media screen and (max-width: 640px) {
        width: 100vw;
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




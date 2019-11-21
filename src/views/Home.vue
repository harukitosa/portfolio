<template>
    <div class="home">
        <div ref="box" class="box">
            <div class="container">
                <h1 id="title">Portfolio</h1>
                <p>Haruki Tosa</p>
            </div>
            <div v-if="this.show" class="profile">
                <h2>Haruki Tosa</h2>
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
            .to(".profile", 0, {
                display: "block"
            })
    }
}
</script>

<style lang="scss" scoped>
.profile {
    display: none;
}

.box {
    height: 100%;
    width: 100%;
    background-color: black;
    position: relative;
}

.container {
    width: 100vw;
    height: 100%;
    display: flex;
    flex-flow: column nowrap;
    justify-content: center;
    align-items: center;
}

.title {
    margin: auto;
    font-size: 32px;
}
</style>




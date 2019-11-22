<template>
    <div class="work">
        <a :href=linkURL>
            <img :src=imgURL alt="">
        </a>
        <p>{{title}}</p>
        <p>{{type}}</p>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        type: String,
        imgURL: String,
        linkURL: String,
    }
}
</script>

<style lang="scss" scoped>
.work {
    padding: 32px;
    width: 60vw;
    max-width: 450px;
    display: flex;
    flex-flow: column nowrap;
    justify-content: center;
    img {
        width: 60vw;
        max-width: 450px;
        margin: auto;
        background-color: white;
    }
    p {
        font-size: 16px;
        font-weight: 500;
    }
}
</style>

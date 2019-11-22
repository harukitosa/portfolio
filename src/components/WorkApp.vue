<template>
    <div class="work">
        <img src="https://warmth.netlify.com/img/logoImage.f98884c8.jpeg" alt="">
        <p>学生団体warmth</p>
        <p>web site(coding)</p>
    </div>
</template>

<script>
export default {
    props: {
        Title: String,
        Type: String,
        ImgURL: String,
    }
}
</script>

<style lang="scss" scoped>
.work {
    padding: 32px;
    display: flex;
    flex-flow: column nowrap;
    justify-content: center;
    img {
        width: 60vw;
        max-width: 450px;
        margin: auto;
    }
    p {
        font-size: 16px;
        font-weight: 500;
    }
}
</style>

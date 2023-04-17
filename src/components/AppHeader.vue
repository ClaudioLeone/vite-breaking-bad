<script>
export default {
    name: "AppHeader"
}
</script>

<template>
    <div class="header d-flex align-items-center">
        <div class="img-container">
            <img src="/Yu-Gi-Oh_Pyramid_Eye_Icon_II.png" alt="">
        </div>

        <div class="title-container">
            <h1>Yu-Gi-Oh API</h1>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style.scss" as *;

h1 {
    margin: 0;
    font-size: 1.7rem;
}
.header {
    height: var(--header-height);
    background-color: wheat;

    .img-container {
        height: var(--header-height);
        margin-left: 1rem;

        img {
            height: var(--header-height);
        }
    }
    .title-container {
        margin-left: 1rem;
    }
}
</style>
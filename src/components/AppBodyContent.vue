<script>
    export default {
        name: "AppBodyContent"
    }
</script>

<template>
    <div class="body">
        <div class="content">
            
            <div class="card-container">
                <div class="card-container-header">

                </div>

                <div class="card-container-body">

                </div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style.scss" as *;

.body {
    background-color: orangered;
    height: calc(100vh - var(--header-height));
}

.content{
    height: calc(100vh - var(--header-height));
    width: 85%;
    margin: 0 auto;
}

</style>
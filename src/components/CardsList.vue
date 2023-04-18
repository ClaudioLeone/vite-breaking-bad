<script>
    import AppCard from "./AppCard.vue";
    import { store } from "../store";

    export default {
        name: "CardsList",
        components: { AppCard },
        data() {
            return {
                store
            }
        }
    }
</script>

<template>
    <div class="container">
        <h4 class="text-center mt-3">Cards List</h4>

        <div class="row row-cols-4">
            <div class="col" v-for="card in store.cards" :key="card.id">
                <AppCard />
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style.scss" as *;

</style>
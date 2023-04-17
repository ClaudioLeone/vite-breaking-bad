<script>
  import { store } from "./store";

  export default {
    data() {
      return {
        store
      }
    }
  }
</script>

<template>
 <h1 v-for="(greeting, index) in store.greetings" :key="index">{{ greeting }}</h1>
</template>

<style scoped lang="scss">
@use "./style.scss" as *;

</style>

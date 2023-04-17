<script>
  import { store } from "./store";
  import AppHeader from "./components/AppHeader.vue";
  import AppBodyContent from "./components/AppBodyContent.vue";

  export default {
    components: {
      AppHeader,
      AppBodyContent
    },
    data() {
      return {
        store,
      }
    }
  }
</script>

<template>
  <AppHeader />
  <AppBodyContent />
</template>

<style lang="scss">
@use "./style.scss";

</style>

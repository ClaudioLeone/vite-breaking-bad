<script>
  import { store } from "./store";
  import AppHeader from "./components/AppHeader.vue";
  import CardsList from "./components/CardsList.vue";
  import axios from "axios";

  export default {
    components: {
      AppHeader,
      CardsList
    },
    data() {
      return {
        store,
      }
    },
    mounted() {
      axios.get("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0").then(resp => {
        this.store.cards = resp.data.data;
        console.log(this.store.cards);
      })
    }
  }
</script>

<template>
  <AppHeader />
  <CardsList />
</template>

<style lang="scss">
@use "./style.scss";

</style>

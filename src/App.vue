<script>
import TheHeader from "./components/TheHeader.vue";
import TheMain from "./components/TheMain.vue";
import TheFooterUp from "./components/TheFooterUp.vue";

export default {
  components: {
    TheHeader,
    TheMain,
    TheFooterUp
  }
};
</script>

<template>
  <TheHeader></TheHeader>
  <TheMain></TheMain>
  <TheFooterUp></TheFooterUp>
  
</template>

<style lang="scss">
@use "./styles/general.scss";

</style>

<script>
import Header from "./components/Header.vue";
import AppContent from "./components/AppContent.vue";
import AppMenu from "./components/AppMenu.vue";
import AppJumbo from "./components/AppJumbo.vue";

export default {
  components: {
    Header,
    AppContent, 
    AppMenu, 
    AppJumbo
  }
}


</script>

<template>

<Header></Header>
<AppContent></AppContent>
<AppMenu></AppMenu>
<AppJumbo></AppJumbo>

</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
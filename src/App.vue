<template>
  <div >
    
    <HeaderComponent />

    <JumboComponent />

    <MainComponent />

    <FloatingComponent />

    <FooterComponent />

  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import FloatingComponent from "./components/FloatingComponent.vue";
import JumboComponent from "./components/JumboComponent.vue";


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    FloatingComponent,
    JumboComponent
}
}
</script>

<style lang="scss">
@import "./assets/img/style/vars";

*{
  font-family: $main-font;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

</style>

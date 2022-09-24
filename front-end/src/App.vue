<template>
  <div class="body">
    <Nav class="above"/>
    <router-view v-slot="{ Component }">
      <transition name="fade" mode="out-in">
        <component :is="Component"/>
      </transition>
    </router-view>
    <Footer />
  </div>
</template>

<script>
import Nav from "@/components/Nav.vue"
import Footer from "@/components/Footer.vue"

export default {
  name: "App",
  components: {
    Nav,
    Footer, 
}
}
</script>

<style>

  @font-face {
    font-family: "Roboto";
    src: url("assets/fonts/Roboto-Regular.ttf");
  }

  body, html {
    margin: 0;
    padding: 0;
    font-family: "Roboto", Arial, Helvetica, sans-serif;
    background-color: #FEFCFD;
  }

  .above{
    z-index: 2;
    position: relative;
  }

</style>
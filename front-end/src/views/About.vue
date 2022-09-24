<template>
  <div class="about">
    <MainSection titleM="Upoznaj Istek!"/>
    <AboutUs />
    <Mission />
    <Internacional />
  </div>
</template>

<script>

import MainSection from "../components/MainSection.vue"
import AboutUs from "../components/about-us/AboutUs.vue"
import Mission from "../components/about-us/Mission.vue"
import Internacional from "../components/about-us/Internacional.vue"


export default {
  name: "Home",
  components: {
    MainSection,
    AboutUs,
    Mission,
    Internacional
}
}

</script>


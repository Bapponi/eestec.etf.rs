<template>
  <div>
    <MainSection titleM="POWER YOUR FUTURE"/>
    <AfterMain/>
    <News/>
    <ToldAboutUs/>
  </div>
</template>

<script>

import MainSection from "../components/MainSection.vue"
import AfterMain from "../components/home/AfterMain.vue"
import News from "../components/home/News.vue"
import ToldAboutUs from "../components/home/ToldAboutUs.vue"

export default {
  name: "Home",
  components: {
    MainSection,
    AfterMain,
    News,
    ToldAboutUs
}
}

</script>

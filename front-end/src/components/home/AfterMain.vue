<template>
    <div class="after-main">
        <img src="../../assets/ilustrations/crkvaR.png" alt="church" id="churchImg">
        <NumberPanel/>
        <InfoCard title="Istek LK Beograd" text="Udruženje studenata elektrotehnike Evrope – Istek 
        (Electrical Engineering STudents’ European assoCiation – EESTEC) predstavlja apolitičnu, nevladinu 
        i neprofitnu organizaciju koja okuplja studente elektrotehnike i računarstva. Slobodno možemo reći 
        da je ovo udruženje najveći međunarodni projekat koji međusobno povezuje studente elektrotehnike. 
        Osnovano je 1986. godine u Ajndhovenu, Holandija. Danas je administrativno sedište organizacije u 
        lokalnom komitetu Delft, Holandija."/>
    </div>
</template>

<script>
import NumberPanel from "@/components/NumberPanel.vue"
import InfoCard from "../InfoCard.vue"

export default {
  name: "AfterMain",
  components: {
    NumberPanel,
    InfoCard
}
}
</script>

<style>
.after-main{
    position: relative;
    margin-top: 0px;
    width: 100%;
    min-height: 900px;
}

#churchImg{
    left: 100px;
    top: 75px;
    opacity: 0.5;
    position: absolute;
    width: 40vw;
}


</style>
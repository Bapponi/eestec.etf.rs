<template>
    <div class="mission">
        <div class="ilustracije">
            <img class="ilustracija" src="../../assets/ilustrations/genexW.png" alt="genex">
            <img class="ilustracija" src="../../assets/ilustrations/pobednikW.png" alt="pobednik">
            <img class="ilustracija" id="muzej" src="../../assets/ilustrations/muzejW.png" alt="muzej">
        </div>
        <h2 class="missionTitle">Misija i vizija Isteka</h2>
        <InfoCard text="Udruženje studenata elektrotehnike Evrope – Istek 
        (Electrical Engineering STudents’ European assoCiation – EESTEC) predstavlja apolitičnu, nevladinu 
        i neprofitnu organizaciju koja okuplja studente elektrotehnike i računarstva. Slobodno možemo reći 
        da je ovo udruženje najveći međunarodni projekat koji međusobno povezuje studente elektrotehnike. 
        Osnovano je 1986. godine u Ajndhovenu, Holandija. Danas je administrativno sedište organizacije u 
        lokalnom komitetu Delft, Holandija."/>
    </div>
</template>

<script>

import InfoCard from "../../components/InfoCard.vue"


export default {
  name: "Mission",
  components: {
    InfoCard
}
}

</script>

<style>

    .mission{
        background-color: #FA4952;
        height: 670px;
    }

    .missionTitle{
        margin: 0px;
        padding: 60px 0px 40px 7.5%;
        font-size: 45px;
        color: white;
    }

    .ilustracije{
        position: absolute;
    }

    .ilustracija{
        width: 32%;
    }

    #muzej{
        opacity: 0.6;
        transform: rotate(20deg);
        margin-bottom: 50px;
    }

@media screen and (max-width: 800px) {
    
    .mission{
        height: 1000px;
    }

    #muzej{
        margin-bottom: 10px;
    }
    
}

</style>
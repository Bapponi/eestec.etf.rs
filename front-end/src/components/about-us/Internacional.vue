<template>
    <div class="int">
        <div>
            <img class="ilustracijaInt" id="istKapija" src="../../assets/ilustrations/istocneKapijeR.png" alt="istocna Kapija">
            <img class="ilustracijaInt" id="pobednik" src="../../assets/ilustrations/pobednikR.png" alt="pobednik">
        </div>
        <div class="intContent">
            <h2 class="intTitle">Internacionala</h2>
            <div>
                <p class="intText">
                    Udruženje studenata elektrotehnike Evrope (Electrical Engineering STudents’ European assoCiation – Istek)
                    predstavlja apolitičnu, nevladinu i neprofitnu organizaciju koja okuplja studente elektrotehnike i
                    računarstva iz cele Evrope. Slobodno možemo reći da je ovo EESTEC najveći međunarodni projekat koji 
                    međusobno povezuje studente elektrotehnike. Osnovano je 1986. godine u Ajndhovenu, Holandija. 
                    Danas je administrativno sedište organizacije Cirih, Svajcarska. 
                    Organizaciji na međunarodnom nivou vode članovi Internacionalnog upravnog odbora, na čelu sa predsednikom. 
                    Upravni odbor sačinjava 5 zaslužnih članova različitih lokalnih komiteta, sa mandatom u trajanju od jedne 
                    godine, i ponosni smo što je više članova LK Beograd imalo privilegiju da tu bude uključeno tokom godina. 
                    Organizaciju na lokalnom nivou sačinjavaju Istek lokalni komiteti, od kojih svaki ima sopstveni upravni odbor, 
                    način organizovanja i članove. Po pravilu, članovi moraju biti studenti elektrotehnike ili računarstva. 
                    Danas, oni se nalaze u 42 univerzitetska centara u 23 zemalje Evrope, sa preko 5000 aktivnih članova. 
                    Ove brojke rastu svake godine prijemom novih Komiteta i širenjem postojećih. 
                </p>
                <p class="intText">
                    Tokom godine lokalni komiteti organizuju radionice, događaje akademskog karaktera na kojima se studenti 
                    susreću sa aktuelnim temama iz oblasti elektrotehnike i računarstva. Putem stručnih predavanja i poseta 
                    fabrikama i kompanijama, studenti se upoznaju sa tehničkim razvojem te zemlje kao i sa novim otkrićima 
                    i saznanjima u nauci. Svaki komitet se trudi da izabere najatraktivnije i najaktuelnije teme kojima se 
                    bave profesori na njihovom univerzitetu, kako bi to prezentovali kolegama iz drugih zemalja. Pored radionica, 
                    lokalni komiteti organizuju i razmene, događaje kulturnog i socijalnog karaktera, putem kojih studenti 
                    upoznaju tradiciju i običaje drugih naroda, ostvaruju nove kontakte, usavršavaju znanje stranih jezika 
                    i time unapređuju lične veštine. 
                </p>
            </div>
            <div class="intPaneli">
                <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
                <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
                <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
                <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
            </div>
        </div>
    </div>
</template>

<script>

import SmallCard from "../SmallCard.vue";

export default {
    name: "Internacional",
    components: { 
        SmallCard
    }
}

</script>

<style>

    .intContent{
        width: 85%;
        margin: 60px 7.5% 40px 7.5%;
    }

    .intTitle{
        margin-bottom: 40px;
        font-size: 45px;
        color: #E52A30;
    }

    .intText{
        line-height: 1.7;
    }

    .ilustracijaInt{
        position: absolute; 
    }

    #istKapija{
        right: 5%;
        width: 60%;
    }

    #pobednik{
        margin-top: 600px;
        right: 39%;
        width: 22%;
    }

    .intPaneli{
        margin: 80px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 80px;
    }


</style>
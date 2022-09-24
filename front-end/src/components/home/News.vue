<template>
    <div class="news">
        <img src="../../assets/ilustrations/muzejW.png" alt="teslaM" id="teslaM">
        <p id="newsTitle">Novosti</p>
        <div class="newsPanels">
            <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
            <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
            <SmallCard title="Naslov neke vesti!" text="Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no" more="Pročitaj više" link="https://www.google.com"/>
        </div>
    </div>
</template>

<script>

import SmallCard from "../SmallCard.vue";

export default {
    name: "News",
    components: { 
        SmallCard
    }
}
//komentari1
</script>

<style>

.news{
    padding-top: 40px;
    position: relative;
    background-color: #FA4952;
    padding-bottom: 250px;
}

#newsTitle{
    padding-top: 5px;
    padding-bottom: 35px;
    margin-left: 9%;
    font-size: 50px;
    color: white;
}

.newsPanels{
    gap: 30px;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

#teslaM{
    left: 56%;
    top: 27%;
    opacity: 0.5;
    position: absolute;
    width: 40vw;
}

</style>

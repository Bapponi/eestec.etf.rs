<template>
    <div class="container">
        <div class="filter"></div>
        <img id="mainImg" src="../assets/mw20.jpg" alt="IstekMW" class="image">
        <h1 class="mainTitle">{{titleM}}</h1>
    </div>
</template>

<script>
export default {
    name: "MainSection",
    props: {
        titleM: String
    }
}
</script>

<style>
    @import 'https://assets.stoumann.dk/css/app-filtermaker.css';

.mainTitle{
    z-index: 1;
    font-family: 'JFont', sans-serif;
    position: absolute;
    color: white;
    text-shadow: var(--text-shadow);
    font-size: 6vw;
    max-width: 85%;
}

#mainImg {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: brightness(70%);
}

.container {
    margin-top:-154px ;
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.filter{
    top: 0px;
    left: 0px;
    position: absolute;
    width: 100%;
    height: 100vh;
    background: linear-gradient(0deg, rgba(229,42,48,0.6365896700477065) 43.1%, rgba(153,0,8,1) 80%) no-repeat top center;
    z-index: 1;
}


</style>
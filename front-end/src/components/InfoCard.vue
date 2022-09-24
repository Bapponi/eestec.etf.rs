<template>
    <div class="card-container">
        <div class="inner">
            <div>
                <h2 class="title">{{ title }}</h2>
                <p class="text">{{ text }}</p>
            </div>
            <div>
                <img src="../assets/mwCircle.jpg" alt="mwCircle" id="mwCircle">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "InfoCard",
    props: {
        title: String,
        text: String,
    }
}
</script>

<style scoped>

.card-container {
    display: grid;
    place-items: center;
    position: relative;
    width: 85%;
    min-height: 400px;
    height: 400px;
    aspect-ratio: 1.2;
    box-shadow: 0 5px 12px rgb(0 0 0 / 16.1%);
    border-radius: 35px;
    margin: 50px auto;
    background-color: white;
    opacity: 0.9;
}
.inner {
    gap: 0px 25px;
    max-width: 95%;
    position: relative;
    height: 95%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
}
.title {
    /* position: absolute; */
    top: 0;
    left: 0;
    font-size: 28px;
    color: #990008;
}
.text {
    /* max-width: 90%; */
    max-width: 500px;
    font-size: 18px;
    line-height: 1.4;
}
.more {
    position: absolute;
    bottom: 0;
    right: 0;
    color: #990008;
    font-weight: bold;
    font-size: 18px;
}
#mwCircle{
    width: 100%;
    border-radius: 10px;
    max-width: 500px;
}

@media screen and (max-width: 1290px) {
    .card-container {
        width: 90vw;
    }

    .text {
        /* max-width: 90%; */
        width: 40vw;
        font-size: 1.5vw;
        /* line-height: 1.4; */
    }
    
    #mwCircle{
        width: 40vw;
    }

    .title{
        font-size: 2.5vw; 
    }
}

@media screen and (max-width: 800px) {
    .card-container {
        width: 90vw;
        height: 700px;
    }

    .inner{
        display: flex;
        justify-content: center;
    }

    .text {
        /* max-width: 90%; */
        width: 350px;
        font-size: 18px;
        /* line-height: 1.4; */
    }
    
    #mwCircle{
        width: 350px;
    }

    .title{
        font-size: 26px; 
    }
}

</style>
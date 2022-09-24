<template>
    <div class="card-container">
        <div class="inner">
            <p class="text">{{ text }}</p>
            <p class="who">{{ who }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "Comment",
    props: {
        text: String,
        who: String
    }
}
</script>

<style scoped>

.card-container {
    display: grid;
    place-items: center;
    position: relative;
    width: 100%;
    height: auto;
    min-height: 300px;
    box-shadow: 0 5px 12px rgb(0 0 0 / 16.1%);
    border-radius: 35px;
    margin: 50px auto;
    background-color: white;
}
.inner {
    max-width: 95%;
    position: relative;
    height: 95%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    padding: 5px;
    justify-content: right;
    gap: 0px;
}

.text {
    font-size: 18px;
    line-height: 1.4;
}

.who{
    font-size: 22px;
    color: #FA4952;
}

@media screen and (max-width: 1100px) {
    .text{
        font-size: 1.5vw;
    }

    .card-container {
        min-height: 30vw;
    }

    .who{
        font-size: 2.0vw;
    }
}


@media screen and (max-width: 700px) {
    
    .card-container{
        margin: 30px auto;
    }

    .text{
        font-size: 16px;
    }

    .card-container {
        min-height: 200px;
    }

    .who{
        font-size: 22px;
    }
}

</style>